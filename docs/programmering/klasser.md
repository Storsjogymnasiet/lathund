---
weight: 10
---
# Klasser

## OOP - Objekt Orienterad Programmering
Klasser är mallar för att skapa objekt.
En klass beskriver vilka egenskaper (variabler) och funktioner (metoder) som ett objekt ska ha. Det betyder att en klass är en mall medan objekt är de faktiska sakerna som byggs av mallen.

## Skapa en klass

    class Car:
        def __init__(self, brand, speed):
            self.brand = brand
            self.speed = speed

        def drive(self):
            print(f"{self.brand} kör i {self.speed} km/h")
    
    class Student:
        def __init__(self, name, age):
            self.name = name
            self.age = age

        def introduce(self):
            print(f"Hej, jag heter {self.name} och är {self.age} år.")
    
    class Pet:
        def __init__(self, name, animal_type):
            self.name = name
            self.animal_type = animal_type

        def make_sound(self):
            print(f"{self.name} gör ett ljud")

## Skapa ett objekt

    car1 = Car("Volvo", 60)
    car1.drive() # Volvo kör i 60 km/h
    
    student1 = Student("Hasse", 16)
    student1.introduce() # Hej, jag heter Hasse och är 16 år.

    pet1 = Pet("Molly", "Hund")
    pet1.make_sound() # Molly gör ett ljud


## \_\_init_\_() metoden
\_\_init_\_() körs när objektet skapas från en klass. Den används för att ge objektet startvärden och för att köra kod vid start. \_\_init_\_() gör det möjligt för objekten att få unika värden

## self parametern
self pekar på objektets aktuella variabler. self gör det möjligt för ett objekt att nå sina egna variabler.

    class Person:
        def __init__(self, name)
            self.name = name

        def say_name()
            print(self.name)