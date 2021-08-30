# Passing Functions as Props

## List and Keys
**- What does .map() return?**  
map() function returns a map object(which is an iterator) of the results after applying the given function to each item of a given iterable.

**-If I want to loop through an array and display each value in JSX, how do I do that in React?**  

The map() method is the most commonly used function to iterate over an array of data in JSX. You can attach the map() method to the array and pass a callback function that gets called for each iteration. When rendering the User component, pass a unique value to the key prop.

**Each list item needs a unique `<li>`.**

**- What is the purpose of a key?**  
Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.

- The best way to pick a key is to use a string that uniquely identifies a list item among its siblings. Most often you would use IDs from your data as keys.

- When you don’t have stable IDs for rendered items, you may use the item index as a key as a last resort.


## The Spread Operator

**- What is the spread operator?**  
Spread operator allows an iterable to expand in places where 0+ arguments are expected. It is mostly used in the variable array where there is more than 1 values are expected. It allows us the privilege to obtain a list of parameters from an array.

*  **spread operator is useful for many different routine tasks in JavaScript, including the following:**  

1. Copying an array  
2. Concatenating or combining arrays  
3. Using Math functions  
4. Using an array as arguments  
5. Adding an item to a list   
6. Combining objects  
7. Converting NodeList to an array  

**An example of using the spread operator to combine two arrays:**  


```
const myArray =['A','B','C']
const yourArray = ['D','F','G']
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // A B C D F G
```

## According to the video of Passing function between components:


 **- what is the first step that the developer does to pass functions between components?**   
 By using State.

**- what does the `increment` function do?**   
it increase the count (the number) each time the user click add on the person name. 

**- How can you pass a method from a parent component into a child component?**  
by using props `this.props`

**- How does the child component invoke a method that was passed to it from a parent component?**  
by using `this.refs.child`
