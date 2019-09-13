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

# The Zen Of Python

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

### Hello, World!

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

```none
>>> 1 + 1
2

>>> 40 + 2
42
```

-

### Subtraction 

```none
>>> 1 - 1
0

>>> 43 - 1
42
```

-

### Multiplication

```none
>>> 7 * 7
49

>>> 21 * 2
42
```

-

### Division

```none
>>> 1 / 1
1.0

>>> 84 / 2
42.0
```

-

### Floor Division

The floor division operator, //, divides two numbers and rounds down to an integer.

```none
>>> minutes = 105
>>> hours = minutes // 60
>>> hours
1
```

-

### Special Note About Python 2
The division operator, /, performs floor division if both operands are integers, 
and floating-point division if either operand is a float.

-

### Modulo (Remainder)

The modulus operator divides two numbers and returns the remainder.

```none
>>> 2 % 2
0

>>> 3 % 2
1
```

-

### Exponentiation

```none
>>> 2 ** 2
4

>>> 3 ** 3
27
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

```none
>>> 42
42

>>> a
35

>>> a + 42
77
```

-

### Statement

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

### Concatenation

```none
>>> 'eggs '+ 'and ' + 'ham'
'eggs and ham'

>>> '3' + '3'
'33'
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
```none
>>> str(3) + '3'
'33'
```

-

### Repetition

```none
>>> 'Spam' * 3
'SpamSpamSpam'
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

```none
>>> 'Spam' * int('3')
'SpamSpamSpam'
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


![That is all](img/comments-that-is-all.png)

-
-

# BREAK & EXERCISES 

-
-

# Functions
## Part 1

-

### What Is It? 

* A function is a named sequence of statements that performs a computation.
* When you define a function, you specify the name and the sequence of statements.
* Later, you can “call” the function by name.

-

### Why Use Functions? 

*  Makes a program smaller by eliminating repetitive code.
*  Makes a program easier to read and debug.
*  Makes code reusable.

-

### Defining a function

```python
def best_ice_cream():
    print("Mint chocolate chip.")
```

* def is a keyword that indicates that this is a function definition.
* The name of the function is best_ice_cream.
* The empty parentheses after the name indicate that this function doesn’t take any arguments.

-

### Defining a function Continued

* The first line of the function definition is called the header.
* The rest is called the body.
* The header has to end with a colon and the body has to be indented.
* By convention, indentation is always four spaces.

-

### Function Type 

Defining a function creates a function object, which has type function:

```none
>>> type(best_ice_cream)
<type 'function'>

>>> print(best_ice_cream)
<function best_ice_cream at 0x1073652a8>
```

-


### Function Name Rules

The rules for function names are the same as for variable names.

* Letters, numbers and underscore are legal.
* The first character can’t be a number. 
* You can’t use a keyword as the name of a function.
* You should avoid having a variable and a function with the same name.

-

### Function Calls

```none
>>> def best_ice_cream():
...     print("Mint chocolate chip.")
... 
>>> best_ice_cream()
Mint chocolate chip.
```

The function definition has to run before the function gets called.

-
-

# Functions
## Part 2

-

### Arguments

* Some functions require one or more arguments. 
* math.power takes two, the base and the exponent.

```none
>>> import math
>>> result = math.pow(2, 3)
>>> print(result)
8.0
```

-

### Parameters 

Inside the function, arguments are assigned to variables called parameters.

```none
>>> def favorite_ice_cream(fav_ice_cream):
...     print("Your favorite ice cream is " + fav_ice_cream)
... 
>>> favorite_ice_cream("mint chocolate chip")
Your favorite ice cream is mint chocolate chip
```

-

### Functions Can Call Functions

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

### Variable Scopes 

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

### docstring Revisited

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

### Built-in Functions

