# Persistence
## Database Files

-

### dbm Module

The [dbm module](https://docs.python.org/3/library/dbm.html) provides an interface for creating adn updating database files.

-

### Pickling

The [pickle module](https://docs.python.org/3/library/pickle.html) can be used to serialize and de-serialize a Python object.

-
-

# Writing Modules

-

### Problem

my_module.py
```python
def say_hello():
    print("Hello")

say_hello()
```

app.py
```
import my_module as mm
# ouput "Hello"
```

-

### Solution

my_module.py
```python
def say_hello():
    print("Hello")

if __name__ == '__main__':
    say_hello()
```

app.py
```
import my_module as mm
# no output

say_hello()
# ouput "Hello"
```

-
-


# The End

![Parrot](img/parrot.jpg)