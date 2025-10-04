### Week-5-Assignment
## Assignment 1: Design Your Own Class! 🏗️
Create a class representing anything you like (a Smartphone, Book, or even a Superhero!).
Add attributes and methods to bring the class to life!
Use constructors to initialize each object with unique values.
Add an inheritance layer to explore polymorphism or encapsulation.

##Answers
# Encapsulation 
class FarmAnimal:
    def __init__(self, name, age):
        self._name = name
        self._age = age
# Polymorphism 
    def make_sound(self):
        return "Some sound"
    
    def get_info(self):
        return f"{self._name}, {self._age} years"
        
# Inheritance 
class Cow(FarmAnimal):
    def make_sound(self):
        return "Moo!"

class Chicken(FarmAnimal):
    def make_sound(self):
        return "Cluck!"

class Pig(FarmAnimal):
    def make_sound(self):
        return "Oink!"

class Goat(FarmAnimal):
    def make_sound(self):
        return "Meeh!"

class Sheep(FarmAnimal):
    def make_sound(self):
        return "Baa!"

# Demonstration
animals = [
    Cow("Bessie", 3), 
    Chicken("Clucky", 1),
    Pig("Porky", 2),
    Goat("Billy", 4),
    Sheep("Wooly", 3)
]

for animal in animals:
    print(f"{animal.get_info()} says: {animal.make_sound()}")


## Activity 2: Polymorphism Challenge! 🎭 

Create a program that includes animals or vehicles with the same action (like move()). However, make each class define move() differently (for example, Car.move() prints "Driving" 🚗, while Plane.move() prints "Flying" ✈️).

class Animal:
    def move(self):
        raise NotImplementedError("Subclasses must implement this method.")

 class Frog(Animal):
    def move(self):
        return "Jumping"

class Snake(Animal):
    def move(self):
        return "Slithering"

class Rat(Animal):
    def move(self):
        return "Scurrying"

class Cat(Animal):
    def move(self):
        return "Prowling"

class Dog(Animal):
    def move(self):
        return "Running"
   # List of animal instances
animals = [Frog(), Snake(), Rat(), Cat(), Dog()]

# Invoke the move method for each animal
for animal in animals:
    print(f"{animal.__class__.__name__}: {animal.move()}")

