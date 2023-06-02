# JavaScript Note

# JavaScript Note

JavaScript is a high-level, dynamic, interpreted programming language that is used to create interactive web pages and user interfaces for web and mobile applications. It was created by Brendan Eich in 1995 and is now one of the most popular programming languages in use today.

JavaScript is often used in conjunction with HTML and CSS to create dynamic and responsive websites. It runs on the client side, meaning that it is executed by the user's web browser rather than on a server. This allows for faster and more efficient processing of user interactions and can lead to a better user experience.

Some of the key features of JavaScript include its ability to manipulate the Document Object Model (DOM) of a web page, its support for event-driven programming, and its use of functions as first-class objects. It is also a versatile language that can be used for a wide range of applications, from simple form validation to complex web applications and even mobile app development.

Overall, JavaScript is a powerful and essential tool for web developers and is likely to remain a key component of web development for the foreseeable future.

### Console.log

To write our first JavaScript code, we used a built-in function **console.log()**. We passed an argument as input data, and the function displays the output. We passed `'Hello, World'` as input data or argument in the console.log() function.

Example `console.log('Hello, World')`

## Adding JavaScript to a Web Page

JavaScript can be added to a web page in four different ways:

- ***Inline script***

Create a project folder on your desktop or in any location, name it first js and create an ***`index.html`*** file in the project folder. Then paste the following code and open it in a browser

For example: 

```
<!DOCTYPE html><html lang="en">
  <head>
    <title>first js Script</title>
  </head>
  <body>
    <button onclick="alert('Welcome to java script!')">Click Me</button>
  </body>
</html>
```

- ***Internal script***

The internal script can be written in the *`head`* or the *`body`*, but it is preferred to put it on the body of the HTML document. First, let us write on the head part of the page

```
<!DOCTYPE html><html lang="en">
  <head>
    <title>first js Script</title>
    <script>
      console.log('Welcome to java script!')
    </script>
  </head>
  <body></body>
</html>
```

- ***External script***

### External Script

Similar to the internal script, the external script link can be on the header or body, but it is preferred to put it in the body. First, we should create an external JavaScript file with .js extension. All files ending with .js extension are JavaScript files. Create a file named introduction.js inside your project directory .

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>first js Script</title>
  </head>
  <body>
   
    <script src="introduction.js"></script>
  </body>
</html>
```

- ***Multiple External scripts***

We can also link multiple external JavaScript files to a web page. Create a `helloworld.js` file inside the first js Script folder and write the following code.

<!DOCTYPE html><html lang="en">
  <head>
    <title>first js Scripts</title>
  </head>
  <body>
    <script src="./helloworld.js"></script>
    <script src="./introduction.js"></script>
  </body>
</html>

**Introduction to Data types**

In JavaScript and also other programming languages, there are different types of data types. 

For Example: **primitive data types** and **non-primitive data type.**

**primitive data types**: 

*Primitive* data types are immutable(non-modifiable) data types. Once a primitive data type is created we cannot modify it.

Type of  primitive data type: *String, Number, Boolean, undefined, Null*, and *Symbol.*

[**Number**](https://javascript.info/types#number)

- Integers: Integer (negative, zero and positive) numbers .
- Float-point numbers: Decimal number

**Examples**

`let n = 123;
n = 12.345;`

There are many operations for numbers, e.g. multiplication `*`, division `/`, addition `+`, subtraction `-`, and so on

### Strings

A collection of one or more characters between two single quotes, double quotes, or backticks.

**For Example**:

for single quotes: ’Betty’ , double quotes :”computer”.

### Booleans

A boolean value is either True or False. Any comparisons returns a boolean value, which is either true or false.

**Booleans**

A boolean value is either True or False. Any comparisons returns a boolean value, which is either true or false.

**Examples**

```
let y = 10;
let x = 5;
console.log(x < y); //true
console.log(x > y); //false

```

### 

**Undefined**

In JavaScript, if we don't assign a value to a variable, the value is undefined. In addition to that, if a function is not returning anything, it returns undefined.

**Example**

```
let x;
console.log(x); // undefined

