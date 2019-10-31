# Working With Strings
## Part 1

-

### What Is It?

A string is an immutable sequence of characters.

```python
name = 'Marklar'
print(name)
# 'Marklar'
```

-

### Index Of A String

An index is an offset from the beginning of a sequence.

```python
name = 'Marklar'
first_letter = name[0]
print(first_letter)
# 'M'
second_letter = name[1]
print(second_letter)
# 'a'
```

-

### Expressions Are Allowed 

You can use an expression that contains variables and operators to describe the index.

```python
i = 0
name = "Guido"
print(name[i])
# G
print(name[i + 1])
# u
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

```python
len('one')
# 3
len('four')
# 4
```

-

### The Last Item 

```python
name = "Roberto"
print(len(name))
# 7
last_char = name[len(name) - 1]
print(last_char)
# o
```

Or we can use negative indices

```python
print(name[-1])
# o
print(name[-2])
# t
```

-
-

# Working With Strings
## Part 2

-

### While Loop

```python
index = 0
while index < len(word):
    letter = word[index]
    print(letter)
    index = index + 1

# p
# y
# t
# h
# o
# n
```

-

### For Loop

```python
word = 'python'
for letter in word:
    print(letter)

# p
# y
# t
# h
# o
# n
```

-

### String Slices

A slice is a segment of a sequence. 

```python
full_name = 'Roberto DeDeus'
print(full_name)
# Roberto DeDeus

first_name = full_name[:7]
print(first_name)
# Roberto

last_name = full_name[8:]
print(last_name)
# DeDeus

full_name[7:8]
# ' '
```

-

### Srings Are Immutable

```python
a = 'top'
a[0] = 'p'
# Traceback (most recent call last):
#   File "<stdin>", line 1, in <module>
# TypeError: 'str' object does not support item assignment
```

-

### String Methods - upper

```python
fruit = 'banana'
upper_banana = fruit.upper()
print(upper_banana)
# BANANA
```

-

### String Methods - find

```python
fruit = 'apple'
fruit.find('p')
# 1
fruit.find('i')
# -1
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

Elements can be accessed with square brackets []. Sequences are 0-indexed.

```python
vowels = ['a', 'e', 'i', 'o', 'u']
vowels[0]
# 'a'
```

-

### Accessing Elements From A Nested List

```python
stuff = [1, 'DOG', ['BALL', 'BAT']]
stuff[0]
# 1
stuff[2]
# ['BALL', 'BAT']
stuff[2][0]
# 'BALL'
stuff[2][1]
# 'BAT'
```

-

### Lists Are Mutable

```python
pets = ['DOG', 'CAT', 'BIRD']
pets[1] = 'TURTLE'
print(pets)
# ['DOG', 'TURTLE', 'BIRD']
```

-
-

# Lists 
## Part 2

-

### Traversing A List

```python
people = ['Joe', 'Jessica', 'James', 'Jennifer']
for person in people:
    print(person)

# Joe
# Jessica
# James
# Jennifer
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

```python
parts_a = ['wheels', 'handlebar', 'tank']
parts_b = ['frame', 'chain', 'engine']
parts_c = parts_a + parts_b
print(parts_c)
# ['wheels', 'handlebar', 'tank', 'frame', 'chain', 'engine']
```

-

### List Repetition

```python
noise = ['Honk']
noise * 3
# ['Honk', 'Honk', 'Honk']

percolate = ["It's", "Time", "For", "The", "Percolator"]
percolate * 3
# ["It's", 'Time', 'For', 'The', 'Percolator', "It's", 'Time', 'For', 'The', 'Percolator', "It's", 'Time', 'For', 'The', 'Percolator']
```
-

### Membership Operators

```python
marvel_heroes = ['Ironman', 'Thor', 'Black Panther', 'Black Widow']
'Batman' in marvel_heroes
# False
'Batman' not in marvel_heroes
# True
```

-

### List Slices

A slice is a segment of a sequence. 

```python
colors = ['r', 'o', 'y', 'g', 'b', 'i', 'v']
first_three = colors[:3]
print(first_three)
# ['r', 'o', 'y']
last_four = colors[3:7]
print(last_four)
# ['g', 'b', 'i', 'v']
```

-

### Assignment With Slices

```python
values = [1, 2, 3, 4, 5, 6]
values[1:4] = ['a', 'b', 'c']
print(values)
# [1, 'a', 'b', 'c', 5, 6]

```

-
-

# Lists 
## Part 3

-

### List Methods - append

Add new element to the end of a list.

```python
letters = ['a', 'b', 'c']
letters
# ['a', 'b', 'c']
letters.append('d')
print(letters)
# ['a', 'b', 'c', 'd']
```

-

### List Methods - extend

Append all elements of a list argument to another list

```python
t1 = ['a', 'b', 'c']
t2 = ['d', 'e']
t1.extend(t2)
print(t1_
# ['a', 'b', 'c', 'd', 'e']
print(t2)
# ['d', 'e']
```

-

### List Methods - sum

Add up elements of a list.

```python
grades = [60, 70, 90]
average = sum(grades) / len(grades)
print(average)
# 73.33333333333333
```

-

### List methods - list

```python
make = 'Yamaha'
make_items = list(make)
print(make_items)
# ['Y', 'a', 'm', 'a', 'h', 'a']
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

```python
nums = [1, 2, 3]
print(nums)
# [1, 2, 3]
x = nums.pop(2)
print(x)
# 3
print(nums)
# [1, 2]
y = nums.pop()
print(y)
# 2
print(nums)
# [1]
```

-

### del

Same as pop but does not return the removed value.

```python
nums = [1, 2, 3]
del nums[2]
print(nums)
# [1, 2]
```
-

### remove

Remove an item by the value rather than by index.
Returns None.

```python
fruits = ['apples', 'bananas', 'peaches']
val = fruits.remove('bananas')
print(val)
#None
print(fruits)
# s['apples', 'peaches']
```

-

### Docs On Lists

[Docs On Lists](https://docs.python.org/3/library/stdtypes.html#list)

-
-


# The End

![Parrot](img/parrot.jpg)