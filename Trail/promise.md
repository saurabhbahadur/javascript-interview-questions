# _Promises_
### Promise is an Object that holds a Placeholder for a value that is not known but it will be returned in the future.
 _Note: Promise is the process, how the FetchAPI works on the function _promise_._ 
_We learn promises because, we need to know how the promise works and how to handle promises._

## _Promise States_
- Pending
- Fulfilled
- Rejected

1. _Pending :_ is the initial state of a promise.
2. _Resolved :_ is the state of a promise when it is fulfilled. 
3. _Rejected :_ is the state of a promise when it is failed.

Syntax of promise,  promise accpets two parameters - _resolve and reject_ are callback functions,

``` js 
let promise = new Promise((resolve, reject) => {
    if (/*logic*/) {
        resolve('resolved')
} else {
    reject('rejected')
```
### _Example_, how to use promise.

``` js
const isEven = (number) => {
    return new Promise((resolve, reject) => {
        // throw new Error("Hola");
        setTimeout(() => {
            if (number % 2 === 0) {
                resolve(${number} is even.);
            } else {
                reject(${number} is odd.);
            }
        }, 3000);
    });
};
```
## _Creation/Consuming a Promise_
Consuming a promise (.then(), .catch() and .finally())
- .then()  is used when the promise is resolved.
- .catch() is used when the promise is rejected.
- .finally() this will be executed irrespect of the promise is fulfilled or rejected.
``` js
isEven(5)
    .then((message) => {
        console.log(`${message}`)
    })
    .catch((error) => {
        console.log(`${error}`)
    })
    .finally(() => {
        console.log('Operation completed')
    })
```