```

### Null

Null in JavaScript means an empty value.

`let emptyValue = null`

### Non-Primitive Data Types

*Non-primitive* data types are modifiable or mutable. We can modify the value of non-primitive data types after it gets created. Let us see by creating an array. An array is a list of data values in a square bracket. Arrays can contain the same or different data types. Array values are referenced by their index. In JavaScript array index starts at zero. I.e., the first element of an array is found at index zero, the second element at index one, and the third element at index two, 

**Variables**

In JavaScript, variables are used to store data values. To declare a variable, use the `var`, `let`, or `const` keyword, followed by a name for the variable. The `var` keyword is outdated and should be avoided in modern JavaScript. The `let` and `const` keywords were introduced in ES6 and should be used instead.

A valid JavaScript variable name must follow the following rules:

A JavaScript variable name should not begin with a number.
A JavaScript variable name does not allow special characters except dollar sign and underscore.
A JavaScript variable name follows a camelCase convention.
A JavaScript variable name should not have space between word

```
// Declare a variable called myVariable and assign it the value 'hello'
let myVariable = 'hello';

// Change the value of myVariable to 'world'
myVariable = 'world';

// Declare a constant called myConstant and assign it the value 42
const myConstant = 42;

```

Variables can store different types of data, including strings, numbers, booleans, and objects.

```
// Declare a variable called myString and assign it the value 'hello'
let myString = 'hello';

// Declare a variable called myNumber and assign it the value 42
let myNumber = 42;

// Declare a variable called myBoolean and assign it the value true
let myBoolean = true;

// Declare a variable called myObject and assign it an object with two properties
let myObject = {
  property1: 'value1',
  property2: 'value2'
};

```

Variables can also be used to store the result of an expression or function.

```
// Declare a variable called mySum and assign it the value of 2 + 2
let mySum = 2 + 2;

// Declare a function called myFunction that returns the sum of two numbers
function myFunction(a, b) {
  return a + b;
}

// Call myFunction and store the result in a variable called myResult
let myResult = myFunction(2, 3);

```

**Operators**
Assignment operators
An equal sign in JavaScript is an assignment operator. It uses to assign a variable

### Arithmetic Operators

Arithmetic operators are mathematical operators.

- Addition(+): a + b
- Subtraction(-): a - b
- Multiplication(*): a * b
- Division(/): a / b
- Modulus(%): a % b
- Exponential(**): a ** b

### Comparison Operators

In programming we compare values, we use comparison operators to compare two values. We check if a value is greater or less or equal to other value.

### Increment Operator

In JavaScript we use the increment operator to increase a value stored in a variable. The increment could be pre or post increment. Let us see each of them:

1. Pre-increment

```
let count = 0
console.log(++count)        // 1
console.log(count)          // 1
```

1. Post-increment

```
let count = 0
console.log(count++)        // 0
console.log(count)          // 1
```

We use most of the time post-increment. At least you should remember how to use post-increment operator.

**Conditionals**

Conditionals are used to control the flow of a program. They allow us to execute different pieces of code based on whether a particular condition is true or false. In JavaScript, we use the following conditional statements:

- **if statement** - executes a block of code if a specified condition is true
- **else statement** - executes a block of code if the same condition is false
- **else if statement** - allows you to specify a new condition to test if the previous condition is false
- **switch statement** - allows you to specify multiple alternatives based on a single value

**if statement**

The if statement is used to execute a block of code if a specified condition is true. The syntax for the if statement is as follows:

```
if (condition) {
  // code to be executed if the condition is true
}

```

**else statement**

The else statement is used to execute a block of code if the same condition is false. The syntax for the else statement is as follows:

```
if (condition) {
  // code to be executed if the condition is true
} else {
  // code to be executed if the condition is false
}

```

**else if statement**

The else if statement allows you to specify a new condition to test if the previous condition is false. The syntax for the else if statement is as follows:

```
if (condition1) {
  // code to be executed if condition1 is true
} else if (condition2) {
  // code to be executed if condition2 is true and condition1 is false
} else {
  // code to be executed if both condition1 and condition2 are false
}

```

**switch statement**

The switch statement allows you to specify multiple alternatives based on a single value. The syntax for the switch statement is as follows:

switch (expression) {

  case value1:
    // code to be executed if expression matches value1
    break;
  case value2:
    // code to be executed if expression matches value2
    break;
  default:
    // code to be executed if expression doesn't match either value1 or value2
    break;
}

**Ternary Operators**

Another way to write conditionals is using ternary operators. We have covered this in other sections, but we should also mention it here.

let isRaining = true
isRaining
  ? console.log('You need a rain coat.')
  : console.log('No need for a rain coat.')

**Arrays**
In contrast to variables, an array can store multiple values. Each value in an array has an index, and each index has a reference in a memory address. Each value can be accessed by using their indexes. The index of an array starts from zero, and the index of the last element is less by one from the length of the array.

An array is a collection of different data types which are ordered and changeable(modifiable). An array allows storing duplicate elements and different data types. An array can be empty, or it may have different data type values.

[Declaration](https://javascript.info/array#declaration)

There are two syntaxes for creating an empty array:

`let arr = new Array();
let arr = [];`

Almost all the time, the second syntax is used. We can supply initial elements in the brackets:

`let fruits = ["Apple", "Orange", "Plum"];`

Array elements are numbered, starting with zero.

We can get an element by its number in square brackets:

`let fruits = ["Apple", "Orange", "Plum"];

