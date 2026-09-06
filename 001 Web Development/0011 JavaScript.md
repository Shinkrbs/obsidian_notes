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
# Strings in JavaScript

Tags: #Strings #StringsinJavaScript #FunctionsofStringsinJavaScript 

---------
## Strings

**String concatenation** using the **concat()** method. It is a very useful method when you need to concatenate multiple strings together. 

Strings are primitive data types and they are immutable. Immutability means that once a string is created, it cannot be changed.

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

**ASCII** stands for **American Standard Code for Information Interchange**.

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

## Includes Method

The `includes()` method is used to check if a string contains a specific substring. If the substring is found within the string, the method returns `true` otherwise, it returns `false`.

```js
let phrase = "JavaScript is awesome!";
let result = phrase.includes("awesome");

console.log(result);  // true
```

It's important to note that the `includes()` method is case-sensitive. This means that the exact match of the characters is required, including their case.

You can also use the `includes()` method to check for a substring starting at a specific index in the string by providing a second parameter:

```js
let text = "Hello, JavaScript world!";
let result = text.includes("JavaScript", 7);

console.log(result);  // true
```

The `includes()` method only returns a `true` or `false` result. It does not provide information on where the substring is located in the string or how many times it occurs. If you need that level of detail, other methods, such as the `indexOf()` method might be more suitable.

## Slice Method

The `slice()` method allows you to extract a portion of a string and returns a new string, without modifying the original string. It takes two parameters: the starting index and the optional ending index.

```js
string.slice(startIndex, endIndex);

let message = "Hello, world!";
let greeting = message.slice(0, 5);

console.log(greeting);  // Hello
```

If you omit the second parameter, `slice()` will extract everything from the start index to the end of the string:

```js
let message = "Hello, world!";
let world = message.slice(7);

console.log(world);  // world!
```

You can also use negative numbers as indexes. When you use a negative number, it counts backward from the end of the string:

```js
let message = "JavaScript is fun!";
let lastWord = message.slice(-4);

console.log(lastWord);  // fun!
```

Let's say you want to extract a section from the middle of a string. You can provide both the starting and ending indexes to precisely control which part of the string you want:

```js
let message = "I love JavaScript!";
let language = message.slice(7, 17);

console.log(language);  // JavaScript
```

## Change Casing of Strings

Transforming all letters to uppercase for a heading or converting text to lowercase for uniformity using `toUpperCase()` and `toLowerCase()`.

The `toUpperCase()` method converts all the characters to uppercase letters and returns a new string with all uppercase characters. This is useful when you want to emphasize text or create consistency in the format of strings.

```js
let greeting = "Hello, World!";
let uppercaseGreeting = greeting.toUpperCase();
console.log(uppercaseGreeting);  // "HELLO, WORLD!"
```

The `toLowerCase()` method converts all characters in a string to lowercase. This is helpful when you need to standardize input, such as when comparing user-provided text or making case-insensitive checks.

```js
let shout = "I AM LEARNING JAVASCRIPT!";
let lowercaseShout = shout.toLowerCase();
console.log(lowercaseShout);  // "i am learning javascript!"
```

## Trim Whitespace from a String

Trim whitespace using `trim()`, `trimStart()`, and `trimEnd()` methods.

Whitespace refers to spaces, tabs, or line breaks that occur in a string but are not visible characters. For example:

```js
let greeting = "   Hello, world!   ";
```

The `trim()` method is the most commonly used way to remove whitespace from both the beginning and the end of a string. Here's an example:

```js
let message = "   Hello!   ";
console.log(message); // "   Hello!   "
let trimmedMessage = message.trim();
console.log(trimmedMessage);  // "Hello!"
```
Note that any whitespace within the string (between words, for example) is left untouched by `trim()`.

Sometimes, you may only want to remove whitespace from either the beginning or the end of a string, but not both. This is where `trimStart()` and `trimEnd()` come in.

`trimStart()` removes whitespace from the beginning (or start) of the string.

```js
let greeting = "   Hello!   ";
console.log(greeting);  // "   Hello!   "
let trimmedStart = greeting.trimStart();
console.log(trimmedStart);  // "Hello!   "
```

`trimEnd()` removes whitespace from the end of the string.

```js
let greeting = "   Hello!   ";
console.log(greeting);  // "   Hello!   "
let trimmedEnd = greeting.trimEnd();
console.log(trimmedEnd);  // "   Hello!"
```

## Replace Parts of a String with Another

The `replace()` method in JavaScript allows you to find a specified value (like a word or character) in a string and replace it with another value. The method returns a new string with the replacement and leaves the original unchanged because JavaScript strings are immutable.

