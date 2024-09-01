- # Universal Quick Capture for Roam Research v0.1.9 Beta
- ## Changelog:
    - v0.1.9 beta [[April 5th, 2021]]
        - New feature: import Todoist subtasks nested under primary task with comments
        - Update: use Roam Research alpha API allowing faster data entry
- ## Configuration:
    - ### **Todoist Quick Capture settings:**
        - ### Mandatory Settings - All Users:
            - **Todoist Account Status:**    __(Free or Premium)__
                - #42Setting TodoistAccount <Replace with either Free or Premium>
                - Instructions:
                    - The Todoist API handles API calls from Free and Premium account holders differently, especially when it comes to comments.
                    - Please enter either Free or Premium to replace all of the text between and including the < > symbols in the 42Setting block above.
            - **Todoist API token:**
                - #42Setting TodoistApiToken <Replace with Todoist API token>
                - Instructions:
                    - {{[[video]]: https://www.loom.com/share/d8e4d6d3c31c43aca3e2ba49914787c3}}
                    - After getting your API token, replace all of the text between and including the < > symbols in the 42Setting block above.
                        - It should look something like this:
                            - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FMark_Lavercombe%2FdwaIyLRzjq.png?alt=media&token=e0277dd9-3c73-4ad3-8ece-1109c3a6ff2d)
                        - Important: Do NOT delete the TodoistApiToken part, just the part between and including the < > symbols.
            - **Todoist Inbox ID:**    __(integer)__
                - #42Setting TodoistInboxId <Replace with Inbox ID>
                - Instructions:
                    - {{[[video]]: https://www.loom.com/share/35816b92f0644c088f19c9bb471bd529}}
                    - After getting your inbox id, replace all of the text between and including the < > symbols in the 42Setting block above.
            - **Preferred tag for imported items:**
                - #42Setting TodoistImportTag <Replace with preferred Roam Research tag>
                - Instructions:
                    - Upon import into Roam Research, this script will assign a tag to items. This can be useful if you want to track imported Quick Capture items, or you want them to automatically appear in an Inbox or Quick Capture area for triaging.
                    - Note that this does not require the hashtag or square bracket symbols to be included. Just place the text you want to use and the scripts will add the hashtag and brackets.
                    - Replace all of the text between and including the < > symbols in the 42Setting block above with your preferred tag.
        - ### Todoist Premium account holders:
            - **Todoist Label Mode:**    __(Label | Unlabelled)__
                - #42Setting TodoistLabelMode <Replace with either Label or Unlabelled>
                - Instructions:
                    - This setting is Mandatory.
                    - You can choose whether to import all items from your Todoist inbox (Unlabelled mode), or only those assigned a specific label (Label mode). This might be useful if you use Todoist for task management and might capture tasks in your inbox that you don't want imported to Roam Research. If you don't use Todoist for task management it would be best to use Unlabelled mode. 
                    - Replace all of the text between and including the < > symbols in the 42Setting block above with either Label or Unlabelled.
                    - If you choose Label mode you **must** complete the Label ID block below.
                - **Todoist Label ID:**    __(integer)__
                    - Instructions:
                        - This setting is **required** if you selected Label for Todoist Label Mode.
                        - Create a label in Todoist that you wish to use for import into Roam Research. Click the button to enter your label and this SmartBlock will retrieve the label id. {{Retrieve Label id:42SmartBlock:Get Todoist Label Id:42RemoveButton=false}}    
        - ### Advanced Settings:
            - For each setting below, change False to True to use this feature.
            - Don't set a tag on imported items:
                - #42Setting TodoistNoTag False
            - Show item created data:
                - #42Setting TodoistCreatedDate False
            - Show due date:
                - #42Setting TodoistDueDates False
            - Show priority as tag:
                - #42Setting TodoistPriority False
        - ### Inbox Notifications:
            - This optional roam/js block will check your Todoist Inbox for pending items and alert you with a notification window. By default, it checks every 15 minutes. If there are pending items, it shows the notification for 3 minutes and then disappears. You can click on the message for it to go away. You can click the button to go to the Roam Research page for the tag you're using and then manually start the import.
            - If you would like to turn on notifications, please click the 'Yes, I know what I'm doing.' button in the next block.
            - {{[[roam/js]]}}
                - ```javascript
;(()=>{  
  var checkEveryMinutes = 15; //default check every 15 minutes
  var displayNotificationMinutes = 3; //default minutes notification stays visible
  setTimeout( async ()=>{
    var myToken 		 = await roam42.settings.get('TodoistApiToken');
    var TodoistInboxId   = await roam42.settings.get('TodoistInboxId');
    var TodoistLabelMode = await roam42.settings.get('TodoistLabelMode');
    var TodoistLabelId   = await roam42.settings.get('TodoistLabelId');
	var TodoistImportTag   = await roam42.settings.get('TodoistImportTag');
    
    var url = "https://api.todoist.com/rest/v1/tasks?project_id=" + TodoistInboxId + "";
    if (TodoistLabelMode == "Label") url += "&label_id=" + TodoistLabelId + "";
    
    const checkInboxAlert = async ()=> {
      var myTasks = JSON.parse($.ajax({url:url, type:"GET", async:false, headers: { Authorization: 'Bearer ' + myToken }, }).responseText);
      if(myTasks.length>0) {
        iziToast.show({
            theme: 'dark',
            message: myTasks.length+' new Quick Capture item(s)',
            position: 'bottomRight',
            buttons: [
                ['<button>Go to Page</button>', function (instance, toast) {
                    roam42.common.navigateUiTo(TodoistImportTag, true);
                }, true],
            ],
            close: false,
            timeout: 18000,
            closeOnClick: true,
            displayMode: 2
        });
      }
    }

    await checkInboxAlert();
    try {if(window.todoistInterval>0) clearInterval(window.todoistInterval)} catch(e) {}
    window.todoistInterval = setInterval( async ()=>{
      await checkInboxAlert()
    }, checkEveryMinutes * 60000);
  },10000) //wait for 42 to be running
})();```
- ## Usage:
    - Now that you have made the necessary configuration, you can start using the Todoist -> Roam Research import functions.
    - You can trigger a manual check by typing `jjuqc` and then pressing ENTER. This will work in any block within your Roam graph.
    - You could also use a button to trigger a check. This button might be useful to have within your daily notes template, for example.
        - {{Check Todoist Inbox:42SmartBlock:UQCRR - Universal Quick Capture for Roam Research:button=true,42RemoveButton=false}}
        - Simply copy the button code from the line above into your template and then trigger it whenever you like.
- 
- ---
- ## Warning: Do Not Change Below this Line 
      (unless you know what you're doing)
- ---
- ---
