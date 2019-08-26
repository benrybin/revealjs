# Introduction to Python

![Python](img/python-logo.png)

-

## Why Python

| Benefit                              | Resource                                                             |
| ------------------------------------ | -------------------------------------------------------------------- |
| Friendly & Easy to Learn             | [Think Python Ebook](https://greenteapress.com/wp/think-python-2e/)  |
| Thoroughly documented                | [Python Docs](https://www.python.org/doc/)                           | 
| Open source                          | [Wiki Entry](https://en.wikipedia.org/wiki/Open_source)              |
| Broad range of applications          | [Applications](https://www.python.org/about/apps/)                   |
| Fully featured standard library      | [Python Standard Library Docs](https://docs.python.org/3/)           |
| Thousands of third-party modules     | [Python Package Index (PyPI)](https://pypi.org/)                     |

-

# The Zen Of Python

Don't worry about this now. One day it will make sense. 

[The Zen of Python](https://www.python.org/dev/peps/pep-0020/)

-
-

# Hello, World!

![Show me the code](img/show-me-the-code.jpg)

-

## Java Hello World

```java
  class HelloJava {
    public static void main(String[] args) {
      System.out.println("Hello Java");
    }
  }
```

-

## Python Hello World

```python
  print("Hello Python")
```

-
-

# Getting Started

-

## How To Run Python Code

* Interactive Mode 
* Script Mode 

-

## Interactive Mode 

Manually type and execute code directly in the Python Interpreter.

-

## Interactive Mode Demo

-

## Script Mode
Execute a script file which contains python code (by convention python files have a .py extention).

-

## Script Mode Demo

-
-

# Arithmetic

![computer](img/hgttg_computer.jpg)

-

## Operations

| Operation          | Symbol  |
| ------------------ | ------- |
| Addition           | +       |
| Subtraction        | -       |
| Multiplication     | *       | 
| Division           | /       |
| Floor Division     | //      |
| Modulo (Remainder) | %       |
| Exponentiation     | **      |

-

## Addition

```none
>>> 1 + 1
2

>>> 40 + 2
42
```

-

## Subtraction 

```none
>>> 1 - 1
0

>>> 43 - 1
42
```

-

## Multiplication

```none
>>> 7 * 7
49

>>> 21 * 2
42
```

-

## Division

```none
>>> 1 / 1
1.0

>>> 84 / 2
42.0
```

-

## Floor Division

The floor division operator, //, divides two numbers and rounds down to an integer.

```none
>>> minutes = 105
>>> hours = minutes // 60
>>> hours
1
```

-

## Special Note About Python 2
The division operator, /, performs floor division if both operands are integers, 
and floating-point division if either operand is a float.

-

## Modulo (Remainder)

The modulus operator divides two numbers and returns the remainder.

```none
>>> 2 % 2
0

>>> 3 % 2
1
```

-

## Exponentiation

```none
>>> 2 ** 2
4

>>> 3 ** 3
27
```

-

## ARITHMETIC OPERATORS DEMO

-
-

# Values & Types 

-

## Important Terms

+ **value**: One of the basic units of data, like a number or string, that a program manipulates.  
+ **type**: A category of values.

-

## Examples

| Type    | Value         | Description |
| ------- | ------------- | --------------------- |
| bool    | True or False | Boolean               | 
| int     | 1             | Integer               |
| float   | 42.0          | Floating-point number |
| str     | Hello Python  | String                |

-

## The type Function

```none
>>> type(True)
<class 'bool'>

>>> type(1)
<class 'int'>

>>> type(42.0)
<class 'float'>

>>> type('Hello, Python!')
<class 'str'>

>>> type('42.0')
<class 'str'>

```

-

## More Information 

[Data Model Docs](https://docs.python.org/3/reference/datamodel.html#)

![Moar](img/types-moar.jpg)

-
-

# Assignment Statements

-

## Important Terms

A **variable** is a name that refers to a value.  
An **assignment** is statement that assigns a value to a variable.

```python
a = 35
greeting = 'Oi'
pi = 3.1415926535897932
```

-

## type Function Revisited

```none
>>> a = 35
>>> type(a)
<class 'int'>

>>> greeting = 'Oi'
>>> type(greeting)
<class 'str'>

>>> pi = 3.1415926535897932
>>> type(pi)
<class 'float'>
```

-

## Variable Names

* Can be as long as you like.
* Can contain letters and numbers, but can't begin with a number.
* Can contain uppercase letters but by convention only lowercase letters are used.
* The underscore character can apper in a name. It is often used in names with multiple words.
* Keywords cannot be used as variable names.  

-

## Keywords

[List of Keywords](https://docs.python.org/3/reference/lexical_analysis.html#keywords)

![Keywords](img/python-keywords.png)

-

## ASSIGNMENT STATEMENTS DEMO

-
-

# Expressions And Statements 

-

## Experssion

An **expression** is a combination of values, variables, and operators.  
A value all by itself is considered an expression, and so is a variable.

```none
>>> 42
42

>>> a
35

>>> a + 42
77
```

-

## Statement

A **statement** is a unit of code that has an effect, like creating a variable or displaying a value.

```none
>>> a = 35
>>> print(a)
```

-
-

# Order Of Operations

-

* For mathematical operators, Python follows mathematical convention. 
* The acronym PEMDAS is a useful way to remember the rules:
  1. Parentheses
  2. Exponentiation
  3. Multiplication and Division
  4. Addition and Subtraction
  Operators with the same precedence are evaluated from left to right.

-
-

# String Operations

-

| Operator | Operation            |
| -------- | -------------------- |
| +        | String Concatenation |
| *        | Repetition           |

```none
>>> 'eggs '+ 'and ' + 'ham'
'eggs and ham'

>>> 'Spam'*3
'SpamSpamSpam'
```

-
-

# Comments

-

## Single Line Comments

```python
# The airspeed velocity of an unladen swallow in meters per second
velocity = 11
```

```python
migratory = False # African swallows are non-migratory.
```

-

## Multi Line Comments

```
"""
In order to maintain air-speed velocity, 
a swallow needs to beat its wings
forty-three times every second
"""
beats_per_second = 43
```

-
-

# BREAK & EXERCISES 

-
-

# Functions

-

## What Is A Function? 

* A function is a named sequence of statements that performs a computation.
* When you define a function, you specify the name and the sequence of statements.
* Later, you can “call” the function by name.

-

## Why Use Functions? 

*  Makes a program smaller by eliminating repetitive code.
*  Makes a program easier to read and debug.
*  Makes code reusable.

-

## Defining a function

```python
def best_ice_cream():
    print("Mint chocolate chip.")
```

* def is a keyword that indicates that this is a function definition.
* The name of the function is best_ice_cream.
* The empty parentheses after the name indicate that this function doesn’t take any arguments.

-

## Defining a function Pt 2 

* The first line of the function definition is called the header.
* The rest is called the body.
* The header has to end with a colon and the body has to be indented.
* By convention, indentation is always four spaces.

-

## Function Type 

Defining a function creates a function object, which has type function:

```none
>>> type(best_ice_cream)
<type 'function'>

>>> print(best_ice_cream)
<function best_ice_cream at 0x1073652a8>
```

-


## Function Name Rules

The rules for function names are the same as for variable names.

* Letters, numbers and underscore are legal.
* The first character can’t be a number. 
* You can’t use a keyword as the name of a function.
* You should avoid having a variable and a function with the same name.

-

## Function Calls

```none
>>> def best_ice_cream():
...     print("Mint chocolate chip.")
... 
>>> best_ice_cream()
Mint chocolate chip.
```

The function definition has to run before the function gets called.

-

## Arguments

* Some functions require one or more arguments. 
* math.power takes two, the base and the exponent.

```none
>>> import math
>>> result = math.pow(2, 3)
>>> print(result)
8.0
```

-

## Parameters 

Inside the function, arguments are assigned to variables called parameters.

```none
>>> def favorite_ice_cream(fav_ice_cream):
...     print("Your favorite ice cream is " + fav_ice_cream)
... 
>>> favorite_ice_cream("mint chocolate chip")
Your favorite ice cream is mint chocolate chip
```

-

## Functions Can Call Functions

```none
>>> def say_hello():
...     print("Hello")
... 
>>> def say_hello_two_times():
...     say_hello()
...     say_hello()
... 
>>> say_hello()
Hello
>>> 
>>> say_hello_two_times()
Hello
Hello
```

-

## Variable Scopes 

* Variables created inside of a function are local.

```
>>> name = 'Alice'
>>> def print_name():
...     name = 'Bob'
...     print(name)
... 
>>> def print_other_name():
...     name = 'John'
...     print(name)
... 
>>> print_name()
Bob 
>>> print_other_name()
John
>>> print(name)
Alice
```

-

# docstring

A docstring is a string at the beginning of a function that explains the interface.

```python
def add(x, y):
    """
    Adds two integers and returns their result.
    x and y are integers.
    """
    return x + y

result = add(1, 2)
print(result)
```

-

# Built-in Functions

[Built-in Function Docs](https://docs.python.org/3/library/functions.html)

![Moar](img/functions-moar.jpg)

-
-

# BREAK & EXERCISES 

-
-

# Relational Operators

-

## What is it? 
One of the operators that compares its operands.

| Operator | Description              | Example |
| -------- | ------------------------ | ------- |
| ==       | is equal to              | x == y  |
| !=       | is not equal to          | x != y  |
| >        | is greater than          | x > y   |
| <        | is less than             | x < y   |
| >=       | greater than or equal to | x >= y  |
| <=       | less than or equal to    | x <= y  |

-
-

# Boolean Expressions

## What is it?
A boolean expression is an expression that is either true or false.

-
-

# Logical Operators

-

## What is it?
One of the operators that combines boolean expressions

-
-

# Conditionals

-
-

# Recursion

-
-
