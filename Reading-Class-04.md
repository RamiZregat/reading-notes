# Readings: React and Forms

## Forms

**- What is form element?**  
HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state.



**- What is a ‘Controlled Component’?**  
- a component that renders form elements and controls them by keeping the form data in the component's state.

- In HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with `setState()`.

**-How do we target what the user is entering if we have an event handler on an input field?**

When you need to handle multiple controlled `input` elements, you can add a `name` attribute to each element and let the handler function choose what to do based on the value of `event.target.name`.


## The Conditional (Ternary Operator)

**- Why would we use a ternary operator?**  
A ternary operator allows you to assign one value to the variable if the condition is true, and another value if the condition is false. ... A ternary operator makes the assignment of a value to a variable easier to see, because it's contained on a single line instead of an if else block.


**- Example: Rewrite the following statement using a ternary statement:**

```
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```


Solution:

```
let Answer=(x===y) ? 'true' : 'false';
console.log(Answer);
```





