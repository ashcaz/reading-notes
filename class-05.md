## Duckett HTML Ch.5 Images

**Adding Images**

- To add an image into a page you need to use an image tag `<img/>`(self closing tag).
- `src` tells the browser where it can find the image.

```javascript
<img src="images/quokka.jpg" alt="A family of quokka"/>
```
- you can change the height and the width of an image in the tag itself.
- Alt atribute provides a text description of the image which describes the image if you can not see it.

**Three Rules for Creating Images**

1. Save images in the right format.
2. Save images at the right size.
3. Use the Correct resolution.

**Figure and Figure Caption**

- `<figure>` contains images and thier caption so the two are associated.
- you can have more than one image inside the `<figure>` element as long as tehy all share the same caption
- `<figcaption>` allows you to add a caption to an image

## Duckett HTML Ch.11 Color

**Foreground Color**

- You can specify any color in CSS in one of three ways
  1. RGB Valves
    - `color: rgb(100,100,90);`
    - Values for red, green, and blue are expressed as numbers between 0 and 255
  2. Hex Codes
    - `color : #ee3e80;`
    - Hex values represent values for red, green and blue in hexidecimal code
  3. Color names
    - `color: DarkCyan;`
    - limited in number

**Understanding Color**

- Hue: near to the colloquial idea of color. A color can have saturationa nd brightness as well as hue
- Saturation: refers to the amount of gray in a color. At maximum saturation there will be no gray in the color. At minimum saturation the color will be mostly gray.
- Brightness: refers to how much black is in a color. At minimum brightness, there would be no black in the color and vice versa.

**Contrast**

- text is easier to read a hight contrast. ie balck bacground with white text.

## Duckett HTML Ch.12 Text

**Alignment**

- text-align: allows you to control the alignment of text. Can take one of 4 values
  1. Left
  2. Right
  3. Center
  4. Justify: indicates that every line in a paragraph, except the last line, should be set to take up the full width of of the containing box.



