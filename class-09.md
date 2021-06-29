# Forms and Events
## Forms
**- Forms:** An HTML form is used to collect user input, the user input is most often sent to a server for processing.


**- Definition and Usage**: 
* The `<form>` tag is used to create an HTML form for user input.

* The `<form>` element can contain one or more of the following form elements:
    
  1.`<input>`  
  2.`<textarea>`   
  3.`<button>`      
  4.`<select>`  
  5.`<option>`  
  6.`<optgroup>`  
  7.`<fieldset>`  
  8.`<label>`  
  9.`<output>`  

**- Attributes:**

Attribute|Value|Description
---------|-----|-----------
accept-charset|	character_set|	Specifies the character encodings that are to be used for the form submission
action|	URL|	Specifies where to send the form-data when a form is submitted
autocomplete|	on/off|Specifies whether a form should have autocomplete on or off
enctype|	application/x-www-form-urlencoded multipart/form-data text/plain|Specifies how the form-data should be encoded when submitting it to the server (only for method="post")
method|	get/post|Specifies the HTTP method to use when sending form-data
name|	text|	Specifies the name of a form
rel | 	external
rel|help|Specifies the relationship between a linked resource and the current document
rel|license|Specifies the relationship between a linked resource and the current document
rel|next|Specifies the relationship between a linked resource and the current document
rel|nofollow|Specifies the relationship between a linked resource and the current document
rel|noopener|Specifies the relationship between a linked resource and the current document
rel|noreferrer|Specifies the relationship between a linked resource and the current document
rel|opener|Specifies the relationship between a linked resource and the current document
rel|prev|Specifies the relationship between a linked resource and the current document
rel|search|Specifies the relationship between a linked resource and the current document
target|_blank|Specifies where to display the response that is received after submitting the form
target|_self|Specifies where to display the response that is received after submitting the form
target|_parent|Specifies where to display the response that is received after submitting the form
target|_top||Specifies where to display the response that is received after submitting the form


* Global Attributes: The `<form>` tag also supports the *Global Attributes in HTML.*
* Event Attributes: The `<form>` tag also supports the *Event Attributes in HTML.*

**- Syntax:**

```
<form>
.
form elements
.
</form>
```

* The `<form>` element is a container for different types of input elements, such as: *text fields, checkboxes, radio buttons, submit buttons*, etc.

**-The `<input>` Element:**

* The HTML `<input>` element is the most used form element.

*An `<input>` element can be displayed in many ways, depending on the `type` attribute.
* Here are some examples:  

Type|Description 
----|----------
`<input type="text">` |Displays a single-line text input field
`<input type="radio">` |Displays a radio button (for selecting one of many choices)
`<input type="checkbox">` |Displays a checkbox (for selecting zero or more of many choices)
`<input type="submit">` | Displays a submit button (for submitting the form)
`<input type="button">` | Displays a clickable button


## Events
**- JavaScript Events:** 
* *HTML* events are "things" that happen to *HTML* elements.
* When *JavaScript* is used in *HTML* pages, *JavaScript* can "react" on these events.

**- HTML Events:** 
* An *HTML* event can be something the browser does, or something a user does.
* Here are some examples of *HTML* events:  
1. An *HTML* web page has finished loading
2. An *HTML* input field was changed
3. An *HTML* button was clicked


* Often, when events happen, you may want to do something **JavaScript** lets you execute code when events are detected.

* HTML allows event handler attributes, with *JavaScript* code, to be added to *HTML* elements. 

* With single quotes:

```
<element event='some JavaScript'>
```

* With double quotes:

```
<element event="some JavaScript">
```

**- Common HTML Events:**
* Here is a list of some common *HTML* events:

Event|Description
----|-------
onchange|An HTML element has been changed
onclick|The user clicks an HTML element
onmouseover	| The user moves the mouse over an HTML element
onmouseout	| The user moves the mouse away from an HTML element
onkeydown	|The user pushes a keyboard key
onload	|The browser has finished loading the page
