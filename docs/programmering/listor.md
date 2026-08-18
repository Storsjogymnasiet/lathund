---
weight: 6
---
# Listor

## Listor 101

Listor är en sorts variabel som kan hålla flera värden. Värden i en lista kallas för items.

    names = ["Hasse", "Hanna", "Blixten McQueen"]

För att plocka ut ett värde ur en lista så använder man positioner i listan.
OBS! I programmering så räknar man alltid från 0.

    names = ["Hasse", "Hanna", "Blixten McQueen"]
    names[0] # Hasse
    names[2] # Blixten McQueen

## Manipulera Listor

### Lägg Till
append() och insert() lägger till items i listor

    names = ["Hasse", "Hanna", "Blixten McQueen"]

    names.append("Simon")
    names # ["Hasse", "Hanna", "Blixten McQueen", "Simon"]

    names.insert(1, "Johan")
    names # ["Hasse", "Johan", "Hanna", "Blixten McQueen", "Simon"]


### Ändra
Man ändrar items i en lista med hjälp av dens position.

    names = ["Hasse", "Hanna", "Blixten McQueen"]
    names[1] = "Harald"

    names # ["Hasse", "Harald", "Blixten McQueen"]

### Ta Bort
remove() och pop() tar bort items från listor

    names = ["Hasse", "Hanna", "Blixten McQueen"]
    
    names.remove("Hasse")
    names # ["Hanna", "Blixten McQueen"]

    names = ["Hasse", "Hanna", "Blixten McQueen"]
    
    names.pop(1)
    names # ["Hasse", "Blixten McQueen"]

## Loopa Genom Listor
De vanligaste sätten att loopa genom en lista kräver både en for loop.
Den första hämtar ut värden ur listan medan den andra hämtar positioner

    names = ["Hasse", "Hanna", "Blixten McQueen"]

    for name in names:
        print(name) # Hasse, Hanna, Blixten McQueen
    
    for i in range(len(names)):
        print(i) # 0, 1, 2