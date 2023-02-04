# Javascript-cheatsheet

Part 1

Variables:
Declare variables to store values in JavaScript.

var name = "John";

Data Types:
There are several data types in JavaScript like string, number, boolean, etc.

var name = "John";
var age = 30;
var isMarried = true;

Arrays:
Arrays are used to store multiple values in a single variable.
css

var names = ["John", "Jane", "Jim"];

Objects:
Objects are used to store multiple values as key-value pairs.
yaml

var person = {
name: "John",
age: 30,
isMarried: true
};

Functions:
Functions are blocks of code that can be executed whenever needed.
scss

function sayHello() {
console.log("Hello World!");
}
sayHello();

Conditional Statements:
Conditional statements are used to execute code based on certain conditions.

var age = 30;
if (age >= 18) {
console.log("You are an adult.");
} else {
console.log("You are a minor.");
}

Loops:
Loops are used to repeat a block of code multiple times.
css

for (var i = 0; i < 5; i++) {
console.log("Hello World!");
}

Events:
Events are actions that trigger JavaScript code.

document.getElementById("myButton").addEventListener("click", function() {
console.log("Button was clicked.");
});

DOM Manipulation:
The Document Object Model (DOM) can be manipulated using JavaScript.

document.getElementById("myDiv").innerHTML = "Hello World!";

AJAX:
AJAX is used to make asynchronous requests to a server.

var xhr = new XMLHttpRequest();
xhr.open("GET", "data.txt", true);
xhr.onreadystatechange = function() {
if (xhr.readyState === 4 && xhr.status === 200) {
console.log(xhr.responseText);
}
};
xhr.send();

JSON:
JSON is used to exchange data between a server and a client.

var person = {
name: "John",
age: 30,
isMarried: true
};
var personJSON = JSON.stringify(person);
console.log(personJSON);

Regular Expressions:
Regular expressions are used to match patterns in strings.
typescript

var pattern = /\d/;
var string = "123";
var result = pattern.test(string);
console.log(result);

Error Handling:
Error handling is used to handle errors in JavaScript code.
vbnet

try {
console.log(undefinedVariable);
} catch (error) {
console.error(error);
}

Template Literals:
Template literals are used to embed expressions in string literals.

var name = "John";
var message = Hello, ${name}!;
console.log(message);

Arrow Functions:
Arrow functions are a shorthand for defining functions in JavaScript.

var sayHello = () => console.log("Hello World!");
sayHello();

Spread Operator:
The spread operator is used to spread the elements of an array.
css

var numbers = [1, 2, 3];
var newNumbers = [...numbers, 4, 5];
console.log(newNumbers);

Destructuring:
Destructuring is used to extract values from objects and arrays.

var person = { name: "John", age: 30 };
var { name } = person;
console.log(name);

Classes:
Classes are a blueprint for creating objects in JavaScript.

class Person {
constructor(name, age) {
this.name = name;
this.age = age;
}
}
var john = new Person("John", 30);
console.log(john.name);

Modules:
Modules are used to organize and share code in JavaScript.

export default function sayHello() {
console.log("Hello World!");
}

// in another file
import sayHello from "./sayHello.js";
sayHello();

Promises:
Promises are used to handle asynchronous operations in JavaScript.

var promise = new Promise((resolve, reject) => {
setTimeout(() => {
resolve("Hello World!");
}, 1000);
});
promise.then(result => console.log(result));

Async/Await:
Async/await is used to simplify the handling of asynchronous operations in JavaScript.

async function getData() {
var result = await fetch("https://jsonplaceholder.typicode.com/posts");
var data = await result.json();
console.log(data);
}
getData();

Map:
The map method is used to transform elements in an array.
typescript

var numbers = [1, 2, 3];
var doubledNumbers = numbers.map(number => number * 2);
console.log(doubledNumbers);

Filter:
The filter method is used to filter elements in an array.
typescript

var numbers = [1, 2, 3, 4, 5];
var evenNumbers = numbers.filter(number => number % 2 === 0);
console.log(evenNumbers);

Reduce:
The reduce method is used to reduce an array to a single value.

var numbers = [1, 2, 3, 4, 5];
var sum = numbers.reduce((accumulator, currentValue) => accumulator + currentValue, 0);
console.log(sum);

Rest and Spread Operators:
The rest and spread operators are used to pass multiple arguments to a function or spread the elements of an array.

function addNumbers(...numbers) {
return numbers.reduce((accumulator, currentValue) => accumulator + currentValue, 0);
}
console.log(addNumbers(1, 2, 3, 4, 5));
