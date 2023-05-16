Certainly! Here are some code snippets to help you understand the concepts:

First-class functions:

```javascript
// Storing a function in a variable
const sayHello = function() {
  console.log("Hello!");
};

// Passing a function as an argument
function greet(greeting) {
  greeting();
}

greet(sayHello); // Output: Hello!

// Returning a function
function createGreeter() {
  return function() {
    console.log("Greetings!");
  };
}

const myGreeter = createGreeter();
myGreeter(); // Output: Greetings!
```

Function as an argument:

```javascript
function add(a, b) {
  return a + b;
}

function multiply(a, b) {
  return a * b;
}

function calculate(operation, a, b) {
  return operation(a, b);
}

console.log(calculate(add, 2, 3)); // Output: 5
console.log(calculate(multiply, 2, 3)); // Output: 6
```

Function invocation:

```javascript
function sayHello() {
  console.log("Hello!");
}

sayHello(); // Output: Hello!
```

Anonymous functions:

```javascript
const multiply = function(a, b) {
  return a * b;
};

const result = multiply(3, 4);
console.log(result); // Output: 12
```

Callback functions:

```javascript
function fetchData(callback) {
  // Simulating an asynchronous operation
  setTimeout(function() {
    const data = "Data from the server";
    callback(data);
  }, 2000);
}

function process(data) {
  console.log("Processing data:", data);
}

fetchData(process); // Output: Processing data: Data from the server
```

HTML:

```html
<!DOCTYPE html>
<html>
<head>
  <title>My Web Page</title>
</head>
<body>
  <h1>Welcome to My Web Page</h1>
  <p>This is a paragraph of text.</p>
  <a href="https://example.com">Visit Example</a>
  <img src="image.jpg" alt="Description of the image">
  <ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
  </ul>
</body>
</html>
```

CSS:

```css
/* Selector and Property */
h1 {
  color: blue;
}

/* Class Selector */
.my-class {
  font-weight: bold;
}

/* ID Selector */
#my-id {
  text-decoration: underline;
}

/* Box Model */
div {
  width: 200px;
  height: 100px;
  padding: 10px;
  border: 1px solid black;
  margin: 10px;
}

/* Flexbox */
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}

/* Grid */
.grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 10px;
}

/* Transition */
button {
  background-color: blue;
  color: white;
  transition: background-color 0.5s ease;
}

button:hover {
  background-color: red;
}

/* Animation */
@keyframes slide-in {
  0% {
    transform: translateX(-100%);
  }
  100% {
    transform: translateX(0);
  }
}

.box {
  width: 100px;
  height: 100px;
  background-color: blue;
  animation: slide-in 1s forwards;
}
```

I hope these code snippets help you understand the concepts better! Feel free to ask