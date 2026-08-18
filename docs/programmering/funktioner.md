---
weight: 6
---
# Variabler & Typer

## Funktioner 101

Funktioner är en färdigskriven block av kod som används för att minska repetition och göra koden lättare att läsa. Funktioner skriver ni bara 1 gång och sedan anropar (köra) varje gång ni behöver funktionen.

Det här är en funktion som hälsar på användaren.

    def greet():
        print("Hallå")

Sedan skriver man namnet av funktionen följt av paranteser för att köra den.

    greet() // printar Hallå
    print("Vad gör du?")

### Argument

Funktioner kan ta emot argument som den använder till sin uträkning. Nedan är en funktion som addera ihop 2 tal och sedan retunerar den tillbaka till där funktionen anropades.

    def add(x, y):
        return x + y
    
    sum = add(10, 5)
    print(sum) # printar 15
    
    sum = add(7, 3)
    print(sum) # printar 10

    # Om man vill så kan man förtydliga genom att skriva argumenten
    sum = add(x = 9, y = 3)
    print(sum) # printar 12


### Scope

Ett viktigt koncept till funktioner är **scope**. Alla funktioner har en egen scope vilket betyder att variablar skapad inuti en funktion excisterar endast där inuti.

    def example_function():
        random_variable = 10


    print(random_variable) # Kraschar då variabeln inte finns utanför funktionen

