---
weight: 8
---
# Felhantering

## Kod som förebygger fel

När du programmerar är det viktigt att skriva kod som klarar av oväntade situationer utan att programmet kraschar. Ett program som avslutas plötsligt är frustrerande för användaren och svårt att felsöka för utvecklaren.

## Try Except

try except testar att köra kod och om koden kraschar eller något går fel så försöker den hantera felet istället för att stängas av.

    try:
        print(0 / 0)
    except:
        print("Error! Du får inte dela med 0.")

En vanlig användning av try except är när man ska casta en variabel.

    number = input("Skriv in ett nummer")
    
    try:
        number = int(number)
    except:
        print("Error! Skriv endast in nummer.")

## Validering

Om det går att validera data innan den används är det ofta ett bättre sätt att förebygga fel än att enbart förlita sig på try/except.

    x = 10
    y = 0

    if y == 0:
        print("Error! Du får inte dela med 0.")
    else:
        print(x/y)