alert( fruits[0] ); // Apple
alert( fruits[1] ); // Orange
alert( fruits[2] ); // Plum`

We can replace an element:

`fruits[2] = 'Pear'; // now ["Apple", "Orange", "Pear"]`

…Or add a new one to the array:

`fruits[3] = 'Lemon'; // now ["Apple", "Orange", "Pear", "Lemon"]`

The total count of the elements in the array is its `length`:

`let fruits = ["Apple", "Orange", "Plum"];

alert( fruits.length ); // 3`

We can also use `alert` to show the whole array.

`let fruits = ["Apple", "Orange", "Plum"];

alert( fruits ); // Apple,Orange,Plum`

An array can store elements of any type.

For instance:

`// mix of values
let arr = [ 'Apple', { name: 'John' }, true, function() { alert('hello'); } ];

// get the object at index 1 and then show its name
alert( arr[1].name ); // John

// get the function at index 3 and run it
arr[3](); // hello`

### Converting array to string

to String: Converts array to string

`const numbers = [1, 2, 3, 4, 5]
console.log(numbers.toString()) // 1,2,3,4,5

const names = ['Asabeneh', 'Mathias', 'Elias', 'Brook']
console.log(names.toString()) // Asabeneh,Mathias,Elias,Brook`

**Trailing comma**

An array, just like an object, may end with a comma:

`let fruits = [
  "Apple",
  "Orange",
  "Plum"*,*];`

The “trailing comma” style makes it easier to insert/remove items, because all lines become alike

## Loops

Loops are a fundamental concept in programming that allow you to execute a block of code repeatedly.

Most of the activities we do in life are full of repetitions. Imagine if I ask you to print out from 0 to 100 using console.log(). To implement this simple task it may take you 2 to 5 minutes, such kind of tedious and repetitive task can be carried out using loop .they  have three  type of loops :

**for loop**

Here is an example of a **for loop** in JavaScript that prints the numbers from 1 to 5:

```
for (let i = 1; i <= 5; i++) {
    console.log(i);
}

```

This loop uses the `for` keyword to create a loop with three expressions: an initialization expression (`let i = 1`), a condition expression (`i <= 5`), and an update expression (`i++`). The loop iterates over each number from 1 to 5 and logs it to the console ¹.

```
const countries = ['Finland', 'Sweden', 'Denmark', 'Norway', 'Iceland']
const newArr = []
for(let i = 0; i < countries.length; i++){
  newArr.push(countries[i].toUpperCase())
}

```

Creating a new array based on the existing array

`const numbers = [1, 2, 3, 4, 5]
const newArr = []
let sum = 0
for(let i = 0; i < numbers.length; i++){
  newArr.push( numbers[i] ** 2)

}

console.log(newArr)  // [1, 4, 9, 16, 25]`

**while loop** 

in JavaScript that prints the numbers from 1 to 5:

`let i = 1;

while (i <= 5) {
    console.log(i);
    i++;
}`

This loop uses the **`while`** keyword to create a loop with a single condition expression (**`i <= 5`**). The loop iterates over each number from 1 to 5 and logs it to the console .

**do-while loop** 

in JavaScript that prints the numbers from 1 to 5:

`let i = 1;

do {
    console.log(i);
    i++;
} while (i <= 5);`
Copy

This loop uses the **`do-while`** keywords to create a loop with a single condition expression (**`i <= 5`**). The loop iterates over each number from 1 to 5 and logs it to the console.

`break`

The **`break`** statement is used to exit a loop or switch statement. When the **`break`** statement is encountered inside a loop, the loop is immediately terminated and the program control resumes at the next statement following the loop

```
for(let i = 0; i <= 5; i++){
  if(i == 3){
    break
  }
  console.log(i)
}

// 0 1 2
```

### continue

We use the keyword *continue* to skip a certain iterations.

`for(let i = 0; i <= 5; i++){
  if(i == 3){
    continue
  }
  console.log(i)
}

// 0 1 2 4 5`

**Functions**

A function is a reusable block of code or programming statements designed to perform a certain task. A function is declared by a function key word followed by a name, followed by parentheses (). A parentheses can take a parameter. If a function take a parameter it will be called with argument. A function can also take a default parameter. To store a data to a function, a function has to return certain data types. To get the value we call or invoke a function. Function makes code:

