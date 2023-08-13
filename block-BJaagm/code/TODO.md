1. What does thread of execution means in JavaScript?
   JavaScript is a single-threaded langauge. It executes statements one-by-one from top to bottom. This is known as thread of execution.

2. Where the JavaScript code gets executed?
   JavaScript code gets executed within global execution context. It required a special engine called JavaScript Engine which is V8 for chrome to execute a javascript program within browsers or servers.

3. What does context means in Global Execution Context?
   Context means the evironment where code is executed.

4. When do you create a global execution context.
   When a javascript program is executed, the engine first creates a global execution context.

5. Execution context consists of what all things?
   It consists of memory(heap), call stack and queue.

6. What are the different types of execution context?
   Execution context can be global and function.

7. When global and function execution context gets created?
   Global is created for every JS code when it is executed. This is the first step of any JS code execution. Function execution is created when a function is called.

8. Function execution gets created during function execution or while declaring a function.
   It is created during function execution.

9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.

```js
var user = "Arya";

function sayHello() {
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./img/image-name.jpg)

```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount) {
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/image-name.jpg)

```js
var age = 21;

function customeMessage(userAge) {
  if (userAge > 18) {
    return `You are an adult`;
  } else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)
