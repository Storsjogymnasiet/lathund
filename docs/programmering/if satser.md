---
weight: 4
---
# If Satser

## Vad Är En If Sats

När ett program grenar ut och utspelas annorlunda beroende på vad användaren mata in eller liknande så behöver vi något som dirigerar vidare. Det är if satser kommer in.

Programmet nedan släpper bara in användaren om deras ålder är 18 eller mer.

    age = input()
    age = int(age)

    if age >= 18:
        print("Välkommen in!")
    else:
        print("Kom tillbaka när du har växt upp")

Det är viktigt att all kod inuti varje gren är indenterad dvs skjutet 1 steg åt höger.

### Jämförelse Operatorer

Alla if satser behöver ett vilkor som bestämmer vilken gren i satsen som utspelas. Där kan man använda sig av en eller flera jämförelse operatorer för att bestämma vilkoret. Några vanliga operatorer är:

    == # Likamed
    != # Inte likamed
    > # Större än
    < # Mindre än
    >= # Större än eller likamed
    <= # Mindre än eller 

### elif
Om en if ska utspelas på fler än 2 sätt så kan man stacka flera elif för att få flera vilkor.

    print("Skriv in din ålder för att kolla om du har rätt till åkkort med nedsatt pris")
    age = input()
    age = int(age)

    if age < 6:
        print("Du åker gratis")
    elif age >= 6 and age <= 19:
        print("Du får åka med ett ungdomskort)
    elif age >= 65:
        print("Du får åka med ett seniorkort)
    else:
        print("Du har inte rätt till något nedsatt pris")