- {{[[roam/js]]}}
    - ```javascript
var existing = document.getElementById("query-builder");
if (!existing) {
  var extension = document.createElement("script");
  extension.src = "https://roamjs.com/query-builder.js";
  extension.id = "query-builder";
  extension.async = true;
  extension.type = "text/javascript";
  document.getElementsByTagName("head")[0].appendChild(extension);
}```
