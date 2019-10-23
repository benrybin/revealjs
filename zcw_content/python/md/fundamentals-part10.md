# Classes & Objects 
## Part 1

-

### Classes

A class is a programmer defined type.  
Classes can be thought of as a blueprint for creating objects.

```python
class Car:
    """Represents a wheeled motor vehicle used for transportation."""

Car
# <class '__main__.Car'>
```

-

### Objects

To create a car, you call the constructor.  
Creating a new object is called **instantiation**.  

```python
my_car = Car()
print(my_car)
# <__main__.Car object at 0x10cb08b38>
```

The object *my_car* is an instance of the *Car* class.  

-

### Attributes - Assignment

You can assign values to an instance using dot notation.

```python
my_car = Car()
my_car.make = 'chevy'
my_car.model = 'camaro'
my_car.transmission = 'manual'
```

-

### Attributes - Reading

You can also read the value of an attribute using dot notation.

```python
my_car = Car()
print(my_car.make)
# chevy

print(my_car.model)
# 'camaro'

print(my_car.transmission)
# 'manual'

print(my_car.x)
# Traceback (most recent call last):
#   File "<stdin>", line 1, in <module>
# AttributeError: 'Car' object has no attribute 'x'
```

-

### Passing Object Instances As Arguments

```python
def print_car_details(car):
    print("Car make: %s" % car.make)
    print("Car model: %s" % car.model)
    print("Transmission: %s" % car.transmission)


print_car_details(my_car)
# Car make: chevy
# Car model: camaro
# Transmission: manual
```

-
-

# Classes & Objects 
## Part 2

-

### Methods 

A method is a function that “belongs to” an object.  

```python
class AnnoyingSinger:
    def sing(self):
        print("Baby shark, do do, do do do do")

pink_fong = AnnoyingSinger()
pink_fong.sing()
# Baby shark, do do, do do do do
```

-

### The __init__() Method

This method is invoked anytime an object is initialized.

```python
class AnnoyingSinger:
    def __init__(self, song):
        self.song = song

    def sing(self):
        print(song)

pink_fong = AnnoyingSinger("Baby shark, do do, do do do do")
pink_fong.sing()
# Baby shark, do do, do do do do

frozen = AnnoyingSinger("Let it go, let it go")
frozen.sing()
# Let it go, let it go
```

-

### The __str__() Method

A special method that returns the string representation of a method.

```python
class Person:
    def __init__(self, name, age, gender):
        self.name = name
        self.age = age
        self.gender = gender

    def __str__(self:
        return f"{self.name} identifies as {self.gender} and is {self.age} years old."

john = Person("John", 25, male)
print(john)
# John identifies as male and is 25 years old.
```

-
-

# Classes & Objects 
## Part 3

-

### Embedded Objects

An object that is an attribute of another object is embedded.

![mytryoshka_doll](img/matryoshka_doll.JPG)

-

### Embedded Object Example 

```python
class Heart:
    def beat(self):
        print("ba-dum ba-dum ba-dum")

class Person:
    def __init__(self):
        self.heart = Heart()


john = Person()
john.heart.beat()
# ba-dum ba-dum
```

-
-

### Classes 

[Classes Docs](https://docs.python.org/3.8/tutorial/classes.html?highlight=classes#)

![Moar](img/classes-moar.jpg)

-


# The End

![Parrot](img/parrot.jpg)