```js
string.replace(searchValue, newValue);
```

`searchValue` is the value you want to search for in the string. It can be either a string or a regular expression (regex), which describes patterns in text. This allows you to search for and manipulate strings in a flexible and powerful way. You'll learn more about regular expressions in future lessons.

The `newValue` is the value that will replace the `searchValue`. Here's a simple example:

```js
let text = "I love JavaScript!";
console.log(text); // "I love JavaScript!"
let newText = text.replace("JavaScript", "coding");
console.log(newText);  // "I love coding!"
```
The `replace()` method is case-sensitive, meaning that it will only find exact matches of the `searchValue`. By default, the `replace()` method will only replace the first occurrence of the `searchValue`

`replaceAll()` method  returns a new string for all matches to the substring.

```js
const dogsOnlySentence = exampleSentence.replaceAll("cats", "dogs");
console.log("Replacing all occurrences of cats with dogs:");
console.log(dogsOnlySentence); // I love dogs and dogs are so much fun!
```

## Repeat a String x Number of Times

The `repeat()` method is a built-in function in JavaScript that allows you to repeat a string a specified number of times.

```js
string.repeat(count);
```

`string` is the string that you want to repeat, and `count` is the number of times you want the string to be repeated. Here's an example:

```js
let word = "Hello!";
let repeatedWord = word.repeat(3);
console.log(repeatedWord);  // "Hello!Hello!Hello!"
```

The `count` parameter must be a non-negative number. If you pass a negative number, JavaScript will throw a `RangeError`. The `count` must be a finite number. If you try to repeat a string an infinite number of times or use `Infinity` as the count, you will also get a `RangeError`.

In JavaScript, `Infinity` is a special value that represents an infinite quantity. It's used to denote numbers that are larger than any finite number.

```js
let word = "Test";
console.log(word.repeat(Infinity));  // Throws RangeError: Invalid count value
```

If the count is not an integer (such as a decimal like `2.5`), the `repeat()` method will round it down to the nearest integer.

```js
let word = "Test";
console.log(word.repeat(2.5));  // "TestTest"
```

If you pass `0` as the count, the `repeat()` method will return an empty string.

```js
let word = "Test";
console.log(word.repeat(0));  // ""
```

You are not limited to passing a number directly into the `repeat()` method. You can also pass a variable that stores a number value.

```js
let count = 4;
let word = "Test";
let repeatedWord = word.repeat(count);
console.log(repeatedWord); // TestTestTestTest
```

------
# Booleans and Numbers in JavaScript

Tags: #Numbers #Booleans #NumbersinJavaScript #BooleansinJavaScript

-------

## Number Type 

 JavaScript uses one unified `Number` type to account for numbers. This means you can work with whole numbers, decimals, and even special numeric values all under the same `Number` data type umbrella.

```js
const wholeNumber = 50;
const decimalNumber = 4.5;
const negativeNumber = -7;

console.log(typeof wholeNumber); // number
console.log(typeof decimalNumber); // number
console.log(typeof negativeNumber); // number
```

JavaScript's `Number` type includes various kinds of numeric values, ranging from simple integers and floating-point numbers to special cases like `Infinity` and `NaN`, or "Not a Number".

JavaScript can represent numbers that are beyond the maximum limit with `Infinity`. You'll encounter this when you try to divide a number by zero or on rare occasions, exceed the upper boundary of the `Number` type.

```js
const infiniteNumber = 1 / 0;
console.log(infiniteNumber); // Infinity
console.log(typeof infiniteNumber); // number
```

Some mathematical operations don't result in a valid number. For instance, if you try to perform a mathematical operation on something that isn't a number, you'll get `NaN`, which stands for "Not a Number".

```js
const notANumber = 'hello world' / 2;
console.log(notANumber); // NaN
```

The type of `NaN` is also `Number`:

```js
const notANumber = 'hello world' / 2;
console.log(typeof notANumber); // number
```

## Arithmetic Operators

The addition operator is a plus sign (`+`). The addition operator allows you to find the total of two or more numbers. 

The subtraction operator is a minus sign (`-`). It allows you to find the difference between two numbers. If a smaller number comes first, you'll get a negative result.

The multiplication operator is represented by an asterisk (`*`) and is used to find the product of two or more numbers.

The division operator is a slash (`/`), which differs from the division symbol used in traditional math (`÷`). It's important to note that if you try to divide by zero, JavaScript will return `Infinity`.

The remainder operator, represented by a percentage sign (`%`), returns the remainder of a division.

The exponentiation operator, represented by a double asterisk (`**`), raises one number to the power of another.

