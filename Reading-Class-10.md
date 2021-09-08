# In memory storage

## Understanding the JavaScript Call Stack

**- What is a ‘call’?**

call stack is a stack data structure that stores information about the active subroutines of a computer program.

**-How many ‘calls’ can happen at once?**

There is no general rule of thumb for recursive or nested functions creating a stack overflow. Instead it is dependent on the memory available on the stack, which may vary depending on underlying hardware and operating system allocations.


**- What does LIFO mean?**

When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

**- Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**

```
function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();
```


**- What causes a Stack Overflow?**

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.


## JavaScript error messages

**- What is a ‘reference error’?**
This is as simple as when you try to use a variable that is not yet declared you get this type os errors.


```
console.log(foo) // Uncaught ReferenceError: foo is not defined
```


**- What is a ‘syntax error’?**

this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

```
JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1
```


**- What is a ‘range error’?**

Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.


```
var foo= []
foo.length = foo.length -1 // Uncaught RangeError: Invalid array length
```


**- What is a ‘type error’?**

Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.


```
var foo = {}
foo.bar // undefined
foo.bar.baz // Uncaught TypeError: Cannot read property 'baz' of undefined
```


**- What is a breakpoint?**

A breakpoint is an intentional stopping or pausing place in a program, put in place for debugging purposes.


**- What does the word ‘debugger’ do in your code?**


Debugging tools (called debuggers) are used to identify coding errors at various development stages. They are used to reproduce the conditions in which error has occurred, then examine the program state at that time and locate the cause.