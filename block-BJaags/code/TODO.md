To create the execution context diagram consider the following:

- Global and Function Execution Context
- Different Phases Of Execution Context
- Var let and const

Create the execution context diagram of the following code line by line.

```js
let num = 21;
function square(num) {
  return num * num;
}
let hundred = square(10);
console.log(hundred);
```

output --
100

Create the execution context diagram of the following code line by line.

```js
var num = 21;
function addFive(n) {
  return n + 5;
}
var five = addFive(0);
var ten = addFive(5);
console.log(five, ten);
```

output --
5
10

Create the execution context diagram of the following code line by line.

```js
let marks = [34, 45, 56, 76];
function multiplyArrayByN(arr, n) {
  let finalArr = [];
  for (let elm of arr) {
    finalArr.push(elm * 2);
  }
  return finalArr;
}

let numbers = multiplyArrayByN(marks);
```

output --
there will be no output but numbers will be [68, 90, 112, 152]

Create the execution context diagram of the following code line by line.

```js
counter();
function counter(){
  let count = 0;
  funciton increment(){
    return count++;
  }
  return increment()
}
```

output --
"SyntaxError: Unexpected identifier 'increment'
at https://static.jsbin.com/js/prod/runner-4.1.8.min.js:1:13924
at https://static.jsbin.com/js/prod/runner-4.1.8.min.js:1:10866"

Create the execution context diagram of the following code line by line.

```js
counter();
let counter = function () {
  let count = 0;
  function increment() {
    return count++;
  }
  return increment();
};
```

output --

no error
