---
weight: 3
---
# Jobba i Projekt
För att flera ska kunna jobba i ett projekt / repo så rekommenderas det att skapa en branch för varje person eller en branch för varje ny feature.

## Skapa en branch
För att skapa en branch så behövs checkout commandet

    git checkout -b namn-på-nya-branch

## Pusha kod till branch

    # Se till att ni står i rätt branch
    git branch

    # om inte byt till rätt branch
    git checkout namn-på-branch

    # Sedan gör precis som vanligt

    git add .
    git commit -m "meddelande"
    git push origin namn-på-branch

## Merge kod till main
Jag rekommenderar att ni merge:ar via GitHub istället för commands

    # För att kunna merge:a koden till huvudbranchen så börjar ni med att hämta det senaste
    git pull origin main

    # Sedan byter ni till branchen som ni ska merge till
    git checkout main

    # Sen är det bara att merge:a
    git merge namn-på-branch