other definition about function in java script : A function in JavaScript is a block of code designed to perform a specific task. A function is executed when it is called or invoked. 

A function can be declared or created in couple of ways:

- *Declaration function*
- *Expression function*
- *Anonymous function*
- *Arrow function*

**Function Declaration**

A **function declaration** in JavaScript is a way to define a function using the `function` keyword followed by the function name, a list of parameters (that might be empty), and a statement block surrounded by curly braces ¹.

Here is an example of a function declaration in JavaScript:

```
function greet(name) {
    console.log(`Hello, ${name}!`);
}

greet("John");

```

This function takes a single parameter `name` and logs a greeting message to the console. When the function is called with the argument `"John"`, it logs the message `"Hello, John!"` to the console.

### Function returning value

Function can also return values, if a function does not return values the value of the function is undefined. Let us write the above functions with return. From now on, we return value to a function instead of printing it.

`function printFullName (){
      let firstName = 'Asabeneh'
      let lastName = 'Yetayeh'
      let space = ' '
      let fullName = firstName + space + lastName
      return fullName
}
console.log(printFullName())`

A function with a parameter is a function that takes one or more input values, called arguments or parameters, and performs a specific task based on those values .

Here is an example of a function with a parameter in JavaScript:

```
function greet(name) {
    console.log(`Hello, ${name}!`);
}

greet("John");

```

This function takes a single parameter `name` and logs a greeting message to the console. When the function is called with the argument `"John"`, it logs the message `"Hello, John!"` to the console.

```
// function with one parameter
function functionName(parm1) {
  //code goes her
}
functionName(parm1) // during calling or invoking one argument needed

function areaOfCircle(r) {
  let area = Math.PI * r * r
  return area
}

console.log(areaOfCircle(10)) // should be called with one argument

function square(number) {
  return number * number
}

console.log(square(10))
```

### Function with unlimited number of parameters

Sometimes we do not know how many arguments the user going to pass. Therefore, we should know how to write a function which can take unlimited number of arguments. The way we do it has a significant difference between a function declaration(regular function) and arrow function. 

### Unlimited number of parameters in regular function

A function declaration provides a function scoped arguments array like object. Any thing we passed as argument in the function can be accessed from arguments object inside the functions

```
function sumAllNums() {
 console.log(arguments)
}

sumAllNums(1, 2, 3, 4)
// Arguments(4) [1, 2, 3, 4, callee: ƒ, Symbol(Symbol.iterator)

**Unlimited number of parameters in arrow function**

Arrow function does not have the function scoped arguments object. To implement a function which takes unlimited number of arguments in an arrow function we use spread operator followed by any parameter name. Any thing we passed as argument in the function can be accessed as array in the arrow function. Let us see an example

// Let us access the arguments object

const sumAllNums = (...args) => {
 // console.log(arguments), arguments object not found in arrow function
 // instead we use a parameter followed by spread operator (...)
 console.log(args)
}

sumAllNums(1, 2, 3, 4)
// [1, 2, 3, 4]
// function declaration

const sumAllNums = (...args) => {
  let sum = 0
  for (const element of args) {
    sum += element
  }
  return sum
}

console.log(sumAllNums(1, 2, 3, 4)) // 10
console.log(sumAllNums(10, 20, 13, 40, 10))  // 93
console.log(sumAllNums(15, 20, 30, 25, 10, 33, 40))  // 173
```

**Function with default parameters**

A function with default parameters is a function that has one or more parameters with default values. If the function is called without providing a value for a parameter with a default value, the default value is used instead,

```
function greetings(name = 'Peter') {
  let message = `${name}, welcome to 30 Days Of JavaScript!`
  return message
}

console.log(greetings())
console.log(greetings('Asabeneh'))
```

`function generateFullName(firstName = 'Asabeneh', lastName = 'Yetayeh') {
  let space = ' '
  let fullName = firstName + space + lastName
  return fullName
}

console.log(generateFullName())
console.log(generateFullName('David', 'Smith'))`

## Scope

Variable is the fundamental part in programming. We declare variable to store different data types. To declare a variable we use the key word *var*, *let* and *const*. A variable can be declared at different scope. In this section, we will see the scope variables, scope of variables when we use var or let. Variables scopes can be:

- Global
- Local

**Global scope**

The global scope in JavaScript refers to the context in which variables and functions are defined outside of any function or block. Variables and functions defined in the global scope are accessible from anywhere in the code.

Here is an example of a variable defined in the global scope in JavaScript:

