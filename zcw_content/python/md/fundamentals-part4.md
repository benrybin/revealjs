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
def endless_inception():
    endless_inception()

endless_inception()
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
```python
name = input("What is your name?\n")
# What is your name?
Seymour
print(name)
# Seymour
```

Python 2
```python
want = raw_input("What do you want\n")
# What do you want
feed me
print(want)
# 'feed me'
```

-
-

# The Range Type

-

### What Is It? 

The range type represents an immutable sequence of numbers and is commonly used for looping a specific number of times in for loops.  

-

### Quick Intro

The range object itself doesn’t contain any of the values in the sequence. Instead, it generates them one at a time, on demand, during iteration. 

```python
a = range(10)
print(a)
# range(0, 10)
type(a)
# <class 'range'>
type(range)
# <class 'type'>
list(a)
# [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

```

-

### Special Note About Python 2

In Python 2, the range function would simply return a list. 

```python
a = range(10)
print(a)
# [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
type(a)
# <type 'list'>
type(range)
# <type 'builtin_function_or_method'>
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

```python
for i in range(2):
    print(i)

# 0
# 1
```

-

### The while Statement

```python
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

```python
for i in range(10):
    print(i)
    if(i == 5):
       print("I have found what I was looking for.")
       break

# 0
# 1
# 2
# 3
# 4
# 5
# I have found what I was looking for.
```

-

### continue Statement

The continue statement continues with the next iteration of the loop.

```python
for i in range(10):
    if(i == 5):
      print("Skipping number 5")
        continue
    print(i)

# 0
# 1
# 2
# 3
# 4
# Skipping number 5
# 6
# 7
# 8
# 9
```

-

### pass Statement

The pass statement does nothing. It can be used when a statement is required syntactically but the program requires no action.

```python
def master_piece():
    pass

master_piece()
```

-

### More On Control Flow 

[Control Flow Tutorial](https://docs.python.org/3/tutorial/controlflow.html)

![Control Flow More](img/control-flow-moar.jpg)

-
-


# The End

![Parrot](img/parrot.jpg)