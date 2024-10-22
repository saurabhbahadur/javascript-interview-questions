# Intro to JS
## 1.1: Variables
There are three  types of variables in JavaScript: number, string, and boolean. We can declare a variable using the 
keyword. For example, we can declare a variable `x` and assign it the value `5` 

## Keywords
- `var` - The `var` is the oldest keyword to declare a variable in JavaScript. It has the Global scoped or function scoped.
    - If you create a variable outside of a function, you can use it anywhere in your code called as _global scope_
    - If you create a variable inside a function, you can only use it within that function called as local scope_ 
``` js
var a = 10
function f() {
    var b = 20
    console.log(a, b) // o/p 10 20
}
f();
console.log(a); // o/p 10
```
- `let` - The _`let`_ keyword is an improved version of the _`var`_ keyword. It is introduced in the ES6 or EcmaScript 2015. These variables has the block scope. It can’t be accessible outside the particular code block ({block}). 
    -   If you create a variable inside a function, you can only use it within that function called as local scope.
    -   While declearing the variable let value can be neglected. If you don’t assign any value to the variable, it will be `undefined`
    -  If you create a variable inside a block, you can only use it within that block. 
``` js
let a = 10;
function f() {
    let b = 9
    console.log(b);  //o/p 9
    console.log(a);  // o/p  10
}
f();
console.log(b); // o/p ReferenceError: b is not defined, as b is defined in a block scope so we cant access b varable.
```

- `const` - The _`const`_ keyword has all the properties that are the same as the _`let`_ keyword, 
    -   Except the user cannot update it and have to assign it with a value at the time of declaration. 
    -   These variables also have the block scope. 
    -   It is mainly used to create constant variables whose values can not be changed once they are initialized with a value.

``` js
const a = 10;
function f() {
    a = 9
    console.log(a)  //TypeError: Assignment to constant variable.
}
f();
```
## Data Types

