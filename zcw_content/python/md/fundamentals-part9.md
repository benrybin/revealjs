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
