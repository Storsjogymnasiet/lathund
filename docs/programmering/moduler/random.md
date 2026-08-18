# Random
Random används till allting som slumpas. Nedan är ett utval av de vanligaste metoderna.

## randint(a, b)
randint() slumpar fram ett nummer inom ett viss omfång.

    random.randint(1,10) # 7
    random.randint(1,10) # 4
    random.randint(1,10) # 2

## shuffle()
shuffle() slumpar ordningen i en lista.

    numbers = [1, 2, 3, 4]
    random.shuffle(numbers)
    print(numbers) # 3, 2, 4, 1

## choice()
choice() slump väljer ett item i en lista.

    fruits = ["banana", "melon", "kiwi"]
    random.choice(fruits) # "melon"