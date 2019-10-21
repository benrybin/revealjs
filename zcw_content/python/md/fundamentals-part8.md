# Sets 
## Part 1

-

### What is it? 

A [set](https://docs.python.org/3/library/stdtypes.html#set) works much like a list but without allowing any duplicates.

-

### Why 

Common uses include:

* membership testing
* removing duplicates from a sequence
* computing mathematical operations such as intersection, union, difference, and symmetric difference

-

### Creating A Set - Using Curly Braces

```none
>>> my_set = {1, 2, 3, 4}
>>> print(my_set)
{1, 2, 3, 4}
>>> type(my_set)
<class 'set'>
```

-

### Creating A Set - Using Built-in Function

* The built-in set function takes any sequence as its argument.
* Items in a set are not ordered.

```none
>>> my_other_set = set(['a', 'a', 'b', 'c'])
>>> print(my_other_set)
{'b', 'a', 'c'}
>>> yet_another_set = set()
>>> print(yet_another_set)
set()
```

-

### Membership Testing

Use the in keyword as with other types to determine membership.

```none
>>> zoo_animals = set(['lion', 'elephant', 'rhino'])
>>> 'pigeon' in zoo_animals
False
```

-
-

# Sets 
## Part 2

-

### add

If the item being added already exists, nothing happens. Otherwise the new item is added.

```none
```

-

### update

Adds the contents of a new dictionary 

```none
>>> set_1 = {1, 2, 3}
>>> set_2 = set()
>>> set_2.update(set_1)
>>> set_2
{1, 2, 3}
```

-

### remove 

Removes an item from the set. If the item isn't present in the set, it raises a KeyError.

```none
```

-

### discard

Just like remove but does not raise exception.

```none
```

-

### pop

Arbitrarily removes and returns an item from the set.

```none
```

-

### clear

Removes all items in one shot.

```none
```

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

The except clause(s) specifies one or more exception handlers. When no exception occurs in the try clause, no exception handler is executed.

```none
>>> try:
...    print(100 / 10)
... except ZeroDivisionError:
...    print("Division by zero is not allowed.")
... 
10.0
```

-

### The else Clause

A way to specify a block of code should be run only if no exceptions were raised at all,

```none
```

-

### The finally clause

If finally is present, it specifies a ‘cleanup’ handler.

```none
```

-

### The with Statement

The [with](https://docs.python.org/3/reference/compound_stmts.html#with) statement is used to wrap the execution of a block with methods defined by a context manager.

-
-

# Persistence
## Database

-

### dbm Module

The [dbm module](https://docs.python.org/3/library/dbm.html) provides an interface for creating adn updating database files.

-

### Pickling

The [pickle module](https://docs.python.org/3/library/pickle.html) can be used to serialize and de-serialize a Python object.

-
-


# The End

![Parrot](img/parrot.jpg)