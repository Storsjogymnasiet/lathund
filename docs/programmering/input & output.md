---
weight: 3
---
# Input & Output

## Interaktion

För att skriva ut till terminalen och ta input från terminal så behövs print() och input() funktioner.

## print()
print() skriver till terminalen

    print("Hej värld!")
    print("4 + 4 är 8 tror jag")

### print() med variabler
Det går att printa variabler med hjälp av , eller fstring

    name = "Hasse"

    print("Hej", name)
    print(f"Hej {name}")

## input()
För att användaren ska styra programmet så används input() funktionen.
Alla variablar som skapas från input() blir en string.

    print("Skriv ditt namn")
    name = input()

    print(f"Hej {name}") # Hej namnet som användaren mata in

