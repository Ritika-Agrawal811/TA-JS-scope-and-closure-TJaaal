1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage = function (marks, total) {
  return (marks * 100) / total;
};

let percentage = (marks, total) => (marks * 100) / total;
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};

function percentage(marks, total) {
  return (marks * 100) / total;
}
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};

function percentage(marks, total) {
  return (marks * 100) / total;
}
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};

function percentage(marks, total) {
  return (marks * 100) / total;
}
```

```js
let percentage = (marks, total) => (marks * 100) / total;

function percentage(marks, total) {
  return (marks * 100) / total;
}
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
   Functions are objects in JavaScript so they can be stored in a variable and this is called function expressions.

4. Why is a function call an expression in JavaScript?
   Because it can be passed to other functions and the return result can be assigned to a variable to store it.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // VALID
five = add; // VALID
five = five(10, 11); // VALID
five = function () {
  return "Hello";
}; // VALID
```

6. What is the difference between function definition and function call? Explain with an example.
   Function definition is declaring a function and writing all the steps that should be executed to perform a task. Function call
   means calling that function to perform those tasks by providing the arguments if required.

7. What is the similarities between function definition and function call?
   They both are expressions and can be stored in a variable.

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log("Hello World!");
}

hello.user = "Sam"; // valid
```

9. What is higher order function explain with an example.
   Higher order functions are functions which either return a function reference or receive a call back function as argument.

10. Explain what is callback function. Why you can pass a function inside a function?
    Callback function is a function which is passed in another function as argument. We can pass functions inside a function because they are objects in JavaScript and objects are expressions.
