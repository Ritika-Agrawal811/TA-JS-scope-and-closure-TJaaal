Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = "Arya";
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = "Arya";
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside a block and we can't access the const variable defined inside a block from outside.

The above code will throw an error `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = "Arya";
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the if block and we can't access the variable defined by let inside an if block from outside.

The above code will throw an error `Reference Error username is not defined`.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = "Arya";
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the if block. We can access the variable defined by var inside an if block from outside.

The above code will say `Arya`.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = "John";
if (true) {
  var username = "Arya";
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope. There is same variable inside the if block also. Variable declared by var are function scope so there this variable will be global. let does not allow same variable to be declared twice so an error will be thrown.

The above code will say `SyntaxError: Identifier 'username' has already been declared`.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = "John";
if (true) {
  let username = "Arya";
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope. There is same variable inside the if block also. let variables are block scopes so varaible inside if block does not know the existance of global variable.

The above code will say `John`.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = "John";
function sayHello() {
  let username = "Arya";
}
sayHello();
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope. There is same variable inside the if block also. let variables are block scopes so varaible inside if block does not know the existance of global variable.

The above code will say `John`.

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, "First"); // output
}
console.log(i, "Second"); // output
```

Here we are looking for variable `i `. `i` is declared using var keyword. hence it is accessible outside the for loop also.

output will be --

0
"First"
1
"First"
2
"First"
3
"First"
4
"First"
5
"First"
6
"First"
7
"First"
8
"First"
9
"First"
10
"Second"

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, "First"); // output
}
console.log(i, "Second"); // output
```

Here we are looking for variable `i `. `i` is declared using let keyword. hence it is not accessible outside the for loop.

output will be --

0
"First"
1
"First"
2
"First"
3
"First"
4
"First"
5
"First"
6
"First"
7
"First"
8
"First"
9
"First"
"error"
"ReferenceError: i is not defined
at null.js:6:38
at https://static.jsbin.com/js/prod/runner-4.1.8.min.js:1:13924
at https://static.jsbin.com/js/prod/runner-4.1.8.min.js:1:10866"
