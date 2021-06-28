# HTML Tables; JS Constructor Functions
## HTML Tables
**- HTML Tables:** 
* The `<table>` *HTML* element represents tabular data — that is, information presented in a two-dimensional **table** comprised of **rows** and **columns** of cells containing data.

* Each **table** may have an associated caption that provides a short description of the **table's** purpose.

* Sytnax for the table:
```
<table>
        <tr>
            <th>The table header1</th>
            <th>The table header2</th>
        </tr>
    <tbody>
        <tr>
            <td>The table body</td>
            <td>with two columns</td>
        </tr>
    </tbody>
</table>
```

* It would look like this :

The table header1|The table header2
---------|----------
The table body | with two columns

* The `<table>` tag defines an *HTML* table.
* Each table row is defined with a `<tr>` tag. Each table header is defined with a `<th>` tag. Each table data/cell is defined with a `<td>` tag.
* By default, the text in `<th>` elements are bold and centered.
* By default, the text in `<td>` elements are regular and left-aligned.

## JS Constructor Functions

**- JS Constructor Functions:**

* Object: Object is the collection of related data or functionality in the form of key. This functionalities are usually consists of several functions and variables. All JavaScript values are objects except primitives.
* Adding a property to Constructor: We cannot add a property to an existing constructor like adding a property to an object (see previous point), for adding a property we need to declare under the constructor.

* Syntax for the constructor:
```
function Person(first, last, age, eye) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eye;
}
```

* Object Types (Blueprints) (Classes):

The examples from the previous chapters are limited. They only create single objects.

Sometimes we need a "blueprint" for creating many objects of the same "type".

The way to create an "object type", is to use an object constructor function.

In the example above, function Person() is an object constructor function.

Objects of the same type are created by calling the constructor function with the new keyword:

