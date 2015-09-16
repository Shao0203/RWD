# RWD
Responsive Web Design - Swipe

#Foundation------------------------------------------
---viewport---
<meta name="viewport" content="width=device-width, initial-scale=1.0, 
user-scalable=no, maximum-scale=1.0, minimum-scale=1.0">
<link rel="stylesheet" href="css/mobile.css" media="(max-width:480px)">

---Media type---
Screen / TV / Print / Projection
<link rel="stylesheet" href="css/print.css" media="print">

---aspect-ratio---
/*visible windows width:height*/
@media(aspect-ratio: 3/2) {...}

---device-aspect-ratio---
/*device width:height*/
@media(device-aspect-ratio: 3/2) {...}

---orientation---
@media(orientation: landscape) {...}
@media(orientation: portrait) {...}

---width / height---
@media(max-width:480px) {...}
@media(min-device-width:480px) {...}
@media(max-height:480px) {...}
@media(min-device-height:480px) {...}

---Resolution---
dpi: dots per inch
@media screen and (resolution:1 dppx), 
screen and (-webkit-device-pixel-ratio:1) {...}

---And, or, not---
@media (max-width: 480px) and (max-height: 480px) {...}
@media (max-width: 480px), (max-height: 480px) {...}
@media not screen {...}

---Layout---
*Breakpoint
@media (min-width: 1200px)
.container: width 960px->1170px, mainbody 620->770 margin-right 20->30, siderbar 320->370;
@media (max-width: 959px)
.container: width->100%, mainbody->67%, siderbar->30%;
@media (max-width: 767px)
mainbody, siderbar->100% | float: none;

---Navigation---
HTML: 
<a href="#nav">openBtn</a> 
<nav id="nav">-menu-</nav>
<a href="#nav">closeBtn</a>

CSS: Two Btns display:none when width is big
@media (max-width: 767px){
	display two btns by class;
	hide nav(and closebtn) as default
	display nav(and closebtn) when nav is targeted by clicking openBtn
}