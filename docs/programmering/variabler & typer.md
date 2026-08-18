---
weight: 1
---
# Variabler & Typer

## Variabler 101

En variabel är en sorts kontainer som sparar data inuti. Variabler används för att hantera & manipulera data. Största fördelen med variabler är att de hanterar datorns RAM minne automatiskt.

Alla variabler har ett namn, en typ och ett värde. När vi skapar en variabel så måste vi ge den ett namn. I python så delas typer ut automatiskt och ett värde är valfritt.

    empty_variable
    name = "Hassan"
    age = 55
    phone_number = "0978-9986705"

Ovan är flera variabler med olika värden, observera att *empty_variable* inte har något värde.

## Namngivning

När det kommer till namngivning av variabler så har python några regler.
{{% steps %}}

1. Namnet måste börja på en bokstav eller ett understreck

2. Namnet får bara innehålla vanliga bokstäver och understreck (A-z, 0-9, och _ )

3. Namnet får inte innehålla någon av pythons reserverade ord

4. Namnet ska vara i stora bokstäver om värdet är konstant (ändras inte)

{{% /steps %}}

    ✅ male_name = "Hassan"
    ✅ home_address = "Storvägen 13"
    ✅ PI = 3.14159
    ✅ MEANING_OF_LIFE = 42
    ✅ number_2 = 22

    ❌ MAle NaME = "Hassan"
    ❌ 2number = 22
    ❌ home address = "Storvägen 13"
    ❌ variabel_på_svenska = 67


## Typer

Variabler kan innehålla olika sorters data, såsom siffror eller text. För att datorn ska veta hur informationen ska bearbetas används typer.

Utan en bestämd typ vet datorn inte om instruktionen 2 + 2 ska tolkas som:

    Matematik: 2 + 2 = 4 (int)
    Sammansättning: 2 + 2 = 22 (string)

Genom att tilldela en typ förstår datorn exakt hur den ska hantera och tolka innehållet i variabeln.

### Vanliga Typer

| Typ | Beskrivning | Exempel |
|-----|-------------|---------|
| **int** (heltal) | Tal utan decimaler. Används för att räkna eller iterera | `5`, `-12`, `2025` |
| **float** | Tal med decimaler. Används vid mer noggrann matematik. | `3.14`, `0.5`, `-12.75` |
| **str** (string/sträng) | Text, alltid inom `' '` eller `" "`. | `"Hej"`, `'Python'`, `"123"` |
| **bool** (boolean) | Sant eller falskt. Ofta resultat av jämförelser. | `True`, `False`, `5 > 2` |
| **list** (lista) | En samling av värden som kan ändras. | `[1, 2, 3]`, `["a", "b"]`, `[True, False]` |
| **dict** (dictionary) | Samling av nyckel–värde-par. Bra för strukturerad data. | `{"name": "Anna"}`, `{"age": 14}`, `{"x": 10, "y": 20}` |
| **none** | Ingenting. Undvik helst | `None` |

### Casting

Casting används för att ändra typen på en variabel

    ✅ x = "10" # x börjar som en string
    ✅ x = int(x) # x blir castad till en int

    ✅ y = 55 # y börjar som en int
    ✅ y = "55" # y blir castad till en string

OBS!
Casta inte en variabel som har ett värde som inte går att representera med den typen.

    ❌ x = "Hasse"
    ❌ x = int(x) # "Hasse" är inte ett heltal så då kraschar programmet