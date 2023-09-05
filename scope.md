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

```
function functionScopeExample() {
    var localVar = "I'm a local variable";

    console.log(localVar); // Accessible within the function
}

functionScopeExample(); // Output: "I'm a local variable"
// console.log(localVar); // This would result in an error because localVar is not accessible outside the function

```

## Block Scope (introduced with let and const in ES6):

Variables declared with let and const are block-scoped, meaning they are only accessible within the block (a set of curly braces) in which they are defined.

```
function blockScopeExample() {
    if (true) {
        let blockVar = "I'm a block-scoped variable";
        const blockConst = "I'm a block-scoped constant";

        console.log(blockVar); // Accessible within the block
        console.log(blockConst); // Accessible within the block
    }

    // console.log(blockVar); // This would result in an error because blockVar is not accessible here
    // console.log(blockConst); // This would result in an error because blockConst is not accessible here
}

blockScopeExample();

```
