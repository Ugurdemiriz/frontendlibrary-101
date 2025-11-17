# JavaScript Guide - Complete Reference

## Table of Contents
1. [Introduction](#introduction)
2. [Variables](#variables)
3. [Data Types](#data-types)
4. [Functions](#functions)
5. [DOM Manipulation](#dom-manipulation)
6. [Events](#events)
7. [Arrays & Objects](#arrays--objects)
8. [Modern JavaScript](#modern-javascript)
9. [Best Practices](#best-practices)

## Introduction

JavaScript is a programming language that adds interactivity to web pages. It's essential for modern web development.

## Variables

### Declaration:
```javascript
// var (old way, avoid)
var oldVariable = "value";

// let (block-scoped, can be reassigned)
let variable = "value";
variable = "new value";

// const (block-scoped, cannot be reassigned)
const constant = "value";
```

## Data Types

### Primitive Types:
```javascript
// String
let name = "John";

// Number
let age = 25;
let price = 99.99;

// Boolean
let isActive = true;
let isInactive = false;

// Undefined
let undefinedVar;

// Null
let nullVar = null;
```

### Type Checking:
```javascript
typeof "text" // "string"
typeof 42 // "number"
typeof true // "boolean"
```

## Functions

### Function Declaration:
```javascript
function greet(name) {
    return `Hello, ${name}!`;
}
```

### Function Expression:
```javascript
const greet = function(name) {
    return `Hello, ${name}!`;
};
```

### Arrow Functions:
```javascript
const greet = (name) => {
    return `Hello, ${name}!`;
};

// Shorthand
const greet = name => `Hello, ${name}!`;
```

## DOM Manipulation

### Selecting Elements:
```javascript
// Single element
const element = document.querySelector('.class');
const elementById = document.getElementById('id');

// Multiple elements
const elements = document.querySelectorAll('.class');
```

### Modifying Content:
```javascript
// Text content
element.textContent = "New text";

// HTML content
element.innerHTML = "<strong>Bold text</strong>";

// Attributes
element.setAttribute('href', 'https://example.com');
element.classList.add('new-class');
element.classList.remove('old-class');
```

### Creating Elements:
```javascript
const newDiv = document.createElement('div');
newDiv.textContent = "New element";
document.body.appendChild(newDiv);
```

## Events

### Event Listeners:
```javascript
// Click event
button.addEventListener('click', function() {
    console.log('Button clicked!');
});

// Form submit
form.addEventListener('submit', function(e) {
    e.preventDefault(); // Prevent default behavior
    // Handle form submission
});

// Input change
input.addEventListener('input', function(e) {
    console.log(e.target.value);
});
```

### Event Delegation:
```javascript
// Listen on parent, handle child events
parent.addEventListener('click', function(e) {
    if (e.target.classList.contains('child')) {
        // Handle child click
    }
});
```

## Arrays & Objects

### Arrays:
```javascript
// Creating arrays
const fruits = ['apple', 'banana', 'orange'];

// Array methods
fruits.push('grape'); // Add to end
fruits.pop(); // Remove from end
fruits.map(fruit => fruit.toUpperCase()); // Transform
fruits.filter(fruit => fruit.length > 5); // Filter
fruits.forEach(fruit => console.log(fruit)); // Iterate
```

### Objects:
```javascript
// Creating objects
const person = {
    name: 'John',
    age: 30,
    greet: function() {
        return `Hello, I'm ${this.name}`;
    }
};

// Accessing properties
person.name;
person['name'];
person.greet();
```

## Modern JavaScript

### Destructuring:
```javascript
// Array destructuring
const [first, second] = [1, 2];

// Object destructuring
const { name, age } = person;
```

### Spread Operator:
```javascript
// Arrays
const newArray = [...oldArray, 'new item'];

// Objects
const newObject = { ...oldObject, newProp: 'value' };
```

### Template Literals:
```javascript
const message = `Hello, ${name}! You are ${age} years old.`;
```

### Arrow Functions:
```javascript
const add = (a, b) => a + b;
const square = x => x * x;
```

### Async/Await:
```javascript
async function fetchData() {
    try {
        const response = await fetch('https://api.example.com/data');
        const data = await response.json();
        return data;
    } catch (error) {
        console.error('Error:', error);
    }
}
```

## Best Practices

1. **Use const by default**: Only use let when reassignment is needed
2. **Meaningful names**: Use descriptive variable and function names
3. **Avoid global variables**: Keep scope local when possible
4. **Comment complex code**: Explain why, not what
5. **Error handling**: Use try-catch for async operations
6. **Modern syntax**: Use ES6+ features
7. **Performance**: Avoid unnecessary DOM queries, use event delegation

## Examples

See the `04-javascript-kategorisi/` folder for practical examples and exercises.

