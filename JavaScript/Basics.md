# `var` vs `let` vs `const`
While a variable can be redeclared multiple times by `var`, you can declare a variable only once by `let` keyword. `const` is similar to `let`, but constants are not re-assignable.
```
var counter = 0; 
var counter = 1; //possible
.
let x = 0;
x = 2+3; // possible
let x = 1; //error
.
const AMOUNT = 5;
AMOUNT = 10; //error
```