```
let message = "Hello, world!";

function greet() {
    console.log(message);
}

greet(); // logs "Hello, world!"

```

In this example, the variable `message` is defined in the global scope and is accessible from anywhere in the code.

### Local scope

A variable declared as local can be accessed only in certain block code.

- Block Scope
- Function Scope

`//scope.js
let a = 'JavaScript' // is a global scope it will be found anywhere in this file
let b = 10 // is a global scope it will be found anywhere in this file
// Function scope
function letsLearnScope() {
  console.log(a, b) // JavaScript 10, accessible
  let value = false
// block scope
  if (true) {
    // we can access from the function and outside the function but 
    // variables declared inside the if will not be accessed outside the if block
    let a = 'Python'
    let b = 20
    let c = 30
    let d = 40
    value = !value
    console.log(a, b, c, value) // Python 20 30 true
  }
  // we can not access c because c's scope is only the if block
  console.log(a, b, value) // JavaScript 10 true
}
letsLearnScope()
console.log(a, b) // JavaScript 10, accessible`

**Object**

 an object is a standalone entity that can contain properties and methods ¹. An object's properties are key-value pairs that can be of any data type, including other objects. A property's value can also be a function, in which case it is called a method ².

Here is an example of how to create an object in JavaScript using the object literal syntax:

```
const person = {
  firstName: "John",
  lastName: "Doe",
  age: 30,
  eyeColor: "blue",
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
};

```

In this example, `person` is an object that has five properties (`firstName`, `lastName`, `age`, `eyeColor`, and `fullName`). The `fullName` property is a method that returns the full name of the person.

### Setting new key for an object

An object is a mutable data structure and we can modify the content of an object after it gets created.

Setting a new keys in an object

`const person = {
  firstName: 'Asabeneh',
  lastName: 'Yetayeh',
  age: 250,
  country: 'Finland',
  city: 'Helsinki',
  skills: [
    'HTML',
    'CSS',
    'JavaScript',
    'React',
    'Node',
    'MongoDB',
    'Python',
    'D3.js'
  ],
  getFullName: function() {
    return `${this.firstName} ${this.lastName}`
  }
}
person.nationality = 'Ethiopian'
person.country = 'Finland'
person.title = 'teacher'
person.skills.push('Meteor')
person.skills.push('SasS')
person.isMarried = true

person.getPersonInfo = function() {
  let skillsWithoutLastSkill = this.skills
    .splice(0, this.skills.length - 1)
    .join(', ')
  let lastSkill = this.skills.splice(this.skills.length - 1)[0]

  let skills = `${skillsWithoutLastSkill}, and ${lastSkill}`
  let fullName = this.getFullName()
  let statement = `${fullName} is a ${this.title}.\nHe lives in ${this.country}.\nHe teaches ${skills}.`
  return statement
}
console.log(person)
console.log(person.getPersonInfo())`

**Object Methods**

In JavaScript, an object’s methods are functions that are stored as properties of the object . Here is an example of how to create an object with a method in JavaScript

### ****

```
const person = {
  firstName: 'Asabeneh',
  age: 250,
  country: 'Finland',
  city:'Helsinki',
  skills: ['HTML', 'CSS', 'JS'],
  title: 'teacher',
  address: {
    street: 'Heitamienkatu 16',
    pobox: 2002,
    city: 'Helsinki'
  },
  getPersonInfo: function() {
    return `I am ${this.firstName} and I live in ${this.city}, ${this.country}. I am ${this.age}.`
  }
}

//Object methods: Object.assign, Object.keys, Object.values, Object.entries
//hasOwnProperty

const copyPerson = Object.assign({}, person)
console.log(copyPerson)
```

### Getting object keys using Object.keys()

*Object.keys*: To get the keys or properties of an object as an array

```
const keys = Object.keys(copyPerson)
console.log(keys) //['firstName', 'age', 'country','city', 'skills','title', 'address', 'getPersonInfo']
const address = Object.keys(copyPerson.address)
console.log(address) //['street', 'pobox', 'city']
```

### Getting object values using Object.values()

*Object.values*:To get values of an object as an array

```
const values = Object.values(copyPerson)
console.log(values)
```

### Getting object keys and values using Object.entries()

*Object.entries*:To get the keys and values in an array

```
const entries = Object.entries(copyPerson)
console.log(entries)
```

### Checking properties using hasOwnProperty()

*hasOwnProperty*: To check if a specific key or property exist in an object

`console.log(copyPerson.hasOwnProperty('name'))
console.log(copyPerson.hasOwnProperty('score'))`