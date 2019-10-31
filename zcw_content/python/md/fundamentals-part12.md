# Conditional Expressions

-

### What Is It? 

[Conditional expressions](https://docs.python.org/3/reference/expressions.html#conditional-expressions) are sometimes referred to as ternary operator.  
In essesence, a conditional expression is a simplified way to express an conditional statement.

-

### The Problem

Even a simple condition can take many lines of code to be expressed using a traditional conditional statement.

```python
def conditional_statement(value: bool) -> bool:
    if(value):
        return True
    else:
        return False

coditional_statemnt(True)
# True

coditional_statemnt(False)
# False
```

-

### The Solution

Conditional expressions can be used to express conditional logic more consisely.

The syntax takes the following format:  
value = true-expr if condition else false-expr

```python
def conditional_statement(value: bool) -> bool:
    return True if value == True else False
```

-

### Readability Counts

Don't automatically assume that concise is always better. In some cases, it may be worth having code that is more drawn out and readable over shorter and hard to read code.

-
-

# List Comprehensions

-

### What Is It?

[List Comprehensions](https://docs.python.org/3/tutorial/datastructures.html?highlight=list%20comprehension) provide a consise way to create lists.

-

### Why?

Suppose you want to generate a list with only items that meet a certain criteria.

```python
output = []
for value in range(10):
    if value > 5:
        output.append(str(value))

output
# ['6', '7', '8', '9']
```

-

### How

The same code can be simplified with list comprehensions.

The syntax takes the following format:  
list_comp = [expr for value in collection if condition]

```python
ouput = [str(value) for value in range(10) if value > 5]
output
# ['6', '7', '8', '9']
```

-

### Breaking It Down 

* Expression for final value
* for clause (iteration)
* if clause (conditional to determine which items should be included)

-
-

# Dictionary Comprehensions

-

### How

The syntax takes the following format:  
dict_comp = {key-expr : value-expr for value in collection if condition}

```python
people = ['Chris', 'Dolio', 'Froilan', 'Kris', 'Roberto']
dict_comp = {person : person.upper() for person in people if len(person) > 4}
dict_comp
{'Chris': 'CHRIS', 'Dolio': 'DOLIO', 'Froilan': 'FROILAN', 'Roberto': 'ROBERTO'}
```

-
-

# Set Comprehensions

-

### How

The syntax takes the following format:  
set_comp = {expr for value in collection if condition}

```python
nums = [1, 2, 3, 4, 5]
odds_squared = {num ** 2 for num in nums if num % 2 != 0}
odds_squared
# {1, 9, 25}
```

-
-

# Generator Expressions

-

### What Is It? 

A [Generator expression](https://docs.python.org/3/reference/expressions.html?highlight=generator#generator-expressions) yeilds a new generator object.  
Generator objects are used to lazily iterate a sequence by levaraging the power of iteration.

-


-
-


# The End

![Parrot](img/parrot.jpg)
