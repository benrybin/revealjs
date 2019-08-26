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

## How to run Python code

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
| Modulo (Remainder) | %       |
| Exponentiation     | **      |

-

## Addition

```
>>> 1 + 1
2

>>> 40 + 2
42
```

-

## Subtraction 

```
>>> 1 - 1
0

>>> 43 - 1
42
```

-

## Multiplication

```
>>> 7 * 7
49

>>> 21 * 2
42
```

-

## Division

```
>>> 1 / 1
1.0

>>> 84 / 2
42.0
```

-

## Modulo (Remainder)

```
>>> 2 % 2
0

>>> 3 % 2
1
```

-

## Exponentiation

```
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

## The type function

```
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

## Link to More Information 

[Data Model Docs](https://docs.python.org/3/reference/datamodel.html#)

![Moar](img/types-moar.jpg)

-
-

# Assignment statements

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

## type function revisited

```
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

# Expressions and statements 

-

## Experssion

An **expression** is a combination of values, variables, and operators.  
A value all by itself is considered an expression, and so is a variable.

```
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

```
>>> a = 35
>>> print(a)
```

-
-

# Order of Operations

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

```
>>> 'eggs '+ 'and ' + 'ham'
'eggs and ham'

>>> 'Spam'*3
'SpamSpamSpam'
```

-
-

# Comments

-

## Single line comments

```python
# The airspeed velocity of an unladen swallow in meters per second
velocity = 11
```

```python
migratory = False # African swallows are non-migratory.
```

-

## Multi line comments

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

* A function is a named sequence of statements that performs a computation.
* When you define a function, you specify the name and the sequence of statements.
* Later, you can “call” the function by name.

-

## Function Definition

```python
def best_ice_cream():
    print("Mint chocolate chip.")
```

* def is a keyword that indicates that this is a function definition.
* The name of the function is best_ice_cream.
* The empty parentheses after the name indicate that this function doesn’t take any arguments.

-

## Function Definition Continued 

* The first line of the function definition is called the header.
* The rest is called the body.
* The header has to end with a colon and the body has to be indented.
* By convention, indentation is always four spaces.

-

## Function Name Rules

The rules for function names are the same as for variable names.

* Letters, numbers and underscore are legal.
* The first character can’t be a number. 
* You can’t use a keyword as the name of a function.
* You should avoid having a variable and a function with the same name.

-

## Function Calls

```
>>> def best_ice_cream():
...     print("Mint chocolate chip.")
... 
>>> best_ice_cream()
Mint chocolate chip.
```

-
-



