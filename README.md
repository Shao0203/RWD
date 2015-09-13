# RWD
Responsive Web Design - Swipe

#------------------------------------------
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

#------------------------------------------
