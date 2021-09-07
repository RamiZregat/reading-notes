# FUNCTIONAL PROGRAMMING

## Functional Programming Concepts

**- What is functional programming?**

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

**- What is a pure function and how do we know if something is a pure function?**

In computer programming, a pure function is a function that has the following properties:

1- The function return values are identical for identical arguments (no variation with local static variables, non-local variables, mutable reference arguments or input streams).


2- The function application has no side effects (no mutation of local static variables, non-local variables, mutable reference arguments or input/output streams).


**- What are the benefits of a pure function?**

The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:  
Given a parameter A → expect the function to return value B  
Given a parameter C → expect the function to return value D


**- What is immutability?**

When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.


**- What is Referential transparency?**

Basically, if a function consistently yields the same result for the same input, it is referentially transparent.


## Node.js

**- What is a module?**
Module in Node.js is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node.js application.

**- What does the word ‘require’ do?**

The basic functionality of require is that it reads a JavaScript file, executes the file, and then proceeds to return the exports object.

**- How do we bring another module into the file the we are working in?**

To include functions defined in another file in Node.js, we need to import the module. we will use the require keyword at the top of the file.

The result of require is then stored in a variable which is used to invoke the functions using the dot notation.

To see that in action, let’s import the lib.js module by requiring it inside the main.js file and invoke the add() function with dot notation.


**- What do we have to do to make a module available?**

by installing it in the termenal use npm i then type the name of the module that u wants.