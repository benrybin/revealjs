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

```python
type(best_ice_cream)
# <type 'function'>

print(best_ice_cream)
# <function best_ice_cream at 0x1073652a8>
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

```python
def best_ice_cream():
    print("Mint chocolate chip.")

best_ice_cream()
# Mint chocolate chip.
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

```python
import math
result = math.pow(2, 3)
print(result)
# 8.0
```

-

### Parameters 

Inside the function, arguments are assigned to variables called parameters.

```python
def favorite_ice_cream(fav_ice_cream):
    print("Your favorite ice cream is " + fav_ice_cream)

favorite_ice_cream("mint chocolate chip")
# Your favorite ice cream is mint chocolate chip
```

-

### Functions Can Call Functions

```python
def say_hello():
    print("Hello")

def say_hello_two_times():
    say_hello()
    say_hello()

say_hello()
# Hello

say_hello_two_times()
# Hello
# Hello
```

-

### Variable Scopes 

Variables created inside of a function are local.

```python
name = 'Alice'

def print_name():
    name = 'Bob'
    print(name)

def print_other_name():
    name = 'John'
    print(name)

print_name()
# Bob 

print_other_name()
# John

print(name)
# Alice
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


# The End

![Parrot](img/parrot.jpg)
