# Inheritance

-

### What Is It? 

Inheritance is the ability to define a new class that is a modified version of an ex- isting class.

-

### How Does It Work?

```python
class Humanoid:
    def walk(self):
        print("walking")
    
    def run(self):
        print("running")

class Human(Humanoid):
    def ride_bicycle(self):
        print("riding bicycle")
    
    def walk(self):
        print("moon walking.")

class Siren:
    def sing(self):
        print("singing song to lure in sailors")

```

-
-


# The End

![Parrot](img/parrot.jpg)