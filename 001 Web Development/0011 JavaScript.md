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
# Data Types and Conditionals

Tags: #DataTypes #Conditionals

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

## String


