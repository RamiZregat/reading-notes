# Local Storage

**- Window.localStorage:** The localStorage read-only property of the window interface allows you to access a Storage object for the Document's origin; the stored data is saved across browser sessions.

* The keys and the values stored with localStorage are always in the UTF-16 DOMString format, which uses two bytes per character. As with objects, integer keys are automatically converted to strings.


**- Definition and Usage:** 
* The localStorage and sessionStorage properties allow to save key/value pairs in a web browser.

* The localStorage object stores data with no expiration date. The data will not be deleted when the browser is closed, and will be available the next day, week, or year.

*  The localStorage property is read-only.

**- Syntax:** 

```
myStorage = window.localStorage;
```

* myStorage = window.localStorage;


* Example: Create a localStorage name/value pair with name="lastname" and value="Smith", then retrieve the value of "lastname" and insert it into the element with id="reslt":

```
// Store
localStorage.setItem("lastname", "Smith");
// Retrieve
document.getElementById("result").innerHTML = localStorage.getItem("lastname");
```

* Example2: The following example counts the number of times a user has clicked a button:


```
if (localStorage.clickcount) {
  localStorage.clickcount = Number(localStorage.clickcount) + 1;
} else {
  localStorage.clickcount = 1;
}
document.getElementById("result").innerHTML = "You have clicked the button " +
localStorage.clickcount + " time(s).";
```


