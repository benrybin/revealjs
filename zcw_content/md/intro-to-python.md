# Introduction to Python

![Python](img/python-logo.png)

-

## Why Python

| Benefit                              | Resource                                                             |
| -------------------------------- | -------------------------------------------------------------------- |
| Friendly & Easy to Learn         | [Think Python Ebook](https://greenteapress.com/wp/think-python-2e/)  |
| Thoroughly documented            | [Python Docs](https://www.python.org/doc/)                           | 
| Open source                      | [Wiki Entry](https://en.wikipedia.org/wiki/Open_source)              |
| Broad range of applications      | [Applications](https://www.python.org/about/apps/)                   |
| Fully featured standard library  | [Python Standard Library Docs](https://docs.python.org/3/)           |
| Thousands of third-party modules | [Python Package Index (PyPI)](https://pypi.org/)                     |

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

Given an argument, the type function return the type of an object.

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

>>> type(str)
<class 'type'>
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

-

## Concatenation

```none
>>> 'eggs '+ 'and ' + 'ham'
'eggs and ham'

>>> '3' + '3'
'33'
```

-

## Concatenation Continued

When using the + operator where one of the operands is a string, both operands must be a string.  

```none
>>> 3 + '3'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unsupported operand type(s) for +: 'int' and 'str'
```

You can convert a numeric value to a string with the built-in function str().
```none
>>> str(3) + '3'
'33'
```

-

## Repetition

```none
>>> 'Spam' * 3
'SpamSpamSpam'
```

-

## Repetition Continued

When using the * operator where one of the operands is a string, the other operand must be an integer.  

```none
>>> 'Spam' * '3'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: can't multiply sequence by non-int of type 'str'
```

You can convert a string to an integer using the built-in function int().

```none
>>> 'Spam' * int('3')
'SpamSpamSpam'
```

-
-

# Comments

-

## Options

* Block comments
* Inline comments
* Documentation Strings

-

## Block comments

Block comments generally apply to some (or all) code that follows them, and are indented to the same level as that code. Each line of a block comment starts with a # and a single space.

```python
# The airspeed velocity of an unladen swallow measured in meters per second.
# This is assuming average weather conditions.
velocity = 11
```

-

## Inline Comments

An inline comment is a comment on the same line as a statement. Inline comments should be separated by at least two spaces from the statement. They should start with a # and a single space.

```python
migratory = False  # African swallows are non-migratory.
```

-

## Documentation Strings

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

## Relevant Links

[PEP 8 Style Guide](https://www.python.org/dev/peps/pep-0008/#comments)  
[PEP 257 Docstring Conventions](https://www.python.org/dev/peps/pep-0257/)

-


![That is all](img/comments-that-is-all.png)

-
-

# BREAK & EXERCISES 

-
-

# Functions

-

## What Is It? 

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

Variables created inside of a function are local.

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

# Boolean Expressions

-

## What Is It?
A boolean expression is an expression that is either true or false.

-

## Examples

```none
>>> 5 == 5
True
>>> 5 == 6
False
>>> 5 > 6
False
>>> 5 < 6
True
```

-
-

# Relational Operators

-

## What Is It? 
One of the operators that compares its operands.

-

## Examples 

| Operator | Description              | Example |
| -------- | ------------------------ | ------- |
| ==       | is equal to              | x == y  |
| !=       | is not equal to          | x != y  |
| >        | is greater than          | x > y   |
| <        | is less than             | x < y   |
| >=       | greater than or equal to | x >= y  |
| <=       | less than or equal to    | x <= y  |

-

## ==

```none
>>> 0 == 0
True
>>> 'a' == 'b'
False
>>> True == True
True
>>> True == False
False

```

-

## !=

```none
>>> 0 != 0
False
>>> 'a' != 'b'
True
>>> True != True
False
>>> True !=  False
True
```

-

## >

```none
>>> 1 > 0
True
>>> 0 > 1
False
>>> 'a' > 'b'
False
>>> 'b' > 'a'
True
>>> True > False
True
>>> False > True
False
```

-

## <

```none
>>> 1 < 0
False
>>> 0 < 1
True
>>> 'a' < 'b'
True
>>> 'b' < 'a'
False
>>> True < False
False
>>> False < True
```

-

## >=

```none
>>> 0 >= 0
True
>>> 0 >= 1
False
>>> 'a' >= 'a'
True
>>> 'a' >= 'b'
False
```

-

## <=

```none
>>> 0 <= 0
True
>>> 0 <= 1
True
>>> 'a' <= 'b'
True
>>> 'b' <= 'a'
False
```

-
-

# Logical Operators

-

## What Is It?
One of the operators that combines boolean expressions.  

There are three logical operators:
* and
* or
* not

-

## and 

Evaluates to True if both conditions are true

```none
>>> x = 5
>>> x > 0 and x < 10
True

>>> x < 0 and x > 3
False
```

-

## or

Evaluates to True if either or both conditions are true

```none
>>> n = 4
>>> n % 2 == 0 or n % 3 == 0
True

>>> n % 5 == 0 or n % 3 == 0
False
```

-

## not

Negates a boolean expression.

```none
>>> not True
False
>>> not False
True
>>> not (1 > 0) 
False
```

-
-

# Compound Statements

-

## Before we begin...

You have already seen compound statements.   
Functions are syntactically compound statements.  
Don't get overwhelmed by the terminology.  

-

## What Is It?

* A compound statement consists of one or more ‘clauses.’
* A clause consists of a header and a ‘suite.’ 
* The clause headers of a particular compound statement are all at the same indentation level.
* Each clause header begins with a uniquely identifying keyword and ends with a colon.
* A suite is a group of statements controlled by a clause. 

-

[Compound Statements](https://docs.python.org/3.7/reference/compound_stmts.html)

-
-

# Conditional Execution

-

## The if Statement

```none
>>> x = 1
>>> if x > 0:
...     print("x is positive")
... 
x is positive
```

-

## Breaking Down The if Statement

* The boolean expression after the if is called the condition.
* If the condition is true, the indented statement runs.
* If the condition is false, nothing happens.
* If statements have the same structure as function definitions. (a header followed by an indented body). These are called compound statements.

-

## The else Clause

```none
>>> x = 7
>>> if x % 2 == 0:
...     print("x is even")
... else:
...     print("x is odd")
... 
x is odd
```

-

## Breaking Down the else Clause

The else clause simply provides an alternative path of execution when the if condition is false.

-

## The elif Clause

```none
>>> x = 10
>>> y = 5
>>> if x < y:
...     print("x is less than y")
... elif x > y:
...     print("x is greater than y")
... else:
...     print("x and y are equal")
... 
x is greater than y
```

-

## Breaking Down The elif Clause:

* elif is an abbreviation for "else if".
* If there is an else clause, it has to be at the end, but there doesn't have to be one.
* Each condition is checked in order. The first one to evaluate to true is run and no other is executed or evaluated.

-

## Nested Conditions

One condition can be nested within another.

-

## Example

```none
>>> x = 10
>>> y = 5
>>> 
>>> if x == y:
...      print("x and y are equal")
... else:
...      if x < y:
...          print("x is less than y")
...      else:
...          print("x is greater than y")
... 
x is greater than y
```

-

## Just Because You Can, Doesn't Mean You Should.

Logical operators often provide a way to simplify nested conditional statements.

-

## Nested Conditional Statement 
```none
>>> x = 5
>>> if 0 < x:
...     if x < 10:
...         print("x is a positive single-digit number.")
... 
x is a positive single-digit number.
```

-

## Simplified Using Logical Operator

```none
>>> if 0 < x and x < 10:
...     print("x is a positive single-digit number.")
... 
x is a positive single-digit number.
```

-
-

# BREAK & EXERCISES 

-
-

# Recursion

-

## What is it? 

It is legal for one function to call another.  
It is also legal for a function to call itself.  

Recursion is the process of calling the function that is currently executing.

-

## Example

```python
def countdown(n):
    if n <= 0: # Base case
        print('Blastoff!') 
    else:
      print(n)
      countdown(n - 1)

countdown(10)
```

-

## Infinite Recursion

If the programmer fails to specify a base case that does not make a recursive call, the program will end in a runtime error.

```python
>>> def endless_inception():
...   endless_inception()
... 
>>> endless_inception()
```

-

## Recursion Error

![RecursionError](img/recursion-error.png)

-

## No Base Case = Bad Time

![No Base Case Bad Time](img/recursion-bad-time.jpg)

-
-

# Keyboard Input

-

Python 3
```python
>>> name = input("What is your name?\n")
What is your name?
Seymour
>>> print(name)
Seymour
```

Python 2
```python
>>> want = raw_input("What do you want\n")
What do you want
feed me
>>> print(want)
'feed me'
```

-
-

# The Range Type

-

## What Is It? 

The range type represents an immutable sequence of numbers and is commonly used for looping a specific number of times in for loops.

-

## Quick Intro

```none
>>> a = range(10)
>>> print(a)
range(0, 10)
>>> type(a)
<class 'range'>
>>> type(range)
<class 'type'>
```

-

## More On Range 

We wil continue to talk about the range type further in the context of sequences and iterations in the upcoming sections.

If you just can't wait, feel free to learn more about it in the docs.  
[Range Type](https://docs.python.org/3/library/stdtypes.html#range)

-
-

# Iteration

-

# What Is It?

Iteration is the ability to run a block of statements repeatedly.

-

# Iteration Kinds

* for 
* while

-

# The for Statement

The for statement is used to iterate over the elements of a sequence (such as a string, tuple or list) or other iterable object.

The for statement has the same structure as function definitions and if statements. (a header followed by an indented body). These are called compound statements.

```python
>>> for i in range(2):
...     print(i)
... 
0
1
```

-

## The while Statement

```
def countdown(n):
    while(n > 0):
        print(n)
        n = n - 1
    print("Blastoff!")

countdown(5)
```

-

## break Statement 

The break statement breaks out of the innermost enclosing for or while loop.

```none
>>> for i in range(10):
...     print(i)
...     if(i == 5):
...        print("I have found what I was looking for.")
...        break
... 
0
1
2
3
4
5
I have found what I was looking for.
```

-

## continue Statement

The continue statement continues with the next iteration of the loop.

```none
>>> for i in range(10):
...     if(i == 5):
...         print("Skipping number 5")
...         continue
...     print(i)
... 
0
1
2
3
4
Skipping number 5
6
7
8
9
```

-

## pass Statement

The pass statement does nothing. It can be used when a statement is required syntactically but the program requires no action.

```none
>>> def master_piece():
...     pass
... 
>>> master_piece()
>>>
```

-

# Control Flow 

[Control Flow Tutorial](https://docs.python.org/3/tutorial/controlflow.html)

![Control Flow More](img/control-flow-moar.jpg)

-
-

# BREAK & EXERCISES 

-
-

# Working With Strings
## Part 1

-

## What Is It?

A string is an immutable sequence of characters.

```none
>>> name = 'Marklar'
>>> print(name)
'Marklar'
```

-

## Index Of A String

An index is an offset from the beginning of a sequence.

```none
>>> name = 'Marklar'
>>> first_letter = name[0]
>>> print(first_letter)
'M'
>>> second_letter = name[1]
>>> print(second_letter)
'a'
```

-

## Expressions Are Allowed 

You can use an expression that contains variables and operators to describe the index.

```none
>>> i = 0
>>> name = "Guido"
>>> print(name[i])
G
>>> print(name[i + 1])
u
```

-

## But...

The value of the index has to be an integer.

```none
>>> print(name[2.2])
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: string indices must be integers, not float
```

-

## The len Built-in Function

[Len](https://docs.python.org/3/library/functions.html#len) is a built-in function that returns the length of an object. When the argument passed to it is a string, it returns the number of characters in the string.

```none
>>> len('one')
3
>>> len('four')
4
```

-

## The Last Item 

```none
>>> name = "Roberto"
>>> print(len(name))
7
>>> last_char = name[len(name) - 1]
>>> print(last_char)
o
```

Or we can use negative indices

```none
>>> print(name[-1])
o
>>> print(name[-2])
t
```

-

## Looping A String 
### While Loop

```none
>>> index = 0
>>> while index < len(word):
...     letter = word[index]
...     print(letter)
...     index = index + 1
... 
p
y
t
h
o
n
```

-

## Looping A String 
### For Loop

```none
>>> word = 'python'
>>> for letter in word:
...     print(letter)
... 
p
y
t
h
o
n
```

-

## String Slices

-

## Srings Are Immutable

-

## String Methods

-

## String comparison

-

## Docs On Strings

[Strings ](https://docs.python.org/3/library/stdtypes.html#text-sequence-type-str)

-
-

# Lists

-
-

# Dictionaries

-
-

# Tuples

-
-