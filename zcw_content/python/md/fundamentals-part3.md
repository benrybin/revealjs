# Boolean Expressions

-

### What Is It?
A boolean expression is an expression that is either true or false.

-

### Examples

```python
5 == 5         # True

5 == 6         # False

5 > 6          # False

5 < 6          # True
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

```python
0 == 0         # True

'a' == 'b'     # False

True == True   # True

True == False  # False
```

-

### !=

```python
0 != 0         # False

'a' != 'b'     # True

True != True   # False

True !=  False # True
```

-

### >

```python
1 > 0          # True

0 > 1          # False

'a' > 'b'      # False

'b' > 'a'      # True

True > False   # True

False > True   # False
```

-

### <

```python
1 < 0          # False

0 < 1          # True

'a' < 'b'      # True

'b' < 'a'      # False

True < False   # False

False < True   # True
```

-

### >=

```python
0 >= 0         # True

0 >= 1         # False

'a' >= 'a'     # True

'a' >= 'b'     # False
```

-

### <=

```python
0 <= 0         # True

0 <= 1         # True

'a' <= 'b'     # True

'b' <= 'a'     # False
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

```python
x = 5
x > 0 and x < 10
# True

x < 0 and x > 3
# False
```

-

### or

Evaluates to True if either or both conditions are true

```python
n = 4
n % 2 == 0 or n % 3 == 0
# True

n % 5 == 0 or n % 3 == 0
# False
```

-

### not

Negates a boolean expression.

```python
not True
# False

not False
# True

not (1 > 0) 
# False
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

```python
x = 1
if x > 0:
    print("x is positive")

# x is positive
```

-

### Breaking Down The if Statement

* The boolean expression after the if is called the condition.
* If the condition is true, the indented statement runs.
* If the condition is false, nothing happens.
* If statements have the same structure as function definitions. (a header followed by an indented body). These are called compound statements.

-

### The else Clause

```python
x = 7
if x % 2 == 0:
    print("x is even")
else:
    print("x is odd")

# x is odd
```

-

### Breaking Down the else Clause

The else clause simply provides an alternative path of execution when the if condition is false.

-

### The elif Clause

```python
x = 10
y = 5
if x < y:
    print("x is less than y")
elif x > y:
    print("x is greater than y")
else:
    print("x and y are equal")

# x is greater than y
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

```python
x = 10
y = 5

if x == y:
     print("x and y are equal")
else:
    if x < y:
        print("x is less than y")
    else:
        print("x is greater than y")

# x is greater than y
```

-

### Just Because You Can, Doesn't Mean You Should.

Logical operators often provide a way to simplify nested conditional statements.

-

### Nested Conditional Statement 

```python
x = 5
if 0 < x:
    if x < 10:
        print("x is a positive single-digit number.")

# x is a positive single-digit number.
```

-

### Simplified Using Logical Operator

```python
if 0 < x and x < 10:
    print("x is a positive single-digit number.")

# x is a positive single-digit number.
```

-
-


# The End

![Parrot](img/parrot.jpg)