It's possible to mix operators in a single operation or expression. When you mix different operators in a single expression, the JavaScript engine follows a system called **operator precedence** to determine the order of operations. **Operator precedence** determines the order in which operations are executed in expressions.

```js
const result = 10 + 5 * 2 - 8 / 4;
console.log(result); // 18
```

## Calculations with Numbers and Strings

In JavaScript, the `+` operator does double duty. It handles both addition and string concatenation, which is a way to join two strings together. 

When you use `+` with a number and a string, JavaScript decides to treat them both as strings and joins them together. If you check the type of the result with the `typeof` operator, you'd see it's indeed a string:

```js
const result = 5 + '10';

console.log(result); // 510
console.log(typeof result); // string
```

The same thing happens even if you switch the string and the number.

Things get more interesting when you try to perform other arithmetic operations like subtraction, multiplication, or division with a string and number. In these cases, JavaScript tries to convert the string into a number before doing the math – another type coercion! Here's what happens:

```js
const subtractionResult = '10' - 5;
console.log(subtractionResult); // 5
console.log(typeof subtractionResult); // number

const multiplicationResult = '10' * 2;
console.log(multiplicationResult); // 20
console.log(typeof multiplicationResult); // number

const divisionResult = '20' / 2;
console.log(divisionResult); // 10
console.log(typeof divisionResult); // number
```

But what if the string doesn't look like a number? Let's see what happens in that case:

```js
const subtractionResult = 'abc' - 5;
console.log(subtractionResult); // NaN
console.log(typeof subtractionResult); // number

const multiplicationResult = 'abc' * 2;
console.log(multiplicationResult); // NaN
console.log(typeof multiplicationResult); // number

const divisionResult = 'abc' / 2;
console.log(divisionResult); // NaN
console.log(typeof divisionResult); // number
```

What if you perform arithmetic operations with a boolean (`true` or `false`)? Let's see what happens. JavaScript treats booleans as numbers in mathematical operations: `true` becomes `1`, and `false` becomes `0`.

```js
const result1 = true + 1;
console.log(result1); // 2
console.log(typeof result1); // number

const result2 = false + 1;
console.log(result2); // 1
console.log(typeof result2); // number

const result3 = 'Hello' + true;
console.log(result3); // "Hellotrue"
console.log(typeof result3); // string
```

For `null` and `undefined`, JavaScript treats `null` as `0` and `undefined` as `NaN` in mathematical operations:

```js
const result1 = null + 5;
console.log(result1); // 5
console.log(typeof result1); // number

const result2 = undefined + 5;
console.log(result2); // NaN
console.log(typeof result2); // number
```

## Operator Precedence

Operator precedence determines the order in which operations are evaluated in an expression. Operators with higher precedence are evaluated before those with lower precedence.

It follows the PEMDAS rule where, parenthesis, exponents, multiplication, division, addition, and subtraction.

Associativity is what tells JavaScript whether to evaluate operators from left to right or right to left. For most operators like addition and multiplication, associativity is left to right. So, JavaScript processes these from the leftmost side of the expression to the right:

```js
const result = 10 - 2 + 3;

console.log(result); // 11
```

The exponent operator is also right-to-left associative:

```js
const result = 2 ** 3 ** 2;

console.log(result); // 512
```

## Increment and Decrement Operators

The increment and decrement operators are represented by `++` and `--`, respectively. They both allow you to adjust the value of a variable by `1`.

They come in two forms, prefix and postfix, with the difference being when the value gets updated. For the increment operator, prefix is `++x` and postfix is `x++`.

Prefix (`++x`) increases the value of the variable first, then returns a new value. Postfix (`x++`) returns the current value of the variable first, then increases it:

```js
let x = 5;

console.log(++x); // 6
console.log(x); // 6
```

Postfix:

```js
let y = 5;

console.log(y++); // 5
console.log(y); // 6
```

## Compound Assignment Operators in JavaScript

 Compound assignment operators provide a concise shorthand for an operation on a variable followed by storing the result in that same variable. They combine the operation and assignment into a shorter form like `x += y`, which is equivalent to writing `x = x + y` but without repeating the variable name.
 
```js
let num = 5;
num += 2;

console.log(num); // 7
```

## Booleans 

Booleans are a data type with only `true` and `false` values.

You can use the `Boolean()` function to check the truthiness of a value. For example, `Boolean("Hello World!")` will return `true` because `"Hello World!"` is truthy.

```js
let isOldEnoughToDrive = true;

if (isOldEnoughToDrive) {
 console.log("You're old enough to drive"); // You're old enough to drive
} else {
 console.log("Sorry, you are not old enough to drive");
}
```

