---
weight: 4
---
# Loopar

## om och om och om och om

Loopar används när man vill att koden ska upprepa sig flera gånger om utan att skriva samma kod flera gånger.

## For Loop

For loopar används när man vill loopa genom något som har en bestämt längd, som bokstäver i en mening eller element i en lista.
Koden nedan loopar genom alla bokstäver i meningen och printar ut varje bokstav

    for letter in "en mening med flera ord":
        print(letter)
    
    # printar
    # e
    # n
    # 
    # m
    # e
    # osv.....

### For i in range()
Ibland så vill man loopa ett x antal gånger eller loopa genom något och plocka ut positioner istället för självaste värdet. Då kan man använda sig av en såkallad **for i in range() loop**.

    for i in range(5):
        #loopar 5 gånger
    
    fruits = ["äpple", "banan", "melon"]

    for i in range(len(fruits)):
        print(fruits[i]) # printar alla frukter med hjälp av position

## While loop
While loopar används när man vill loopa men inte vet hur många gånger i förväg, som att fortsätta äta tills man blir mätt eller fortsätta vänta till bussen har kommit.

    while hungry:
        eat()
    
    x = 0
    while x > 5:
        x++


## Break
break används för att avsluta loopar tidigt.
Koden nedan loopar genom listan med namn för att hitta vilken position som Hasse har.

    names = ["Mikael", "Sara", "Hasse", "Pippi"]
    position = 0
    for i in range(len(names)):
        if names[i] == "Hasse":
            position = i
            break

## Continue
Använd continue för att avbryta den nuvarande iterationen i en loop och direkt hoppa till nästa. Koden nedan loopar genom och printar ut alla namn förrutom Sara.

    names = ["Mikael", "Sara", "Hasse", "Pippi"]
    for name in names:
        if name == "Sara":
            continue

        print(name)