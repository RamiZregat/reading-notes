# HTML Links, CSS Layout, JS Functions


## HTML Links

**- What is HTML Links:**  
 * Links are found in nearly all web pages. Links allow users to click their way from page to page.  


* *HTML* links are **hyperlinks**.

* You can click on a link and jump to another document.

* When you move the mouse over a link, the mouse arrow will turn into a little hand.

* A link does not have to be text, a link can be an image or any other *HTML* element.


**- HTML Links - Syntax:** The *HTML* `<a>` tag defines a **hyperlink**. It has the following syntax:
```
<a href="url">link text</a>
```
* it will be like this [link text]()
* The most important attribute of the `<a>` element is the `href` attribute, which indicates the link's destination.

* The link text is the part that will be visible to the reader.

* Clicking on the link text, will send the reader to the specified URL address.

## CSS Layout

**- CSS Layout:** A website is often divided into headers, menus, content and a footer as shown below:  

![CSS Website Layout](https://media.geeksforgeeks.org/wp-content/uploads/website_layout-300x268.png)

* There are many different layout designs, however the structure above is one of the most common structure used.    

  

* The CSS website layout components:
1. Header: A header is usually located at the top of the website (or right below a top navigation menu). It often contains a logo or the website name.

2. Navigation Bar: A navigation bar contains a list of links to help visitors navigating through your website.

3. Content: The layout in this section, often depends on the target users interest.

4. Footer: The footer is placed at the bottom of your page. It often contains information like copyright and contact info.


## JavaScript Functions

**- What is JavaScript Functions:** 
* A JavaScript function is a block of code designed to perform a particular task.
* A JavaScript function is executed when "something" invokes it (calls it).

**- JavaScript Function Syntax:** 
*A JavaScript function is defined with the `function` keyword, followed by a name, followed by parentheses **()**.

* Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

* The parentheses may include parameter names separated by commas:
**(parameter1, parameter2, ...)**

* The code to be executed, by the *function*, is placed inside curly brackets: **{}**
 
* The typical formula (Syntax) will be as shown below:
```
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```
* Function parameters are listed inside the parentheses () in the function definition.
* Function arguments are the values received by the function when it is invoked.
* Inside the function, the arguments (the parameters) behave as local variables.

**- Function Invocation:** The code inside the function will execute when "something" **invokes** (calls) the function:
* When an event occurs (when a user clicks a button).
* When it is invoked (called) from JavaScript code.
* Automatically (self invoked).
