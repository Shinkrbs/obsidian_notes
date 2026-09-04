Tags: #JavaScript #JavaScriptSyntax

## A collection of JavaScript syntax found from different sources/references.

[***JavaScript Documentation***](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

---
# Objects

Tags: #Objects #NestedObjects #Objectliteralmethod

Just like in java, objects in JavaScript are of the same, it also contains its own attributes and methods. The only difference is the syntax in which how it is defined within the class but still has the same syntax when you instantiate an object.

***Declaring an object in a class file using object literal method

**Object literal method*** is a simple and concise way to create objects using **curly braces {}**.

``` JavaScript
const person = {
	// Attributes
	name = 'John',
	age = 26,
	dateOfBirth = '1991 - 12 - 05'
};
```

***Instantiating an object using new keyword :

```JavaScript
const person = new Object();

// Adding properties to new person object
person.name = 'John';
person.age = 26;
person.dateOfBirth = '1991 - 12 - 05';
```

***Nested Objects:***
	An attribute within an attribute within an attribute... .

```JavaScript
// Nested Objects

const nestedObjects = {
    layer1: {
        layer2: {
            layer3: {
                targetValue: 20
            }
        }
    }
};

// Accessing values within nested objects
console.log(nestedObjects.layer1.layer2.layer3.targetValue);
```

For more information about [objects](https://www.w3schools.com/js/js_objects.asp), access here.

---
# Functions

Tags: #Functions #Immediatelyinvokedfunctions

A block of code designed to perform a particular tasks.

***JavaScript Function***: 
	Defined with the **function** keyword, followed by a name, followed by parenthesis.
	
```JavaScript
function myFunction(){ }
```

***JavaScript Function with Parameters:***
	Same declaration as when you declare a function but inside the parenthesis it contains parameters that is used within the function.

```JavaScript
function myFunction(param1, param2){
	return param1 * param2;
}
```

**Assigning Function to Variable:***
	Also called as **anonymous functions**, typically assigned to a variable or used directly. It is often used when in need of a function for a short period. 
	
```JavaScript
const someFunction = function() {
	console.log('this is some function');
}
```

***Immediately Invoked Function***
	Immediately calls the function on runtime.

```JavaScript
(function anotherFunction() {
    console.log('hello');
})();
```
## Arrow Functions

Tags: #Arrowfunctions

An alternative to traditional function expression. It is a short yet very readable way of writing functions. 

***It is always assigned to some variable, so technically it is a way of writing anonymous functions.***

***Arrow Functions Example:***

```JavaScript
// Traditional anonymous function
(function (a) {
	return a + 100;
});

// 1. Remove the word "function" and place arrow between the argument and opening body brace
(a) => {
	return a + 100;
};	  

// 2. Remove the body braces and word "return" — the return is implied.
(a) => a + 100;

// 3. Remove the parameter parentheses
a => a + 100;
```

***Implementing an Arrow Function with Parameters***:

```JavaScript
const someVariable = (paramsOne, paramsTwo) => {
	return paramsOne + paramsTwo;
}
```

---
# JavaScript With HTML and CSS

Tags: #JavaScript #HTML #CSS 

JavaScript in making web development helps makes the web pages interactive. This section is focused on the fundamentals of JavaScript and how it can be used to manipulate all the various interactions between the web page and the user.

---
# How to Run JavaScript Code

Tags: #RunJavaScript

Running JavaScript in the html file can be done using the **script** tag.

```html
<script>  
	// JavaScript code here
	console.log("Hello World!");
</script>
```

Another way to include JavaScript in a web page is through an external script. This is very similar to linking external CSS docs to a website.

```html
<script src="javascript.js"> </script>
```

--- 
# Node.js in Web Development

Tags: #NodeJS #NodeConsole

Node.js is a JavaScript runtime environment that allows you to run JavaScript outside of you web browser. 

## Using Node Console

Node provides an interactive console which lets you run and edit your JavaScript code right in the terminal. This is quite helpful to debug or test small snippets of code quickly without opening the browser every time.

**To run the Node console, open up terminal and type node. Type .exit to quit the console.**

[What is NodeJS?](https://www.youtube.com/watch?v=uVwtVBpw7RQ)

---


Data types in JavaScript are called **dynamically typed**, meaning that there exist data types, but variables are not bound to any of them.

## Number

The number type represents both integer and floating point numbers. Besides regular numbers, there are so-called **special numeric values** which also belong to this data type: **Infinity, -Infinity, and Nan**.

**Infinity** represents mathematical infinity. It is a special value that's greater than any number. We can get it as a result of division by zero:

``` javascript
alert (1/0); //Infinity

```

Or just reference it directly: 

```javascript
alert (Infinity); //Infinity
```

**Nan** represents computational error. It is a result of an incorrect or an undefined mathematical operation, for instance:

```javascript
alert("not a number" / 2); //Nan
```

Nan is sticky. Any further mathematical operation on Nan returns Nan:

```javascript
alert( NaN + 1 ); // NaN
alert( 3 * NaN ); // NaN
alert( "not a number" / 2 - 1 ); // NaN
```

So, if there's a Nan somewhere in a mathematical expression, it propagates to the whole result (there's only one exception to that: Nan ** 0 is 1).

## BigInt

**BigInt** type was added to the language to represent integers of arbitrary length. A BigInt value is created by appending n to the end of an integer.

```javascript
// the "n" at the end means it's a BigInt
const bigInt = 1234567890123456789012345678901234567890n;
```

## Strings

**String concatenation** using the **concat()** method. It is a very useful method when you need to concatenate multiple strings together.

```js
let str1 = 'Hello';
let str2 = 'World';

let result = str1.concat(' ', str2); 
console.log(result); // Hello World
```v
```


## Typeof

The typeof operator lets you see the data type of variable or value. It always returns a string indicating a type.

```js
let num = 42;
console.log(typeof num); // "number"
```

## Symbol 

The symbol data type is a unique and immutable value that may used as an identifier for object properties.

```js
const crypticKey1= Symbol("saltNpepper");
const crypticKey2= Symbol("saltNpepper");
console.log(crypticKey1 === crypticKey2); // false
```

## Length

The length property of a string tells you how many characters it contains.

```js
let greeting = "hello";
console.log(greeting[greeting.length - 1]); // "o"
```

## Bracket Notations

Strings are treated as sequences of characters, and each character in a string can be accessed using bracket notation. 

```js
let greeting = "hello";
console.log(greeting[1]); // "e"
```

## Escaping Characters

Place backslash (\) before the statement.

```js
let statement = "She said, \"Hello!\"";
console.log(statement); // She said, "Hello!"
```

## Template Literals

Allow for easier string manipulation, including embedding variables directly inside a string, a feature known as **string interpolation**.

```js
const name = "Alice";
const greeting = `Hello, ${name}!`;

console.log(greeting);
```

```js
const name = "Alice";
const age = 25;
const message = `My name is ${name} and I am ${age} years old.`;
console.log(message);
```

Spaces without using \n
```js
let poem = `Roses are red,
Violets are blue,
JavaScript is fun,
And so are you.`;

console.log(poem);
```

Embed JavaScript expressions directly within the string.
```js
const song = "Bohemian Rhapsody";
const score = 9.5;
const highestScore = 10;
const output = `One of my favorite songs is "${song}". I rated it ${
  (score / highestScore) * 100
}%.`;
console.log(output); 
```

## Finding a substring using indexOf method

The `indexOf()` method takes two arguments: the first is the substring you want to find within the larger string, and the second is an option starting position for the search. If you don’t provide a starting position, the search will begin at the start of the string. It is important to note that the method is case sensitive.
 
```js
let sentence = "JavaScript is awesome!";
let position = sentence.indexOf("awesome!");
console.log(position); // 14
```

```js
let sentence = "JavaScript is awesome!";
let position = sentence.indexOf("fantastic");
console.log(position); // -1
```

```js
let sentence = "JavaScript is awesome, and JavaScript is powerful!";
let position = sentence.indexOf("JavaScript", 10);
console.log(position); // 27
```

```js
console.log("freeCodeCamp".indexOf("F")) // -1
```

## Prompt

The `prompt()` method is an important part of JavaScript's interaction with the user. It’s one of the simplest ways to get input from a user through a small pop-up dialog box. It opens a dialog box that asks the user for some input, and then it returns the text entered by the user as a string.

The `prompt()` method takes two arguments: The first one is the message which will appear inside the dialog box, typically prompting the user to enter information. And the second one is a default value which is optional and will fill the input field initially.

```js
prompt(message, default);
```

```html
<button id="prompt-btn">Show Prompt</button>
<p id="output"></p>
<script src="index.js"></script>
```

```js
const btn = document.getElementById("prompt-btn");
const output = document.getElementById("output");
btn.addEventListener("click", () => {
  const userName = prompt("What is your name?", "Guest");
  output.textContent = "Hello, " + userName + "!";
});
```

## ASCII

In JavaScript, you can access the numeric code of a character using the `charCodeAt()` method. This method returns the UTF-16 code unit of the character at a specified index. For the first 128 characters, this value matches the ASCII code.

```js
let letter = "A";
console.log(letter.charCodeAt(0));  // 65

let symbol = "!";
console.log(symbol.charCodeAt(0));  // 33
```

`fromCharCode()` method allows you to do the opposite: convert a UTF-16 code unit (which matches ASCII for basic characters) into its corresponding character.

```js
let char = String.fromCharCode(65);
console.log(char);  //  A
```



