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

Hello, World!

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
# How to run Python code

* Interactive Mode 
* Script Mode 

-

# Interactive Mode 

Manually type and execute code directly in the Python Interpreter.

-

# Interactive Mode Demo

-

# Script Mode
Execute a script file which contains python code (by convention python files have a .py extention).

-

# Script Mode Demo

-
-

# Arithmetic operators

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

```python
>>> 1 + 1
2
>>> 40 + 2
42
```
![computer](img/hgttg_computer.jpg)

-

## Subtraction 

```python
>>> 1 - 1
0
>>> 43 - 1
42
```

-

## Multiplication

```python
>>> 7 * 7
49
>>> 21 * 2
42
```

-

## Division

```python
>>> 1 / 1
1.0
>>> 84 / 2
42.0
```

-

## Modulo (Remainder)

```python
>>> 2 % 2
0
>>> 3 % 2
1
```

-

## Exponentiation

```python
>>> 2 ** 2
4
>>> 3 ** 3
27
```

-

# ARITHMETIC OPERATORS DEMO

-
-

# Values & Types 
## Important Terms

+ **value**: One of the basic units of data, like a number or string, that a program manipulates.  
+ **type**: A category of values.

-

# Values & Types
## Examples

| Type    | Value         | Description |
| ------- | ------------- | --------------------- |
| bool    | True or False | Boolean               | 
| int     | 1             | Integer               |
| float   | 42.0          | Floating-point number |
| str     | Hello Python  | String                |

-

# Values & Types 
## The type function

```
>>>type(True)
<class 'bool'>

>>>type(1)
<class 'int'>

>>>type(42.0)
<class 'float'>

>>>type('Hello, Python!')
<class 'str'>

>>>type('42.0')
<class 'str'>

```

-

# Values & Types 
## Link to More Information 

[Data Model Docs](https://docs.python.org/3/reference/datamodel.html#)

![Moar](img/types-moar.jpg)

-
-

# Assignment statements

+ **variable** is a name that refers to a value.
+ **assignment** is statement that assigns a value to a variable.

```python
a = 35
greeting = 'Oi'
pi = 3.1415926535897932
```

-

# type function revisited

```python
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

# Variable Names
* Can be as long as you like.
* Can contain letters and numbers, but can't begin with a number.
* Can contain uppercase letters but by convention only lowercase letters are used.
* The underscore character can apper in a name. It is often used in names with multiple words.
* Keywords cannot be used as variable names.  
[List of Keywords](https://docs.python.org/3/reference/lexical_analysis.html#keywords)

![Keywords](img/python-keywords.png)
-

# ASSIGNMENT STATEMENTS DEMO

-

# Expressions and statements 

+ **expression** is a combination of values, variables, and operators. A value all by itself is
considered an expression, and so is a variable.

```
>>>42
42
>>>a
35
>>>a + 42
77
```

+ **statement** is a unit of code that has an effect, like creating a variable or displaying a value.

```
>>> a = 35
>>>print(a)
```

-

# Order of Operations

* For mathematical operators, Python follows mathematical convention. 
* The acronym PEMDAS is a useful way to remember the rules:
  1. Parentheses,
  2. Exponentiation
  3. Multiplication and Division
  4. Addition and Subtraction
  Operators with the same precedence are evaluated from left to right.

-
-

# String Operations

-
-

# Comments
