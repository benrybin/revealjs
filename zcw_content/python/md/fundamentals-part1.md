# Attribution

-

[PSF](https://www.python.org/psf/)  

[Allen Downey / Green Tea Press](https://greenteapress.com/wp/)

-
-

# Introduction to Python

![Python](img/python-logo.png)

-

### What Is It?

"Python is a programming language that lets you work quickly and integrate systems more effectively."

-

### Why Python

| Benefit                              | Resource                                                             |
| -------------------------------- | -------------------------------------------------------------------- |
| Friendly & Easy to Learn         | [Think Python Ebook](https://greenteapress.com/wp/think-python-2e/)  |
| Thoroughly documented            | [Python Docs](https://www.python.org/doc/)                           | 
| Open source                      | [Wiki Entry](https://en.wikipedia.org/wiki/Open_source)              |
| Broad range of applications      | [Applications](https://www.python.org/about/apps/)                   |
| Fully featured standard library  | [Python Standard Library Docs](https://docs.python.org/3/)           |
| Thousands of third-party modules | [Python Package Index (PyPI)](https://pypi.org/)                     |

-

### The Zen Of Python

```none
>>> import this
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!

```

[The Zen of Python](https://www.python.org/dev/peps/pep-0020/)

-
-

# Hello, World!

![Show me the code](img/show-me-the-code.jpg)

-

### Java Hello World

```java
  class HelloJava {
    public static void main(String[] args) {
      System.out.println("Hello Java");
    }
  }
```

-

### Python Hello World

```python
  print("Hello Python")
```

-
-

# Getting Started

-

### How To Run Python Code

* Interactive Mode 
* Script Mode 

-

### Interactive Mode 

Manually type and execute code directly in the Python Interpreter.

-

### Interactive Mode Demo

-

### Script Mode
Execute a script file which contains python code (by convention python files have a .py extention).

-

### Script Mode Demo

-
-

# Arithmetic

![computer](img/hgttg_computer.jpg)

-

### Operations

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

### Addition

```python
1 + 1
# 2

40 + 2
# 42
```

-

### Subtraction 

```python
1 - 1
# 0

43 - 1
# 42
```

-

### Multiplication

```python
7 * 7
# 49

21 * 2
# 42
```

-

### Division

```python
1 / 1
# 1.0

84 / 2
# 42.0
```

-

### Floor Division

The floor division operator, //, divides two numbers and rounds down to an integer.

```python
minutes = 105
hours = minutes // 60
hours
# 1
```

-

### Special Note About Python 2
The division operator, /, performs floor division if both operands are integers, 
and floating-point division if either operand is a float.

-

### Modulo (Remainder)

The modulus operator divides two numbers and returns the remainder.

```python
2 % 2
# 0

3 % 2
# 1
```

-

### Exponentiation

```python
2 ** 2
# 4

3 ** 3
# 27
```

-

### ARITHMETIC OPERATORS DEMO

-
-

# Values & Types 

-

### Important Terms

+ **value**: One of the basic units of data, like a number or string, that a program manipulates.  
+ **type**: A category of values.

-

### Examples

| Type    | Value         | Description |
| ------- | ------------- | --------------------- |
| bool    | True or False | Boolean               | 
| int     | 1             | Integer               |
| float   | 42.0          | Floating-point number |
| str     | Hello Python  | String                |

-

### The type Function

Given an argument, the type function return the type of an object.

```python
type(True)
# <class 'bool'>

type(1)
# <class 'int'>

type(42.0)
# <class 'float'>

type('Hello, Python!')
# <class 'str'>

type('42.0')
# <class 'str'>

type(str)
# <class 'type'>
```

-

### More Information 

[Data Model Docs](https://docs.python.org/3/reference/datamodel.html#)

![Moar](img/types-moar.jpg)

-
-

# Assignment Statements

-

### Important Terms

A **variable** is a name that refers to a value.  
An **assignment** is statement that assigns a value to a variable.

```python
a = 35
greeting = 'Oi'
pi = 3.1415926535897932
```

-

### type Function Revisited

```python
a = 35
type(a)
# <class 'int'>

greeting = 'Oi'
type(greeting)
# <class 'str'>

pi = 3.1415926535897932
type(pi)
# <class 'float'>
```

-

### Variable Names

* Can be as long as you like.
* Can contain letters and numbers, but can't begin with a number.
* Can contain uppercase letters but by convention only lowercase letters are used.
* The underscore character can apper in a name. It is often used in names with multiple words.
* Keywords cannot be used as variable names.  

-

### Keywords

[List of Keywords](https://docs.python.org/3/reference/lexical_analysis.html#keywords)

![Keywords](img/python-keywords.png)

-

### ASSIGNMENT STATEMENTS DEMO

-
-

# Expressions And Statements 

-

### Experssion

An **expression** is a combination of values, variables, and operators.  
A value all by itself is considered an expression, and so is a variable.

```python
42
# 42

a
# 35

a + 42
# 77
```

-

### Statement

A **statement** is a unit of code that has an effect, like creating a variable or displaying a value.

```python
a = 35
print(a)
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

-

### Concatenation

```python
'eggs '+ 'and ' + 'ham'
# 'eggs and ham'

'3' + '3'
# '33'
```

-

### Concatenation Continued

When using the + operator where one of the operands is a string, both operands must be a string.  

```none
>>> 3 + '3'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unsupported operand type(s) for +: 'int' and 'str'
```

You can convert a numeric value to a string with the built-in function str().
```python
str(3) + '3'
# '33'
```

-

### Repetition

```python
'Spam' * 3
# 'SpamSpamSpam'
```

-

### Repetition Continued

When using the * operator where one of the operands is a string, the other operand must be an integer.  

```none
>>> 'Spam' * '3'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: can't multiply sequence by non-int of type 'str'
```

You can convert a string to an integer using the built-in function int().

```python
'Spam' * int('3')
# 'SpamSpamSpam'
```

-
-

# Comments

-

### Options

* Block comments
* Inline comments
* Documentation Strings

-

### Block comments

Block comments generally apply to some (or all) code that follows them, and are indented to the same level as that code. Each line of a block comment starts with a # and a single space.

```python
# The airspeed velocity of an unladen swallow measured in meters per second.
# This is assuming average weather conditions.
velocity = 11
```

-

### Inline Comments

An inline comment is a comment on the same line as a statement. Inline comments should be separated by at least two spaces from the statement. They should start with a # and a single space.

```python
migratory = False  # African swallows are non-migratory.
```

-

### Documentation Strings

This will become relevant in future sections. Just know it exists.

```
"""
In order to maintain air-speed velocity, 
a swallow needs to beat its wings
forty-three times every second
"""
beats_per_second = 43
```

-

### Relevant Links

[PEP 8 Style Guide](https://www.python.org/dev/peps/pep-0008/#comments)  
[PEP 257 Docstring Conventions](https://www.python.org/dev/peps/pep-0257/)


-
-


# The End

![Parrot](img/parrot.jpg)
