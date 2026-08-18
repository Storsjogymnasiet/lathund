---
weight: 7
---
# Dictionaries

## Engelska till Svenska

Dictionaries är ett smidigt sätt att spara data i key:value par. Det betyder att man kopplar ett värde med en unik nyckel. Dictionaries fungerar som ordböcker där man frågar om ett ord på svenska som sedan leder till samma ord på engelska.

    swedish_to_english = {
        "äpple" : "apple",
        "stege" : "ladder",
        "skola" : "school"
    }

    swedish_to_english["skola"] # school

## Manipulera Dictionaries

### Lägg Till
Använd namnet på nyckeln för att lägga till den eller med update metoden.
    car = {
        "brand": "Ford",
        "model": "Mustang",
        "year": 1964
    }

    # 1.
    car["year"] = 1999
    # 2.
    car.update({"year" : 1999})
### Ändra
Ändra dictionaries via namnet på nyckeln eller med update metoden.
    car = {
        "brand": "Ford",
        "model": "Mustang",
        "year": 1964
    }

    # 1.
    car["year"] = 1999
    # 2.
    car.update({"year" : 1999})
### Ta Bort
Ta bort från dictionaries med pop() methoden.
    car = {
        "brand": "Ford",
        "model": "Mustang",
        "year": 1964
    }

    car.pop(year)


## Loopa Genom Dictionaries
Det finns flera sätt att loopa genom en dictionary.

    car = {
        "brand": "Ford",
        "model": "Mustang",
        "year": 1964
    }

    for key in car.keys():
        print(key) # brand, model, year
    
    for value in car.values():
        print(value) # Ford, Mustang, 1964
    
    for key, value in car.items()
        print(key, value) # brand, Ford, model, Mustang, year, 1964