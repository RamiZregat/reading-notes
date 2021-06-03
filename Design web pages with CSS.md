# Design web pages with CSS

* **What is CSS?** *CSS* stand for (**C**ascading **S**tyle **S**heets), *CSS* describes how **HTML** elements are to be displayed on screen, paper, or in other media,also it allows you to create great-looking web pages.


* **CSS syntax:** *CSS* is a rule-based language — you define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page. For example "I want the main heading on my page to be shown as large red text."


* The following code shows a very simple CSS rule that would achieve the styling described above:


```
 h1 {
    color: red;
    font-size: 5em;
}
```

  * The rule opens with a selector . This selects the **HTML** element that we are going to style. In this case we are styling level one headings (h1).

  


* **How To Add CSS:** When a browser reads a *style sheet*, it will format the **HTML** document according to the information in the *style sheet*.


* **there is three ways to insert _CSS_:**
1. External CSS
2. Internal CSS
3. Inline CSS

* **External CSS:** With an external style sheet, you can change the look of an entire    website by changing just one file.  

Each **HTML** page must include a reference to the external style sheet file inside the link element, inside the head section.

* **Example** external styles are defined within the link element, inside the head section of an **HTML** page:


```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

* **Internal CSS:** An internal style sheet may be used if one single **HTML** page has a unique style.

The internal style is defined inside the style element, inside the head section.

* **Example** internal styles are defined within the style element, inside the head section of an HTML page:


```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

* **Inline CSS:** An inline style may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

* **Example** inline styles are defined within the "style" attribute of the relevant element:


```
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```



