# RWD
Responsive Web Design - Swipe  
You may clone the code, run and swipe it on Chrome mobile emulator.  

FortAwesome/Font-Awesome & thebird/Swipe is used here, thanks.  

###Foundation
---viewport---  
`<meta name="viewport" content="width=device-width, initial-scale=1.0, 
user-scalable=no, maximum-scale=1.0, minimum-scale=1.0">`  

---Media type---  
Screen / TV / Print / Projection  
`<link rel="stylesheet" href="css/print.css" media="print">`  

---aspect-ratio---  
Browser windows - width:height  
`@media(aspect-ratio: 3/2) {...}`  

---device-aspect-ratio---  
Device - width:height  
`@media(device-aspect-ratio: 3/2) {...}`  

---orientation---  
`@media(orientation: landscape) {...}`  
`@media(orientation: portrait) {...}`  

---width / height---  
`@media(max-width:480px) {...}`  
`@media(min-device-width:480px) {...}`  
`@media(max-height:480px) {...}`  
`@media(min-device-height:480px) {...}`  

---Resolution---  
dpi: dots per inch  
`@media screen and (resolution:1 dppx), screen and (-webkit-device-pixel-ratio:1) {...}`  

---And, or, not---  
`@media (max-width: 480px) and (max-height: 480px) {...}`  
`@media (max-width: 480px), (max-height: 480px) {...}`  
`@media not screen {...}`  

---Layout---  
Breakpoint, different width defines different css style  
`@media (min-width: 1200px)`  
`.container: width 960px->1170px, mainbody 620->770 margin-right 20->30, siderbar 320->370;`  
`@media (max-width: 959px)`  
`.container: width->100%, mainbody->67%, siderbar->30%;`  
`@media (max-width: 767px)`  
`mainbody, siderbar->100% | float: none;`  

---Navigation---  
HTML part:  
`<a href="#nav" class="open toggle-btn">openBtn</a>`  
`<nav id="nav"><ul>Items[1-5]</ul></nav>`  
`<a href="#top" class="close toggle-btn">closeBtn</a>`  

CSS part:  
Two Btns are hidden as default (full-screen of browser), :target pseudo-class will be used.  
`@media (max-width: 767px){`  
`display two btns by their class`  
`hide nav(and closebtn) as default`  
`display nav(and closebtn) when nav is targeted by clicking openBtn`  
`}`  

---Image---  
`<div id="showcase"></div>`  

`#showcase {`  
  `background: url(../../img/01.jpg) 50% 50% no-repeat;`  
  `margin-bottom: 20px;`  
  **`background-size: cover;`**  
  **`padding-top: 56%;	/*image height:width*/`**  
`}`  

changing a less pixel image for small device to reduce loading time  

`@media ( max-width: 480px) {`  
`#showcase {`  
`background: url(../../img/01_s.jpg) 50% 50% no-repeat;`  
` }`  
`}`  