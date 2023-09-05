# scope :

it determines the accessblity of varible with in the javascript

## Global Scope:

Variables declared in the global scope are accessible throughout the entire JavaScript program, from any part of your code.

```
var globalVariable = "I'm a global variable";

function accessGlobal() {
    console.log(globalVariable); // Accessible inside functions
}

accessGlobal(); // Output: "I'm a global variable"
console.log(globalVariable); // Output: "I'm a global variable" (accessible globally)

```

## Function Scope:

Variables declared within a function are only accessible within that function. They are not visible outside of the function.

## Block Scope (introduced with let and const in ES6):

Variables declared with let and const are block-scoped, meaning they are only accessible within the block (a set of curly braces) in which they are defined.