To compare two values, you can use either the equality or strict equality operator. The result of the comparison will be a boolean of either `true` or `false`.

```js
console.log(5 == "5"); // true
```

In this example, JavaScript converts the string `"5"` into the number `5` and then checks if they are equal. Since both values are now the same, the result is true. The equality operator uses type coercion before checking if each value is equal.

This differs from the strict equality operator, which does not perform type coercion. The strict equality operator will check if the types are the same and if the values are the same. Here is an example using the strict equality operator to compare a number and string. This operator is represented by a triple equals sign (`===`).

```js
console.log(5 === '5'); // false
```

The following comparison will be `false`, because a string data type is not the same as a number data type.

If you need to check if something is not equal to another value, then you can use the inequality or strict inequality operators. Here is an example of using the inequality operator (`!=`) to compare a number with a string.

```js
console.log(5 != "5"); // false
```

In this example, the result would be `false` because the inequality operator first converts the string value to a number and then compares the values. Since the values would be the same it will return `false`. If you tried to use the strict inequality operator, then you would get a different result. The strict inequality operator is represented by an exclamation mark followed by two equal signs (`!==`).

```js
console.log(5 !== "5"); // true
```

The result would be `true` because the strict inequality operator does not perform any type coercion. Since the number `5` is not equal to the string `"5"`, then the result is `true`.

## Comparison Operators

Comparison operators allow you to compare two values and return a `true` or `false` result.

The greater than operator, represented by a right-angle bracket (`>`), checks if the value on the left is greater than the one on the right:

```js
let a = 6;
let b = 9;

console.log(a > b); // false
console.log(b > a); // true
```

The greater than or equal operator, represented by a right-angle bracket and the equals sign (`>=`), checks if the value on the left is either greater than or equal to the one on the right:

```js
let a = 6;
let b = 9;
let c = 6;

console.log(a >= b); // false
console.log(b >= a); // true
console.log(a >= c); // true
```

The lesser than operator, represented by a left-angle bracket (`<`) works similarly to `>`, but in reverse. It checks if the value on the left is smaller than the one on the right:

```js
let a = 6;
let b = 9;

console.log(a < b); // true
console.log(b < a); // false
```

The less than or equal operator, represented by a left-angle bracket and the equals sign (`<=`) checks if the value on the left is smaller than or equal to the one on the right:

```js
let a = 6;
let b = 9;
let c = 6;

console.log(a <= b); // true
console.log(b <= a); // false
console.log(a <= c); // true
```

## Unary Operators

Unary operators act on a single operand to perform operations like type conversion, value manipulation, or checking certain conditions.

The unary plus operator converts its operand into a number. If the operand is already a number, it remains unchanged.

```js
const str = '42';
const strToNum = +str;

console.log(strToNum); // 42
console.log(typeof str); // string
console.log(typeof strToNum); // number
```

Unary plus is handy when you want to make sure you're working with a numeric value. As you might guess, there's a unary negation operator. It negates the value of the operand. It works similarly to the unary plus, except it flips the sign.

```js
const str = '42';
const strToNegativeNum = -str;

console.log(strToNegativeNum); // -42
console.log(typeof str); // string
console.log(typeof strToNegativeNum); // number
```

The logical NOT operator, represented by an exclamation mark (`!`), is another unary operator. It flips the boolean value of its operand. So, if the operand is `true`, it becomes `false`, and if it's `false`, it becomes `true`. 

```js
let isOnline = true;
console.log(!isOnline); // false

let isOffline = false;
console.log(!isOffline); // true
```

The bitwise NOT operator is a less commonly used unary operator. Represented by a tilde, `~`, it inverts the binary representation of a number. Computers store numbers in binary format (1s and 0s). The `~` operator flips every bit, meaning it changes all 1s to 0s and all 0s to 1s.

```js
const num = 5; // The binary for 5 is 00000101

console.log(~num); // -6
```

The `void` keyword is a unary operator that evaluates an expression and returns `undefined`.

```js
const result = void (2 + 2);

console.log(result); // undefined
```

`void` is also commonly used in hyperlinks to prevent navigation:

```js
<a href="javascript:void(0);">Click Me</a>
```

The `void` keyword is a unary operator that evaluates an expression and returns `undefined`.

```js
const result = void (2 + 2);

console.log(result); // undefined
```

`void` is also commonly used in hyperlinks to prevent navigation:

```js
<a href="javascript:void(0);">Click Me</a>
```

## Bitwise Operators

Bitwise operators in JavaScript are special operators that work on the binary representations of numbers.