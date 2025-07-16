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

