## Duckett HTML Ch. 16 Images (p. 406-427)

**Controlling Sizes of Images in CSS**

- You can control the size of an image using the width and height properties in CSS, just like you can for any other box

```Css
img.large {
width: 500px;
height: 500px;}
img.medium {
width: 250px;
height: 250px;}
img.small {
width: 100px;
height: 100px;}
```

**Alignning Images Using CSS**

```Css
img.align-left {
float: left;
margin-right: 10px;}
img.align-right {
float: right;
margin-left: 10px;}
img.medium {
width: 250px;
height: 250px;}
```

**Centering Images Using CSS**

- By deafault images are in-line elements. That means they flow within the surrounding text.
- In order to center an image it should be turned into a block level element.

```Css
iimg.align-center {
display: block;
margin: 0px auto;}
img.medium {
width: 250px;
height: 250px;}
```

**Repeating Imgages**

- backgroud-repeat
  - repeat: repeated both horizontally and vertically
  - repeat-x: repeated only horizontally
  - repeat-y: repeats vertically only
  - no-repeat: image shown only once

- background-attachment
  - fixed: background stays in the same position on the page
  - scroll: the background image moves up and down as the user scrolls up and down the page

  ## Ducket HTML Ch. 19 Practical Information (p.476-492)

  **SEO**

  [Back to Homepage](https://ashcaz.github.io/reading-notes)