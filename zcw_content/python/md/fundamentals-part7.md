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

### zip Built-in Function Revisited

```none
>>> keys = ['a', 'b', 'c']
>>> values = [1, 2, 3]
>>> my_dict = dict(zip(keys, values))
>>> print(my_dict)
{'a': 1, 'b': 2, 'c': 3}
```

-
-


# The End

![Parrot](img/parrot.jpg)