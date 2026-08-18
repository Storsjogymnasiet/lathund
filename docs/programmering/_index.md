---
weight: 1
bookFlatSection: true
title: "Programmering"
---

# Introduktion

## Programmering 101

I den här programmeringskursen kommer ni att lära er hur man skriver program som styr datorer. Dagens datorer är väldigt snabba och smarta, men de behöver tydliga instruktioner för att veta vad de ska göra.

Ni kommer att arbeta med programmeringsspråket Python och främst skapa mindre program som löser enkla uppgifter.

## Python

Python är en av världens mest populära programmeringsspråk som är ett vanligt val när man vill lära sig programmering. Med python kan man göra allt från att skriva små skripts till att bygga en egen ai. Nedan är en bit kod tagen från ett program som verifierar personnummer.

    id = "8112189876"
    numbers = ""
    number_total = 0
    control_number = 0

    for i in range(len(id) - 1):
        if(i % 2 == 0):
            numbers += str(int(id[i]) * 2)
        else:
            numbers += id[i]

    for num in numbers:
        number_total += int(num)

    control_number = (10 -(number_total % 10)) % 10