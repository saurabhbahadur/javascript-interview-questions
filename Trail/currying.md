# Currying 
-   It is used to convert a function that takes multiple function arguments. 
-   That function takes only one argument. 
-   It is used to make the code more readable and easier to understand.  
-   It is also used to make the code more flexible and reusable. 

``` js
// Original function that takes three arguments
function add(a, b, c) {
    return a + b + c;
}

// Curried version of the add function
function curriedAdd(a) {
    return function(b) {
        return function(c) {
            return a + b + c;
        };
    };
}

// Usage of the curried function
const add5 = curriedAdd(5); // Fixes the first argument to 5
const add5And10 = add5(10); // Fixes the second argument to 10
const result = add5And10(15); // Finally adds 15

console.log(result); // Output: 30
```