[Built-in Function Docs](https://docs.python.org/3/library/functions.html)

![Moar](img/functions-moar.jpg)

-
-

# BREAK & EXERCISES 

-
-

# Boolean Expressions

-

### What Is It?
A boolean expression is an expression that is either true or false.

-

### Examples

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

### What Is It? 
One of the operators that compares its operands.

-

### Examples 

| Operator | Description              | Example |
| -------- | ------------------------ | ------- |
| ==       | is equal to              | x == y  |
| !=       | is not equal to          | x != y  |
| >        | is greater than          | x > y   |
| <        | is less than             | x < y   |
| >=       | greater than or equal to | x >= y  |
| <=       | less than or equal to    | x <= y  |

-

### ==

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

### !=

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

### >

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

### <

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

### >=

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

### <=

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

### What Is It?
One of the operators that combines boolean expressions.  

There are three logical operators:
* and
* or
* not

-

### and 

Evaluates to True if both conditions are true

```none
>>> x = 5
>>> x > 0 and x < 10
True

>>> x < 0 and x > 3
False
```

-

### or

Evaluates to True if either or both conditions are true

```none
>>> n = 4
>>> n % 2 == 0 or n % 3 == 0
True

>>> n % 5 == 0 or n % 3 == 0
False
```

-

### not

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

### Before we begin...

You have already seen compound statements.   
Functions are syntactically compound statements.  
Don't get overwhelmed by the terminology.  

-

### What Is It?

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
## Part 1

-

### The if Statement

```none
>>> x = 1
>>> if x > 0:
...     print("x is positive")
... 
x is positive
```

-

### Breaking Down The if Statement

* The boolean expression after the if is called the condition.
* If the condition is true, the indented statement runs.
* If the condition is false, nothing happens.
* If statements have the same structure as function definitions. (a header followed by an indented body). These are called compound statements.

-

### The else Clause

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

### Breaking Down the else Clause

The else clause simply provides an alternative path of execution when the if condition is false.

-

### The elif Clause

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

### Breaking Down The elif Clause:

* elif is an abbreviation for "else if".
* If there is an else clause, it has to be at the end, but there doesn't have to be one.
* Each condition is checked in order. The first one to evaluate to true is run and no other is executed or evaluated.

-
-

# Conditional Execution
## Part 2

-

### Nested Conditions

One condition can be nested within another.

-

### Example

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

### Just Because You Can, Doesn't Mean You Should.

Logical operators often provide a way to simplify nested conditional statements.

-

### Nested Conditional Statement 
```none
>>> x = 5
>>> if 0 < x:
...     if x < 10:
...         print("x is a positive single-digit number.")
... 
x is a positive single-digit number.
```

-

### Simplified Using Logical Operator

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

### What is it? 

It is legal for one function to call another.  
It is also legal for a function to call itself.  

Recursion is the process of calling the function that is currently executing.

-

### Example

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

### Infinite Recursion

If the programmer fails to specify a base case that does not make a recursive call, the program will end in a runtime error.

```python
>>> def endless_inception():
...   endless_inception()
... 
>>> endless_inception()
```

-

### Recursion Error

![RecursionError](img/recursion-error.png)

-

### No Base Case = Bad Time

![No Base Case Bad Time](img/recursion-bad-time.jpg)

-
-

# Keyboard Input

-

Python 3
```none
>>> name = input("What is your name?\n")
What is your name?
Seymour
>>> print(name)
Seymour
```

Python 2
```none
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

### What Is It? 

The range type represents an immutable sequence of numbers and is commonly used for looping a specific number of times in for loops.

-

### Quick Intro

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

### More On Range 

We wil continue to talk about the range type further in the context of sequences and iterations in the upcoming sections.

If you just can't wait, feel free to learn more about it in the docs.  
[Range Type](https://docs.python.org/3/library/stdtypes.html#range)

-
-

# Iteration  
# &  
# Control Flow

-

### What Is It?

Iteration is the ability to run a block of statements repeatedly.

-

### What We Will Cover

* for statement
* while statement
* break statement
* continue statement
* pass statement

-

### The for Statement

The for statement is used to iterate over the elements of a sequence (such as a string, tuple or list) or other iterable object.

The for statement has the same structure as function definitions and if statements. (a header followed by an indented body). These are called compound statements.

```none
>>> for i in range(2):
...     print(i)
... 
0
1
```

-

### The while Statement

```
def countdown(n):
    while(n > 0):
        print(n)
        n = n - 1
    print("Blastoff!")

countdown(5)
```

-

### break Statement 

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

### continue Statement

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

### pass Statement

The pass statement does nothing. It can be used when a statement is required syntactically but the program requires no action.

```none
>>> def master_piece():
...     pass
... 
>>> master_piece()
>>>
```

-

### More On Control Flow 

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

### What Is It?

A string is an immutable sequence of characters.

```none
>>> name = 'Marklar'
>>> print(name)
'Marklar'
```

-

### Index Of A String

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

### Expressions Are Allowed 

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

### But...

The value of the index has to be an integer.

```none
>>> print(name[2.2])
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: string indices must be integers, not float
```

-

### The len Built-in Function

[Len](https://docs.python.org/3/library/functions.html#len) is a built-in function that returns the length of an object. When the argument passed to it is a string, it returns the number of characters in the string.

```none
>>> len('one')
3
>>> len('four')
4
```

-

### The Last Item 

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
-

# Working With Strings
## Part 2

-

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

### String Slices

A slice is a segment of a sequence. 

```none
>>> full_name = 'Roberto DeDeus'
>>> print(full_name)
Roberto DeDeus
>>> first_name = full_name[:7]
>>> print(first_name)
Roberto
>>> last_name = full_name[8:]
>>> print(last_name)
DeDeus
>>> full_name[7:8]
' '
```

-

### Srings Are Immutable

```none
>>> a = 'top'
>>> a[0] = 'p'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'str' object does not support item assignment
```

-

### String Methods - upper

```none
>>> fruit = 'banana'
>>> upper_banana = fruit.upper()
>>> print(upper_banana)
BANANA
```

-

### String Methods - find

```none
>>> fruit = 'apple'
>>> fruit.find('p')
1
>>> fruit.find('i')
-1
```

-

### Docs On Strings

[Strings ](https://docs.python.org/3/library/stdtypes.html#text-sequence-type-str)

-
-

# Lists
## Part 1

-

### What Is It? 

A list is a sequence of values.  
Lists are mutable.  
Items in a list can be any type.

-

### Creating A List

```none
vowels = ['a', 'e', 'i', 'o', 'u']
pets = ['DOG', 'CAT', 'BIRD']
nums = [1, 7, 14, 21, 28]
```

-

### Elements Don't have to be The Same Type

```none
[1, 'DOG', True, 2.3]
```

-

### Lists Can Contain (Nested) Lists

```none
[1, 'DOG', ['BALL', 'BAT']]
```

-

### Accessing Elements From A List

```none
>>> vowels = ['a', 'e', 'i', 'o', 'u']
>>> vowels[0]
'a'
```

-

### Accessing Elements From A Nested List

```none
>>> stuff = [1, 'DOG', ['BALL', 'BAT']]
>>> stuff[0]
1
>>> stuff[2]
['BALL', 'BAT']
>>> stuff[2][0]
'BALL'
>>> stuff[2][1]
'BAT'
```

-

### Lists Are Mutable

```none
>>> pets = ['DOG', 'CAT', 'BIRD']
>>> pets[1] = 'TURTLE'
>>> pets
['DOG', 'TURTLE', 'BIRD']
```

-
-

# Lists 
## Part 2

-

### Traversing A List

```none
>>> people = ['Joe', 'Jessica', 'James', 'Jennifer']
>>> for person in people:
...     print(person)
... 
Joe
Jessica
James
Jennifer
```

-

### List Operations

| Operator | Operation                               |
| -------- | --------------------------------------- |
| +        | List Concatenation                      |
| *        | List Repetition                         |
| in       | Element is a member of the sequence     |
| not (in) | Element is not a member of the sequence |

-

### List Concatenation 

```none
>>> parts_a = ['wheels', 'handlebar', 'tank']
>>> parts_b = ['frame', 'chain', 'engine']
>>> parts_c = parts_a + parts_b
>>> parts_c
['wheels', 'handlebar', 'tank', 'frame', 'chain', 'engine']
```

-

### List Repetition

```none
>>> noise = ['Honk']
>>> noise * 3
['Honk', 'Honk', 'Honk']

>>> percolate = ["It's", "Time", "For", "The", "Percolator"]
>>> percolate * 3
["It's", 'Time', 'For', 'The', 'Percolator', "It's", 'Time', 'For', 'The', 'Percolator', "It's", 'Time', 'For', 'The', 'Percolator']
```
-

### Membership Operators

```none
>>> marvel_heroes = ['Ironman', 'Thor', 'Black Panther', 'Black Widow']
>>> 'Batman' in marvel_heroes
False
>>> 'Batman' not in marvel_heroes
True
```

-

### List Slices

A slice is a segment of a sequence. 

```none
>>> colors = ['r', 'o', 'y', 'g', 'b', 'i', 'v']
>>> first_three = colors[:3]
>>> print(first_three)
['r', 'o', 'y']
>>> last_four = colors[3:7]
>>> print(last_four)
['g', 'b', 'i', 'v']
```

-

### Assignment With Slices

```none
>>> values = [1, 2, 3, 4, 5, 6]
>>> values[1:4] = ['a', 'b', 'c']
>>> values
[1, 'a', 'b', 'c', 5, 6]

```

-
-

# Lists 
## Part 3

-

### List Methods - append

Add new element to the end of a list.

```none
>>> letters = ['a', 'b', 'c']
>>> letters
['a', 'b', 'c']
>>> letters.append('d')
>>> letters
['a', 'b', 'c', 'd']
```

-

### List Methods - extend

Append all elements of a list argument to another list

```none
>>> t1 = ['a', 'b', 'c']
>>> t2 = ['d', 'e']
>>> t1.extend(t2)
>>> t1
['a', 'b', 'c', 'd', 'e']
>>> t2
['d', 'e']
```

-

### List Methods - sum

Add up elements of a list.

```none
>>> grades = [60, 70, 90]
>>> average = sum(grades) / len(grades)
>>> print(average)
73.33333333333333
```

-

### List methods - list

```none
>>> make = 'Yamaha'
>>> make_items = list(make)
>>> print(make_items)
['Y', 'a', 'm', 'a', 'h', 'a']
```

-

### Deleting Elements

* pop
* del
* remove

-

### pop

Uses an index to remove an element from the list.  
Returns the removed element.  
If no index is provided, it will default to the last element.

```none
>>> nums = [1, 2, 3]
>>> print(nums)
[1, 2, 3]
>>> x = nums.pop(2)
>>> print(x)
3
>>> print(nums)
[1, 2]
>>> y = nums.pop()
>>> print(y)
2
>>> print(nums)
[1]
```

-

### del

Same as pop but does not return the removed value.

```none
>>> nums = [1, 2, 3]
>>> del nums[2]
>>> print(nums)
[1, 2]
```
-

### remove

Remove an item by the value rather than by index.
Returns None.

```none
>>> fruits = ['apples', 'bananas', 'peaches']
>>> val = fruits.remove('bananas')
>>> print(val)
None
>>> print(fruits)
['apples', 'peaches']
```

-

### Docs On Lists

[Docs On Lists](https://docs.python.org/3/library/stdtypes.html#list)

-
-

# BREAK & EXERCISES 

-
-

# Aliasing

The association of a variable with an object is called a reference.  
In this example, there are two references to the same object.
When an object has more than one reference, we say that the object is aliased.

```none
>>> a = [1, 2, 3]
>>> b = a
>>> b is a
True
```

-
-

# Tuples
## Part 1

-

### What Is It?

A tuple is a sequence of values.  
Tuples are immutable.  
Items in a tuple can be any type.

-

### Creating A Tuple

* comma separated list of values
* comma separated list of values enclosed in parantheses
* using the built-in tuple() function

-

### Comma Separated List Of Values

```none
>>> t1 = 1, 2, 3, 4, 5
>>> print(t1)
(1, 2, 3, 4, 5)
>>> type(t1)
<class 'tuple'>
```

-

### Enclosed In Parantheses

```none
>>> t2 = ('a', 'e', 'i', 'o', 'u')
>>> t2
('a', 'e', 'i', 'o', 'u')
>>> type(t2)
<class 'tuple'>
```

-

### tuple Function

```none
>>> t3 = tuple(['king', 'queen', 'bishop', 'knight', 'rook', 'pawn'])
>>> print(t3)
('king', 'queen', 'bishop', 'knight', 'rook', 'pawn')
>>> type(t3)
<class 'tuple'>
```

If the argument is a sequence, the result is a tuple with the elements of the sequence:

```none
>>> name_tuple = tuple("Roberto")
>>> print(name_tuple)
('R', 'o', 'b', 'e', 'r', 't', 'o')
```

-

### Single Element Tuples

When creating a tuple with a single element, you have to include a final comma.

```none
>>> t1 = 'a'
>>> type(t1)
<class 'str'>

>>> t1 = 'a',
>>> type(t1)
<class 'tuple'>
>>> print(t1)
('a',)
```

-

### Tuples Are Immutable

```none
>>> sides = ('a', 'b')
>>> sides[0] = 'z'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'tuple' object does not support item assignment
```

-
-

# Tuples
## Part 2

-

### Tuple Assignment

Suppose you needed to swap the values of variables a and b. A conventional solution would involve assigning one of the values to a temporary variable.

```none
>>> a = 1
>>> b = 2
>>> print(a, b)
(1, 2)

>>> temp = a
>>> a = b
>>> b = temp
>>> print(a, b)
(2, 1)
```

-

### Tuple Assignment

The left side is a tuple of variables.  
The right side is a tuple of expressions.  
Each value is assigned to its respective variable.  
All the expressions on the right side are evaluated before any of the assignments.   
The number of variables on the left and the number of values on the right have to be the same.  

```none
>>> a = 1
>>> b = 2
>>> print(a, b)
(1, 2)
>>> a, b = b, a
>>> print(a, b)
(2, 1)
```

-

### Tuples As Return Values

A function can only return one value.  
A tuple can be used to effectively return multiple values.  

```none
def first_and_last(word):
  return word[0], word[-1]

print(first_and_last("monkey"))
('m', 'y')
```

-

### Tuples As Args - Gather

Functions can take a variable number of arguments. A parameter name that begins with * gathers arguments into a tuple.

```python
def print_all(*args):
    print(type(args))

print_all("kit kat", "snickers", "milky way")
```

-

### Tuples As Args - Scatter

```python
def sum(a, b):
    return a + b

print(sum(1, 2))

t = (1, 2)
print(sum(*t))
```

-
-

# zip Built-in Function

-

### What Is It? 

A function that takes two or more sequences and interleaves them.  
Returns a zip object. 

-

### How Does It Work?

```none
>>> s = 'abc'
>>> t = [0, 1, 2]
>>> result = zip(s, t)
>>> type(result)
<class 'zip'>
>>> print(result)
<zip object at 0x10b7c2188>
```

-

### Special Note About Python 2

In Python 2, the zip function returns a list of tuples.

```none
>>> s = 'abc'
>>> t = [0, 1, 2]
>>> zip(s, t)
[('a', 0), ('b', 1), ('c', 2)]
>>> result = zip(s, t)
>>> type(result)
<type 'list'>
```
-

### Iterating With Zip

```none
>>> s = 'abc'
>>> t = [0, 1, 2]
>>> for pair in zip(s, t):
...     print(pair)
... 
('a', 0)
('b', 1)
('c', 2)
```

-
-

# enumerate Built-in Function

-

### What is it? 

A function that takes an interable and allows the iteration over a sequence of pairs; an index and an element from the given iterable.  
Returns an enumerate object.

-

### How Does It Work?

```none
>>> trilogy = ['The Matrix', 'The Matrix Reloaded', 'The Matrix Revolutions']
>>> for index, element in enumerate(trilogy, start= 1):
...     print(index, element)
... 
1 The Matrix
2 The Matrix Reloaded
3 The Matrix Revolutions
```

-
-

# BREAK & EXERCISES 

-
-

# Dictionaries
## Part 1

-

### What is it? 

A dictionary is an unordered mapping of key-value pairs.  
Dictionaries are indexed by keys of any immutable type.  

-

### Creating A Dictionary

```python
empty_dict = {}
another_empty_dict = dict()
phone_numbers = {'mom': '302-123-4567', 'dad': '302-123-4567', 'my_boy_blue': '302-654-9876'}
items_to_prices = {'milk', '4.5', 'bread': '2.55', 'beef': '7.50'}
```

-

### Accessing Elements From A Dictionary

Use keys to look up corresponding values.

```none
>>> english_to_spanish = {'one': 'uno', 'two': 'dos', 'three': 'tres'}
>>> english_to_spanish['one']
'uno'
>>> english_to_spanish['four']
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
KeyError: 'four'
```

-

### The In Operator - Keys

The in operator can be used to check if a key is present in the dictionary.

```none
>>> english_to_spanish = {'one': 'uno', 'two': 'dos', 'three': 'tres'}
>>> 'one' in english_to_spanish
True
>>> 'four' in english_to_spanish
False
```

-

### The In Operator - Values

```none
>>> english_to_spanish = {'one': 'uno', 'two': 'dos', 'three': 'tres'}
>>> english_to_spanish.keys()
dict_keys(['one', 'two', 'three'])
>>> english_to_spanish.values()
dict_values(['uno', 'dos', 'tres'])
>>> 'uno' in english_to_spanish.values()
True
```

-

### Updating Items In A Dictionary

If the item already exist, it will be updated. If the item does not exist, it will be added.
```none
>>> spells = {}
>>> spells['Expelliarmus'] = 'The only spell Harry knows.'
>>> print(spells)
{'Expelliarmus': 'The only spell Harry knows.'}
>>> spells['Expelliarmus'] = 'A useless spell that can be ignored if you own a Nintendo Wii hand strap.'
>>> print(spells)
{'Expelliarmus': 'A useless spell that can be ignored if you own a Nintendo Wii hand strap.'}
```

-

### Deleting Items From Dictionary


```none
>>> nums_to_words = {1: 'one', 2: 'two', 3: 'three'}
>>> print(nums_to_words)
{1: 'one', 2: 'two', 3: 'three'}
```

del
```none
>>> del nums_to_words[1]
>>> print(nums_to_words)
{2: 'two', 3: 'three'}
```

pop
```none
>>> item = nums_to_words.pop(3)
>>> print(item)
three
>>> print(nums_to_words)
{2: 'two'}
```

-
-

# Dictionaries
## Part 2

-

### Dictionary Methods - get

Returns the value for key if key is in the dictionary, else returns a default item.  
This method avoids KeyError.

```none
>>> xmen_powers = {'Phoenix': 'Telepathic and telekinetic', 'Wolverine': 'Healing and claws'}
>>> result = xmen_powers.get('Wolverine')
>>> print(result)
Healing and claws
```

Default value provided
```none
>>> result = xmen_powers.get('Nightcrawler', 'Unknown Powers')
>>> print(result)
Unknown Powers
```

Default value not provided
```none
>>> result = xmen_powers.get('Captain Underpants') 
>>> print(result)
None
```

-

### Dictionary Iteration

```none
>>> xmen_powers = {'Phoenix': 'Telepathic and telekinetic', 'Wolverine': 'Healing and claws'}
>>> for key in xmen_powers:
...      print("key: {0:20s} \tValue: {1:s}".format(key, xmen_powers[key]))
... 
key: Phoenix              	Value: Telepathic and telekinetic
key: Wolverine            	Value: Healing and claws
```

-

### Dictionary Methods - items

The items() method in dictionaries returns a sequence of tuples where each tuple is a key-value pair.

```none
>>> simple_dict = {'a': 1, 'b': 2, 'c': 3}
>>> simple_dict.items()
dict_items([('a', 1), ('b', 2), ('c', 3)])
```

-

### Iterating Dictionaries With items Method

```none
>>> for key, value in simple_dict.items():
...     print(key, value)
... 
a 1
b 2
c 3
```

-
-

# BREAK & EXERCISES 

-
-

# Persistence
## Files

-

### The open Built-in Function

Use the [open](https://docs.python.org/3/library/functions.html#open) built-in function to acquire a file object.

```none
>>> fout = open('new_file', 'w')
>>> fout.write("Hello file\n")
11
>>> fout.close()
>>> fin = open('new_file', 'r')
>>> for line in fin:
...     print(line)
... 
Hello file

```

-

### Available Modes

| character | Meaning                                                         |
| --------- | --------------------------------------------------------------- |
| r         | open for reading (default)                                      |
| w         | open for writing, truncating the file first                     |
| x         | open for exclusive creation, failing if the file already exists |
| a         | open for writing, appending to the end of the file if it exists |
| b         | binary mode                                                     |
| t         | text mode (default)                                             | 
| +         | open a disk file for updating (reading and writing)             |

-

### os Module

-

### What Is It?

This [os module](https://docs.python.org/3/library/os.html) provides a portable way of using operating system dependent functionality.

-

### How Does It Work?

```none
```

-
-

# Exceptions

-

### What Is It? 

Exceptions are a means of breaking out of the normal flow of control of a code block in order to handle errors or other exceptional conditions.

```none
>>> fin = open('i_like_turtles.py', 'r')
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
FileNotFoundError: [Errno 2] No such file or directory: 'i_like_turtles.py'

```

-

### The Try Statement

The [try](https://docs.python.org/3/reference/compound_stmts.html#try) statement specifies exception handlers and/or cleanup code for a group of statements.  
The except clause(s) specify one or more exception handlers. When no exception occurs in the try clause, no exception handler is executed.

```none
>>> try:
...     fin = open('i_like_turtles.py', 'r')
... except FileNotFoundError:
...     print('The file does not exist!')
... 
The file does not exist!

```

-

### The except Clause 

The except clause(s) specify one or more exception handlers.

-

### The else Clause

A way to specify a block of code should be run only if no exceptions were raised at all,

-

### The finally clause

If finally is present, it specifies a ‘cleanup’ handler.

-

### The with Statement

The [with](https://docs.python.org/3/reference/compound_stmts.html#with) statement is used to wrap the execution of a block with methods defined by a context manager.

-
-

# Persistence
## Database

-

### dbm Module

-

### Pickling

-
-

# BREAK & EXERCISES 

-
-

# Writing Modules

-
-

# Classes & Objects

-
-

# Classes & Functions

-
-

# Inheritance

-
-
