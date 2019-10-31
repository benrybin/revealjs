# Aliasing

-

The association of a variable with an object is called a reference.  
In this example, there are two references to the same object.
When an object has more than one reference, we say that the object is aliased.

```python
a = [1, 2, 3]
b = a
b is a
# True
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

```python
t1 = 1, 2, 3, 4, 5
print(t1)
# (1, 2, 3, 4, 5)
type(t1)
# <class 'tuple'>
```

-

### Enclosed In Parantheses

```python
t2 = ('a', 'e', 'i', 'o', 'u')
print(t2)
# ('a', 'e', 'i', 'o', 'u')
type(t2)
# <class 'tuple'>
```

-

### tuple Function

Any sequence or iterator can be converted into a tuple by invoking the tuple function. 

```python
t3 = tuple(['king', 'queen', 'bishop', 'knight', 'rook', 'pawn'])
print(t3)
# ('king', 'queen', 'bishop', 'knight', 'rook', 'pawn')
type(t3)
# <class 'tuple'>
```

```python
name_tuple = tuple("Roberto")
print(name_tuple)
# ('R', 'o', 'b', 'e', 'r', 't', 'o')
```

-

### Single Element Tuples

When creating a tuple with a single element, you have to include a final comma.

```python
t1 = 'a'
type(t1)
# <class 'str'>

t1 = 'a',
type(t1)
# <class 'tuple'>
print(t1)
# ('a',)
```

-

### Nested Tuples

Tuples can be nested. In other words, it is possible to create a tuple of tuples.

```python
nested_tuple = (1, 2, 3), (4, 5)
nested_tuple
# ((1, 2, 3), (4, 5))
```

-

### Accessing Elements From A Tuple

Elements can be accessed with square brackets []. Sequences are 0-indexed.

```python
regular_tuple = (1, 2, 3)
regular_tuple[0]
# 1
```

```python
nested_tuple = (1, 2, 3), (4, 5)
nested_tuple[1]
# (4, 5)

nested_tuple[1][0]
# 4
```

-

### Tuples Are Immutable

```python
sides = ('a', 'b')
sides[0] = 'z'
# Traceback (most recent call last):
#   File "<stdin>", line 1, in <module>
# TypeError: 'tuple' object does not support item assignment
```

-

### Mutable Objects Inside Of Tuples

If an object inside of a tuple is mutable, you can modify it in place

```python
my_tuple = (['a', 'b', 'c'], 'roberto', (1, 2, 3))
my_tuple[0]
# ['a', 'b', 'c']
 my_tuple[0].append('d')
my_tuple[0]
(['a', 'b', 'c', 'd'], 'roberto', (1, 2, 3))
```

-
-

# Tuples
## Part 2

-

### Tuple Concatenation 

```python
fruits = ('apples', 'bananas')
vegetables = ('green beans', 'broccoli')
fruits + vegetables
# ('apples', 'bananas', 'green beans', 'broccoli')
```

-

### Unpacking Tuples

```python
nums_tup = (1, 2, 3)
a, b, c = nums_tup
a
# 1
b 
# 2
c 
# 3
```

-

### Tuple Assignment

Suppose you needed to swap the values of variables a and b. A conventional solution would involve assigning one of the values to a temporary variable.

```python
a = 1
b = 2
print(a, b)
# (1, 2)

temp = a
a = b
b = temp
print(a, b)
# (2, 1)
```

-

### Tuple Assignment

The left side is a tuple of variables.  
The right side is a tuple of expressions.  
Each value is assigned to its respective variable.  
All the expressions on the right side are evaluated before any of the assignments.   
The number of variables on the left and the number of values on the right have to be the same.  

```python
a = 1
b = 2
print(a, b)
# (1, 2)
a, b = b, a
print(a, b)
# (2, 1)
```

-

### Tuples As Return Values

A function can only return one value.  
A tuple can be used to effectively return multiple values.  

```python
def first_and_last(word):
    return word[0], word[-1]

print(first_and_last("monkey"))
# ('m', 'y')
```

-

### Tuples As Args - Gather

Functions can take a variable number of arguments. A parameter name that begins with * gathers arguments into a tuple.

```python
def print_all(*args):
    print(type(args))

print_all("kit kat", "snickers", "milky way")
# <class 'tuple'>
```

-

### Tuples As Args - Scatter

```python
def sum(a, b):
    return a + b

print(sum(1, 2))
# 3

t = (1, 2)
print(sum(*t))
# 3
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

```python
s = 'abc'
t = [0, 1, 2]
result = zip(s, t)
type(result)
# <class 'zip'>
print(result)
# <zip object at 0x10b7c2188>
```

-

### Special Note About Python 2

In Python 2, the zip function returns a list of tuples.

```python
s = 'abc'
t = [0, 1, 2]
zip(s, t)
# [('a', 0), ('b', 1), ('c', 2)]
result = zip(s, t)
type(result)
# <type 'list'>
```
-

### Iterating With Zip

```python
s = 'abc'
t = [0, 1, 2]
for pair in zip(s, t):
    print(pair)

# ('a', 0)
# ('b', 1)
# ('c', 2)
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

```python
trilogy = ['The Matrix', 'The Matrix Reloaded', 'The Matrix Revolutions']
for index, element in enumerate(trilogy, start= 1):
    print(index, element)

# 1 The Matrix
# 2 The Matrix Reloaded
# 3 The Matrix Revolutions
```

-
-


# The End

![Parrot](img/parrot.jpg)