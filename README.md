### Week-5-Assignment
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
