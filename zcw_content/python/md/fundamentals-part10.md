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

### Embedded Objects

An object that is an attribute of another object is embedded.

![mytryoshka_doll](img/matryoshka_doll.JPG)

-

### Embedded Objects Continued 

```python

```

-
-


# The End

![Parrot](img/parrot.jpg)