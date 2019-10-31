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
items_to_prices = {'milk': '4.5', 'bread': '2.55', 'beef': '7.50'}
```

-

### Accessing Elements From A Dictionary

Use keys to look up corresponding values.

```python
english_to_spanish = {'one': 'uno', 'two': 'dos', 'three': 'tres'}
english_to_spanish['one']
# 'uno'
english_to_spanish['four']
# Traceback (most recent call last):
#   File "<stdin>", line 1, in <module>
# KeyError: 'four'
```

-

### The In Operator - Keys

The in operator can be used to check if a key is present in the dictionary.

```python
english_to_spanish = {'one': 'uno', 'two': 'dos', 'three': 'tres'}
'one' in english_to_spanish
# True
'four' in english_to_spanish
# False
```

-

### The In Operator - Values

```python
english_to_spanish = {'one': 'uno', 'two': 'dos', 'three': 'tres'}
english_to_spanish.keys()
# dict_keys(['one', 'two', 'three'])
english_to_spanish.values()
# dict_values(['uno', 'dos', 'tres'])
'uno' in english_to_spanish.values()
# True
```

-

### Updating Items In A Dictionary

If the item already exist, it will be updated. If the item does not exist, it will be added.
```python
spells = {}
spells['Expelliarmus'] = 'The only spell Harry knows.'
print(spells)
# {'Expelliarmus': 'The only spell Harry knows.'}
spells['Expelliarmus'] = 'A useless spell that can be ignored if you own a Nintendo Wii hand strap.'
print(spells)
# {'Expelliarmus': 'A useless spell that can be ignored if you own a Nintendo Wii hand strap.'}
```

-

### Deleting Items From Dictionary


```python
nums_to_words = {1: 'one', 2: 'two', 3: 'three'}
print(nums_to_words)
# {1: 'one', 2: 'two', 3: 'three'}
```

del
```python
del nums_to_words[1]
print(nums_to_words)
# {2: 'two', 3: 'three'}
```

pop
```python
item = nums_to_words.pop(3)
print(item)
# three
print(nums_to_words)
# {2: 'two'}
```

-
-

# Dictionaries
## Part 2

-

### Dictionary Methods - get

Returns the value for key if key is in the dictionary, else returns a default item.  
This method avoids KeyError.

```python
xmen_powers = {'Phoenix': 'Telepathic and telekinetic', 'Wolverine': 'Healing and claws'}
result = xmen_powers.get('Wolverine')
print(result)
# Healing and claws
```

Default value provided
```python
result = xmen_powers.get('Nightcrawler', 'Unknown Powers')
print(result)
# Unknown Powers
```

Default value not provided
```python
result = xmen_powers.get('Captain Underpants') 
print(result)
# None
```

-

### Dictionary Iteration

```python
xmen_powers = {'Phoenix': 'Telepathic and telekinetic', 'Wolverine': 'Healing and claws'}
for key in xmen_powers:
    print("key: {0:20s} \tValue: {1:s}".format(key, xmen_powers[key]))

# key: Phoenix              	Value: Telepathic and telekinetic
# key: Wolverine            	Value: Healing and claws
```

-

### Dictionary Methods - items

The items() method in dictionaries returns a sequence of tuples where each tuple is a key-value pair.

```python
simple_dict = {'a': 1, 'b': 2, 'c': 3}
simple_dict.items()
# dict_items([('a', 1), ('b', 2), ('c', 3)])
```

-

### Iterating Dictionaries With items Method

```python
for key, value in simple_dict.items():
    print(key, value)

# a 1
# b 2
# c 3
```

-

### zip Built-in Function Revisited

```python
keys = ['a', 'b', 'c']
values = [1, 2, 3]
my_dict = dict(zip(keys, values))
print(my_dict)
# {'a': 1, 'b': 2, 'c': 3}
```

-
-

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

```python
my_set = {1, 2, 3, 4}
print(my_set)
# {1, 2, 3, 4}
type(my_set)
# <class 'set'>
```

-

### Creating A Set - Using Built-in Function

* The built-in set function takes any sequence as its argument.
* Items in a set are not ordered.

```python
my_other_set = set(['a', 'a', 'b', 'c'])
print(my_other_set)
# {'b', 'a', 'c'}
yet_another_set = set()
print(yet_another_set)
# set()
```

-

### Membership Testing

Use the in keyword as with other types to determine membership.

```python
zoo_animals = set(['lion', 'elephant', 'rhino'])
'pigeon' in zoo_animals
# False
```

-
-

# Sets 
## Part 2

-

### add

If the item being added already exists, nothing happens. Otherwise the new item is added.

```python
abcs = {'a', 'b', 'c'}
abcs.add('d')
print(abcs)
# {'a', 'b', 'c', 'd'}
 
abcs.add('a')
print(abcs)
# {'a', 'b', 'c', 'd'}
```

-

### update

Adds the contents of a new dictionary 

```python
set_1 = {1, 2, 3}
set_2 = set()
set_2.update(set_1)
set_2
# {1, 2, 3}
```

-

### remove 

Removes an item from the set. If the item isn't present in the set, it raises a KeyError.

```python
abcs = {'a', 'b', 'c'}
abcs.remove('a')
print(abcs)
# {'b', 'c'}

abcs.remove('z')
# Traceback (most recent call last):
#  File "<stdin>", line 1, in <module>
# KeyError: 'z'
```

-

### discard

Just like remove but does not raise exception.

```python
abcs = {'a', 'b', 'c'}
abcs.discard('z')
```

-

### pop

Arbitrarily removes and returns an item from the set.

```python
abcs = {'a', 'b', 'c'}

removed_item = abcs.pop()
print(removed_item)
# a 

removed_item = abcs.pop()
print(removed_item)
# b

print(abcs)
# {'c'}
```

-

### clear

Removes all items in one shot.

```python
abcs = {'a', 'b', 'c'}
abcs.clear()
print(abcs)
# set()
```

-
-


# The End

![Parrot](img/parrot.jpg)