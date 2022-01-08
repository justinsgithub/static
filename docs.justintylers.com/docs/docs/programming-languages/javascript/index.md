# JavaScript

## data types

* number 
* float
* infinity
* -infinity
* NaN
* string
* boolean
* undefined
* null

## binary operators

* \+  add
* \-  subtract
* \*  multiply
* /  divide
* %  remainder
* <  less than
* \>  greater then
* <= less than or equal to
* \>= greater than or equal to
* == equal to
* === equal to and same type
* and  2 truths
* ||  1 truth
* typeof type of a value
* ? ternary

## strange scope

!!! warning
    - creating bindings with var keyword will make it global

```Javascript
let x = 10;
if (true) {
let y = 20;
var z = 30;
console.log(x + y + z);
// → 60
}
// y is not visible here
console.log(x + z);
// → 40
```

!!! danger
    - creating functions using a function declaration make it global


```Javascript
console.log("The future says: ", future());
// The future says: You'll never have flying cars

function future() {
return "You'll never have flying cars";
}
```

## type cohersion

!!! danger
    - JavaScript will try it's best to run any code you give it
    - will perform automatic type conversion if necessary
    - this can be an unwanted behavior

```Javascript
console.log(8 * null)
// → 0
console.log("5" - 1)
// → 4
console.log("5" + 1)
// → 51
console.log("five" * 2)
// → NaN
console.log(false == 0)
// → true
```
