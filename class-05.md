# HTML Images; CSS Color & Text
## HTML Images
**- The use of HTML Images:** 
* Images can improve the design and the appearance of a web page.

**- Typical formula for images in HTML _(Syntax)_:**
```
<img src="url" alt="alternatetext">
```
* The HTML `<img>` tag is used to embed an image in a web page.


* The `<img>` tag is empty, it contains attributes only, and does not have a closing tag.

* The `<img>` tag has two required attributes:

1. `src` - Specifies the path to the image. 
2. `alt` - Specifies an alternate text for the image.



**- Image Size - Width and Height:** ou can use the style attribute to specify the width and height of an image:
```
<img src="url" alt="alternatetext" style="width:#px;height:#px;">
```
* Always specify the width and height of an image. If width and height are not specified, the web page might flicker while the image loads.
  

## CSS Color
**- Infos about CSS Color:** 
* All modern browsers support 140 color names
* With CSS, colors can be set by using color names

**- CSS Color Values:** 
* With CSS, colors can be specified in different ways:
1. By color names.
2. As RGB values. 
3. As hexadecimal values.
4. As HSL values (CSS3).
5. As HWB values (CSS4).

* RGB Colors: An RGB color value is specified with: rgb( RED , GREEN , BLUE ).
* Hexadecimal Colors: A hexadecimal color is specified with: #RRGGBB.


## CSS Text
**- CSS** has a lot of properties for formatting text some of this properties: 
* CSS Text Overflow: The **CSS** `text-overflow` property specifies how overflowed content that is not displayed should be signaled to the user.

 * CSS Word Wrapping: The **CSS** `word-wrap` property allows long words to be able to be broken and wrap onto the next line. 

 * CSS Word Breaking: The **CSS** `word-break` property specifies line breaking rules.

 * CSS Writing Mode: The **CSS** `writing-mode` property specifies whether lines of text are laid out horizontally or vertically.

 **-** This table will summarize text effect properties:

 Property|Description
 -------|----------
 text-align-last|Specifies how to align the last line of a text.
 text-justify|Specifies how justified text should be aligned and spaced.
text-overflow|Specifies how overflowed content that is not displayed should be signaled to the user.
word-break|Specifies line breaking rules for non-CJK scripts.
word-wrap|Allows long words to be able to be broken and wrap onto the next line.
writing-mode|Specifies whether lines of text are laid out horizontally or vertically.


