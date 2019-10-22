# os Module

-

### What Is It?

This [os module](https://docs.python.org/3/library/os.html) provides a portable way of using operating system dependent functionality.

-

### How Does It Work?

The code below uses the os module to display the current working directory. 
This is equivalent to the console command 'pwd'.

```python
import os
cwd = os.getcwd()
cwd 
# '/Users/rd/'
```

-

### Paths

A **relative path** relates to the location of a file relative to the current working directory.  

An **absolute path** is a path that begins from the root directory of the operating system. Paths that start with a / (from the root directory) are not relative to the current directory.

```python
import os
os.path.abspath('README.md')
# '/Users/rd/Dev/my_awesome_project/README.md'
```

-

### Verify a file exists.

```python
import os
os.path.exists('README.md')
# True
```

-

### Verify a path points to a directory.

```python
import os
os.path.isdir('/Users/rd')
# True
```

-

### Verify a path points to a file.

```python
import os
os.path.isfile('/Users/rd')
# False
```

-

### List the contents of a directory.

```python
import os
os.listdir('/Users/rd')
# ['Applications', 'Desktop', 'Documents', 'Downloads', '.bash_profile']
```

-
-

# Exceptions

-

### What Is It? 

Exceptions are a means of breaking out of the normal flow of control of a code block in order to handle errors or other exceptional conditions.

```python
fin = open('i_like_turtles.py', 'r')
# Traceback (most recent call last):
#   File "<stdin>", line 1, in <module>
# FileNotFoundError: [Errno 2] No such file or directory: 'i_like_turtles.py'
```

-

### The Try Statement

The [try](https://docs.python.org/3/reference/compound_stmts.html#try) statement specifies exception handlers and/or cleanup code for a group of statements.  

```python
try:
    fin = open('i_like_turtles.py', 'r')
except FileNotFoundError:
    print('The file does not exist!')

# The file does not exist!
```

-

### The except Clause 

The except clause(s) specifies one or more exception handlers. When no exception occurs in the try clause, no exception handler is executed.

```python
try:
    print(100 / 10)
except ZeroDivisionError:
    print("Division by zero is not allowed.")

# 10.0
```

-

### The else Clause

A way to specify a block of code should be run only if no exceptions were raised at all,

```python
try:
    print(100 / 10)
except ZeroDivisionError:
    print("Division by zero is not allowed.")
else:
    print("No issues were encountered.")

# 10.0
# No issues were encountered.
```

```python
try:
    print(100 / 0)
except ZeroDivisionError:
    print("Division by zero is not allowed.")
else:
    print("No issues were encountered.")

# Division by zero is not allowed.
```

-

### The finally clause

If finally is present, it specifies a ‘cleanup’ handler.

```python
try:
    print(100 / 10)
except ZeroDivisionError:
    print("Division by zero is not allowed.")
finally:
    print("This runs no matter what happened.")

# 10.0
# This runs no matter what happened.
```

```python
try:
    print(100 / 0)
except ZeroDivisionError:
    print("Division by zero is not allowed.")
finally:
    print("This runs no matter what happened.")

# Division by zero is not allowed.
# This runs no matter what happened.
```

-
-

# Persistence
## Files

-

### The open Built-in Function

Use the [open](https://docs.python.org/3/library/functions.html#open) built-in function to acquire a file object.

```python
fout = open('new_file', 'w')
fout.write("Hello file\n")
# 11
fout.close()
fin = open('new_file', 'r')
for line in fin:
    print(line)

# Hello file
fout.close()
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
-

# The with Statement

The [with](https://docs.python.org/3/reference/compound_stmts.html#with) statement is used to wrap the execution of a block with methods defined by a context manager.

The context manager will automatically close the file handler when you are done with it.

-

### Opening Files Using With Statement

```python
with open('new_file', 'r') as file_handler:
    for line in file_handler:
        print(line)

```

-
-

# Putting It Together

```python
import os

def read_file(file_name):
    with open(file_name, 'r') as file_handler:
        for line in file_handler:
            print(line)

file_name = "new_file.txt"
if os.path.exists(file_name) and os.path.isfile(file_name):
    read_file(file_name)
else:
    print("invalid file path")
```

-
-

# The End

![Parrot](img/parrot.jpg)