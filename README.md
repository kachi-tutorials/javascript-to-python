# Learning Python as a Javascript developer

As a coder, you should always be looking to expand your knowledge. The best way to do this is by learning different coding languages and frameworks. I myself am a **`Javascript`** and **`Python`** fullstack developer and like most self-taught developers, I started by learning **`HTML`**, **`CSS`** and **`Javascript`** first. Eventually I learned **`Python`** and found it very useful. Python is great for handling backend data and creating simple scripts like web-scrapers.

If you're nervous about learning **`Python`**, remember that **`Python`** is a high level programming language. This means it is around the same level of difficulty to learn as **`Javascript`**. I would even argue it is easier to learn than javascript, and the transition from **`Javascript`** to **`python`** much smoother than the other way round.

In this tutorial, I'll outline the main differences between the two coding languages.

## Set Up

Firstly, make sure [**`python`**](https://www.python.org/downloads/) is installed on your machine before you start.

You can check this by running this command in your terminal:

```bash
python3 --version
```

Alternatively, you can use a [**`sandbox`**](https://pythonsandbox.com/) to test **`python`** code.

## Methods

The methods used in **`python`** and **`javascript`** are not the same.

Here are some examples of this:

In **`javascript`**:

```javascript
"Hello World".length; // Length of a string
arr.push("new string"); // Add new item to end of array
arr.sort((a, b) => a - b); // Sort an array
```

In **`python`**:

```python
len("Hello world") # Length of a string
arr.append("new string") # Add new item to end of list
arr.sort() # Sort a list
```

As you can see, the differences are not huge and you of course do not need to remember all of them. Here are links to some of the ones you'll need to know.

| Type       | Page                                                                 |
| ---------- | -------------------------------------------------------------------- |
| Strings    | [Methods](https://www.w3schools.com/python/python_ref_string.asp)    |
| List/Array | [Methods](https://www.w3schools.com/python/python_ref_list.asp)      |
| Functions  | [Keywords](https://www.w3schools.com/python/python_ref_keywords.asp) |

## Output

When you want to log something in the terminal or browser. Just change **`console.log`** to **`print`**!

In **`javascript`**:

```javascript
console.log("hello world");
```

In **`python`**:

```python
print("hello world")
```

## Comments

When leaving a comment or commenting something out change **`//`** to **`#`**:

In **`javascript`**:

```javascript
// javascript comment

/* multiline
javascript
comment */
```

In **`python`**:

```python
# Python comment

# Multi
# Line
# Comment
```

## Variables

There are a couple difference between **`Javascript`** and **`Python`** variables.

- **`Javascript`** use **camel casing** and **`Python`** use **underscores**.
- **`const`**, **`let`** and **`var`** for **`javascript`**. Cases for **`python`**.

In **`Javascript`**:

```javascript
var myExample = "hello world"; // global variable
let myExample = "hello world"; // scope variable
const myExample = "hello world"; // unchangeable variable (scope)
```

In **`Python`**:

```python
my_example = "hello world" # basic variable
MY_EXAMPLE = "hello world" # Red flag to not change
```

**Note**: In **`python`**, every variable is mutable. There is no real way to prevent but when writing code, you changing the case of the variable can signal to other programmers that the variable should not be changed.

## List and Arrays

There are a couple differences between **`Javascript`** and **`Python`** arrays.

- **`Arrays`** in **`Javascript`** are called **`lists`** in **`Python`**.
- **`Javascript`** use **camel casing** and **`Python`** use **underscores**.
- **`const`**, **`let`** and **`var`** are used in **`javascript`**. Cases are used in **`python`**.

In **`Javascript`**:

```javascript
const myList = [4, 5, 6];
```

In **`Python`**:

```python
my_list = [1, 3, 5]
```

## Functions

**`Javascript`** uses curly braces `{}` and **`function`** (or an _**`arrow function`**_):

```javascript
function foo(str) {
  console.log(str);
}

const foo = (str) => console.log(str);
```

**`Python`** uses **`def`** followed by a colon **`:`** for their functions:

```python
def foo(str):
    print(str)
```

## If Statements

**`Javascript`** uses **`curly braces`** `{}` and **`parenthesis`** `()` for each condition separated by a **`else if`** or **`else`**:

```javascript
if (condition1) {
  console.log("condition 1 met");
} else if (condition2) {
  console.log("condition 2 met");
} else {
  console.log("else condition");
}
```

**`Python`** just uses colons **`:`** after each condition and an indented code block. Statements are separated by a **`elif`** and **`else`**:

```python
if condition_one:
  print("condition 1 met")
elif condition_two:
  print("condition 2 met")
else:
  print('else condition')
```

### Logical Operators

When declaring conditions, we use the following:

| Javascript     | Python              |
| -------------- | ------------------- |
| &#124;&#124;   | **`or`**            |
| **&&**         | **`and`**           |
| **!condition** | **`not condition`** |

In **`Javascript`**:

```javascript
if (condition1 || condition2) // or
if (condition1 && condition2) // and
if (!condition) // is not
```

In **`Python`**:

```python
if condition1 or condition2 # ||
if condition1 and condition2 # &&
if not condition ## !condition
```

## For Loop

In **`Javascript`**, you are required to declare a variable and increment it using the for loop.

In **`Python`** we replace that logic with **`in range(x)`**.

In **`Javascript`:**

```javascript
for (var i = 0; i < 5; i++) {
  console.log(i);
}
```

in **`Python`:**

```python
for i in range(5):
    print(i)
```

### If you want to access an object or item in an Array:

In **Javascript:**

```javascript
for (var i = 0; i < arr.length; i++) {
  console.log(arr[i]);
}
```

In **Python:**

```python
for obj in arr:
    print(obj)
```

## Types

**`Primitive data`** types represent the fundamental values that we can work with in a programming language. **`JavaScript`** has 6 types and **`Python`** has 4 types:

- **`JavaScript`** data types: `undefined`, `Boolean`, `String`, `Number`, `BigInt`, and `Symbol`.

- **`Python`** data types: Integers (`int`), Floats (`float`), Booleans (`bool`), and strings (`str`).

To check types in **`javascript`**:

```python
type(instance)
```

To check types in **`python`**:

```javascript
typeof instance;
```

## Imports

Importing files are pretty similar, you just have to swap the order of **`import`** and **`from`**.

In **`Javascript`:**

```javascript
import React from "react";
```

In **`Python`:**

```python
from django.db import models
```

## Classes

**`Javascript`** uses curly braces **`{}`** and **`Python`** uses colons **`:`**.

In **`JavaScript`**, the constructor method is called constructor and it has a parameters list as well.

In **`Python`**, the constructor that initialises the new instance is called **`__init__`**. This method is called automatically when an instance of the class is created to initialise its attributes. It's parameters list defines the values that we have to pass to create the instance. This list starts with self as the first parameter.

### Class format

In **`Javascript`**:

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }
}
```

In **`Python`**:

```python
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age
```

### Assign value to a Class

In **`Javascript`**:

```javascript
this.attribute = value;
```

In **`Python`**:

```python
self.attribute = value
```

### Create Class Instance

In **`Javascript`**:

```javascript
personOne = new Person("John", 18);
```

In **`Python`**:

```python
person_one = Person("John", 18)
```

## Summary

The goal of this tutorial is to show the subtle differences between **`javascript`** and **`python`**. The best way to learn is to rewrite some of your **`javascript`** functions in **`python`**.

If you want to try solve a few problems in python on [**`Code Wars`**](https://www.codewars.com/).

Thanks for reading and Good Luck!
