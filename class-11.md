# Assorted Topics

**- HTML Images:** Images can improve the design and the appearance of a web page.

**- HTML Images Syntax:** 

```
<img src="url" alt="alternatetext">
```

* The HTML `<img>` tag is used to embed an *image* in a web page.

* Images are not technically inserted into a web page; images are linked to web pages. The `<img>` tag creates a holding space for the referenced *image*.

* The `<img>` tag is empty, it contains attributes only, and does not have a closing tag.

* The `<img>` tag has two required attributes:

1. src - Specifies the path to the *image*
2. alt - Specifies an alternate text for the *image*

**- CSS Styling Images:** 

* CSS Setting height and width: 
1. The height and width properties are used to set the height and width of an element.
2. The height and width properties do not include padding, borders, or margins. It sets the height/width of the area inside the padding, border, and margin of the element.

3. You can use the in-line method:

```
<img src= "forest.jpg" width = "300" height = "300">  
```

4. You can use the CSS file to change them (External method):

```
img {
  width: 300px;
  height: 300px;
}
```


* Rounded Images: Use the `border-radius` property to create rounded *images*:

```
<style>
img {
  border-radius: 50%;
}
</style>

```

* Thumbnail Images: Use the border property to create thumbnail images:

```
<style>
img {
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
  width: 150px;
}
</style>
```

* Responsive Images: Responsive images will automatically adjust to fit the size of the screen.


* Center an Image: To center an image, set left and right margin to `auto` and make it into a `block` element:

```
<style>
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
```

* Transparent Image: The `opacity` property can take a value from 0.0 - 1.0. The lower value, the more transparent:

```
<style>
img {
  opacity: 0.5;
}
</style>
```

* Image Filters: The `CSS` filter property adds visual effects (like blur and saturation) to an element.  

Example: Change the color of all images to black and white (100% gray):

```
img {
  filter: grayscale(100%);
}
```

* Flip an Image: Move your mouse over the image:

```
img:hover {
  transform: scaleX(-1);
}
```






