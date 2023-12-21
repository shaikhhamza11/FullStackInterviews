## Javascript Interview Questions

#### Q: Is Javascript a statically typed or a dynamically typed language?
**Answer:**
JavaScript is a dynamically typed language. In a dynamically typed language, the type of a variable is checked during run-time in contrast to a statically typed language, where the type of a variable is checked during compile-time.

* Static Typing
  * Variables have types
  * Variables cannot change type 
* Dynamic Typing  
  * Variables have no types
  * Variables can change type

#### Q: How Javascript works?
**Answer:** 
[Video explanation,](https://www.youtube.com/watch?v=ZvbzSrg0afE&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=2).

#### Q: How Javascript code is executed?
**Answer:** [Video explanation.](https://www.youtube.com/watch?v=iLWTnMzWtj4&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=3).

#### Q: Hoisting in Javascript?
**Answer:** [Video explanation.](https://www.youtube.com/watch?v=Fnlnw8uY6jo&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=4)

Hoisting is a JavaScript behavior where variable and function declarations are moved to the top of their containing scope during the compilation phase, allowing them to be used before they are actually declared in the code.

Let's consider an example of variable hoisting:

```js
console.log(myVar); // Output: undefined
var myVar = 10;
console.log(myVar); // Output: 10
```
In this example, even though `myVar` is being logged before it's assigned a value, JavaScript doesn't throw an error. This is because of hoisting. During compilation, the variable declaration var `myVar`; is hoisted to the top of its scope (in this case, the global scope or the scope of the function it's in). So, the code is actually interpreted like this:

```js
var myVar; // Declaration is hoisted to the top

console.log(myVar); // Output: undefined
myVar = 10; // Assignment still happens where it's written
console.log(myVar); // Output: 10
```
As you can see, the variable declaration `var myVar`; gets hoisted to the top, which is why the `console.log(myVar)` doesn't throw an error. However, the assignment `myVar = 10;` remains in its original position.

It's important to note that only the declaration is hoisted, not the initialization. If there's an initialization along with the declaration, only the declaration part is hoisted. This behavior is specific to var declarations; let and const declarations, introduced in newer versions of JavaScript, behave differently in terms of hoisting.

#### Q: How functions work in Javascript?
**Answer:** [Video explanation.](https://www.youtube.com/watch?v=gSDncyuGw0s&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=5)

#### Q: Shortest Javascript program?
**Answer:** [Video explanation.](https://www.youtube.com/watch?v=QCRpVw2KXf8&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=6)

#### Q: Undefined vs Not defined? Undefined vs Null?
**Answer:** [Video explanation.](https://www.youtube.com/watch?v=B7iF6G3EyIk&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=7)


#### Q: Scope Chain, Scope and Lexical Environment?
**Answer:** [Video explanation.](youtube.com/watch?v=uH-tVP8MUs8&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=8)

#### Q: var, let and const in JS?
**Answer:** [Video explanation.](https://www.youtube.com/watch?v=BNC6slYCj50&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=9)

#### Q: Block scope and shadowing in JS?
**Answer:** [Video explanation.](https://www.youtube.com/watch?v=lW_erSjyMeM&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=10)

#### Q: 
**Answer:** [Video explanation.]

#### Q: 
**Answer:**
#### Q: 
**Answer:**
#### Q: 
**Answer:**
#### Q: 
**Answer:**
#### Q: 
**Answer:**
#### Q: 
**Answer:**
#### Q: 
**Answer:**
#### Q: 
**Answer:**