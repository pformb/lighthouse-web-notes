# Module 1 - Adding Numbers


The code I had for this exercise is:

``` javascript
const args = process.argv.slice(2);
const num1 = Number(args[0]);
const num2 = Number(args[1]);
function addNumbers(num1, num2) {
  return Number(num1) + Number(num2);
};

console.log(num1 + num2);
```
### Notes from AI Feedback: 
there's a small issue. You've defined a function addNumbers(num1, num2) but you're not actually using it in your code. Instead, you're directly adding num1 and num2 in your console.log statement.

To make use of your function, you should call it inside the console.log statement like this:

``` javascript
console.log(addNumbers(num1, num2)); 
```

This way, you're actually using the function you've defined to add the numbers together.

Also, you've already converted args[0] and args[1] to numbers when you assigned them to num1 and num2. So, there's no need to convert them again inside your function. You can simplify your function to:

``` javascript
function addNumbers(num1, num2) {
  return num1 + num2;
};
```

Lastly, remember to remove the semicolon after the function declaration. In JavaScript, you don't need to put a semicolon after a function or loop declaration.


The correct code to do the adding numbers function is:



``` javascript
const args = process.argv.slice(2);
const num1 = Number(args[0]);
const num2 = Number(args[1]);

function addNumbers(num1, num2) {
  return num1 + num2;
}

console.log(addNumbers(num1, num2));
```