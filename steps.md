Step:1
```
Make assets folder which will contain images and videos folder.
```
Step:2
```
Inspect and download the svg of netflix logo by right click on logo-svg and then copy -> copy element.
```
Step:3
```
Inspect and grab the background image and then the below tv images and by inspecting locate the video tag and right click on its source link to open in new tab and then download it from there.
```
Step:4
```
Now make index.html and style.css.
-> make div.main and link external css

-> add background image to .main with height otherwise it won't be visible.

-> select * and give margin and padding 0.
-> make div.box inside div.main and give position relative to .main and position absolute to .box and top:0.

-> so that div.box sticks to .main and then control opacity by giving a black background to .box.

-> Because if .main reduces its opacity then text won't appear perfectly on it.

-> Add nav bar inside .main and above .box to keep netflix logo and language and sign In button.
```

Step:5
```
Design .main and .box:
-> add background image and position to center then background size to either cover or to max(1200px, 100vw) ---- inspect from chrome.

Design nav bar:
-> add logo, two buttons and make nav as flexbox
-> give max-width of 80vw and give margin auto as it centers the div items.

-> justify content to space-between so that netflix logo and buttons are separated to ends.
```

Step:6
```
Give nav image and buttons --> position relative so that z-index: 10 should pop them out of everything (opacity).
Coz, z-index works only on non-static positions.

-> Copy the text from Netflix title and paste under div.hero outside the div.box and obviously inside the div.main.

-> give .hero as position relative so that content pops out and keep each line of content in a separate span or div and make .hero a flexbox by keeping flex-direction as column and things at center and give height 100%.

-> add and extension WhatFont to look after the font-family of this text on netflix webpage.

-> Instead of netflix sans we got martel sans so for * keep poppins and for .hero keep martel sans and again look through WhatFont to see actual font-size, font-weight.

-> Make a div containing input type for email address and a button to get started and make background color black.

-> Give padding to .hero which is a flexbox and align all its texts to center.   ---> responsiveness.
```

Step:7
```
-> To add the dark greyish line after the title background image, observe through the chrome inspector.
-> Remove the padding from y direction from hero and then it is observed that hero takes 100% height of main but it is excluding the navbar which is of 62px.

-> That's why line exceeds 62px from the background image, so adjust the height of hero by subtracting the height of navbar from its height.

-> USE calc(100% - 62px) <--- calc() function is inbuilt func of css.
```

Step:8
```
Add class btn and btn-red and btn-red-sm to the buttons and do styling.(language, sign in and get started)

Use css peeper extension to know the colors and font size of buttons and add them in a flexbox .hero-buttons so that they appear at same level.

For input type -> give a 1px border rgba(23, 23, 23, 0.3) --- it adds transparency and opacity.
```

Step:9
```
PAGE SOURCE: view page source and CTRL+F -> find the title and copy it then paste in html title.

FAVICON: edit the www.domain.com/favicon.ico    <---------------- download the icon
       : Add link:favicon =>     <link rel="shortcut icon" href="./assets/images/favicon.ico" type="image/x-icon"> 

Create section-1 with flexbox and adjusting margin: auto ---> it centers the div elements and make the color white so that it appears.
video<> use muted also then only video will autoplay in chrome and for safari it autoplays without muted attribute also.
```

Step:10
```
FAQ:
hugeicons: go and fetch plus svg or just inspect and copy element for plus svg.
It is made flex-box of flex-boxes, internal flex-box is made to use the property justify-content: space-between, so that the questions and the plus icon get separated.

To inspect the color, either inspect and check or just add color: red (for example) in the inspect bar and it gives a pencil icon and drag it to the boxes of actual content then it will give the real color.
```