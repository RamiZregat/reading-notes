# Programming with JavaScript

## Control flow

* **Control flow:** The *control flow* is the order in which the computer executes statements in a script.

* Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops. 


* **Example:**
```
if (field==empty) {
    promptUser();
} else {
    submitForm();
}
```
* For example, the above excerpt might be inside a function that runs when the user clicks the Submit button for the form. The function could also include a loop, which iterates through all of the fields in the form, checking each one in turn. Looking back at the code in the `if` and `else` sections, the lines `promptUser` and `submitForm` could also be calls to other functions in the script, as you can see, control structures can dictate complex flows of processing even with only a few lines of code.  

## JavaScript Functions

* A __JavaScript function__ is a block of code designed to perform a particular task.


* __JavaScript Function Syntax:__ A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().
The code to be executed, by the function, is placed inside curly brackets: {}.


 * The typical form for **Function:**
```
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```
* The code inside the function will execute when "something" invokes (calls) the function as the typical function form u can call it like below:

```
name(parameter1, parameter2, parameter3)
```


