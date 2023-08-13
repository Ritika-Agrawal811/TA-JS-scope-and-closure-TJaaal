Find the output of the code snippets below:

```js
console.log(numA + numB); //OUTPUT
var numA = 21,
  numB = 30;
```

output --
NaN

Find the output of the code snippets below:

```js
console.log(numA + numB); //OUTPUT
let numA = 21,
  numB = 30;
```

output --
"ReferenceError: Cannot access 'numA' before initialization"

Find the output of the code snippets below:

```js
let numA = 21,
  numB = 30;
console.log(numA + numB); //OUTPUT
```

output --
51

Find the output of the code snippets below:

```js
console.log(sayHello()); // OUTPUT
function sayHello() {
  console.log("Hey");
}
function sayHello() {
  console.log("Hello");
}
```

output --
"Hello"
undefined

Find the output of the code snippets below:

```js
let username = "Tyrion";
sayHello(); // OUTPUT
function sayHello() {
  console.log(username);
}
```

output --
"Tyrion"

Find the output of the code snippets below:

```js
sayHello(); // OUTPUT
let username = "Tyrion";
function sayHello() {
  console.log(username);
}
```

output --
"ReferenceError: Cannot access 'username' before initialization"

Find the output of the code snippets below:

```js
let username = "Tyrion";
sayHello(); // OUTPUT
let sayHello = () => {
  console.log(username);
};
```

output --
"ReferenceError: Cannot access 'sayHello' before initialization"

Find the output of the code snippets below:

```js
sayHello(); // OUTPUT
let username = "Tyrion";
let sayHello = () => {
  console.log(username);
};
```

output --
"ReferenceError: Cannot access 'sayHello' before initialization"

Find the output of the code snippets below:

```js
sayHello(); // OUTPUT
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
};
```

output --
"ReferenceError: Cannot access 'sayHello' before initialization"

Find the output of the code snippets below:

```js
var username = "Tyrion";
sayHello(); // OUTPUT
let sayHello = () => {
  console.log(username);
};
```

output --
"ReferenceError: Cannot access 'sayHello' before initialization"

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
  var username = "John";
};
sayHello(); // OUTPUT
```

output --
undefined

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  var username = "John";
  console.log(username);
};
sayHello(); // OUTPUT
```

output --
"John"

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
  let username = "John";
};
sayHello(); // OUTPUT
```

output --
"ReferenceError: Cannot access 'username' before initialization"
