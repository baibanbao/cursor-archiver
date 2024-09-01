- 
- ### suggestions
    - __(Feel free to delete anything in this section.)__
    - links
        - [PLUGIN PAGE](https://roamresearch.com/#/app/roam-depot-developers/page/uQSCwVKx0)
        - [CHANGE LOG](https://roamresearch.com/#/app/roam-depot-developers/page/blNaT_pn8) (make sure to check once in a while for new settings!)
        - [CARD BANK](https://roamresearch.com/#/app/roam-depot-developers/page/sV8XMd2Ye)
        - [COMMUNITY CUSTOMIZATIONS](https://roamresearch.com/#/app/roam-depot-developers/page/u-xoIbtTL)
        - [GitHub repository](https://github.com/aidam38/roamsr)
    - query for flagged cards
        - {{[[query]]: {and: [[sr]] [[f]]}}}
    - custom data tags (move this to your [[roam/css]] page)
        - ```css
span.rm-page-ref[data-tag="sr"] {
    background: #0059B1;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}```
- ### settings
- ### script
    - {{[[roam/js]]}}
        - ```javascript
/* roam/sr - Spaced Repetition in Roam Research
   Author: Adam Krivka
   https://github.com/aidam38/roamsr
*/

var roamsrID = "roamsr-script";
var oldRoamSR = document.getElementById(roamsrID);
if (oldRoamSR) oldRoamSR.remove();
var s = document.createElement('script');
	s.type = "text/javascript";
	s.id = roamsrID;
    s.src =  "https://serene-williams-db0c75.netlify.app/js/stable.js";
  	s.async = true;
document.getElementsByTagName('head')[0].appendChild(s);```
- ### [[roam/css]]
    - ```css
```
- 
