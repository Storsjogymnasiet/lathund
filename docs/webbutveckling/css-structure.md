# Hur en CSS-fil är uppbyggd

CSS (*Cascading Style Sheets*) är ett språk som används för att styla en hemsida. Det är CSS som bestämmer färger, textstorlek, marginaler, placering och mycket mer.

En CSS-fil sparas med filtillägget `.css`.

## Grundläggande struktur

En CSS-fil består av regler. Varje regel innehåller en selector och ett block med egenskaper.

```css
p {
  color: blue;
  font-size: 18px;
}
```

Det här betyder:

- `p` är väljaren, alltså vilken HTML-tag som ska påverkas.
- `{ ... }` är regeln där vi skriver styling.
- `color: blue;` ändrar textfärgen.
- `font-size: 18px;` ändrar textstorleken.

## Hur CSS fungerar

CSS kopplas oftast till HTML med hjälp av en länk i `<head>`:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Min sida</title>
    <link rel="stylesheet" href="style.css" /> <-- här!
  </head>
  <body>
    <p>Hej! Jag är stylad med CSS.</p>
  </body>
</html>
```

Och i filen `style.css` kan vi skriva:

```css
p {
  color: green;
  font-size: 20px;
}
```

Nu blir texten i paragrafen grön och lite större.

## Vanliga CSS-egenskaper

Här är några vanliga saker som CSS kan ändra:

```css
h1 {
  color: red;
  font-size: 32px;
  text-align: center;
}

p {
  color: black;
  font-size: 18px;
}
```

Detta betyder att:

- `color` ändrar färgen
- `font-size` ändrar storleken
- `text-align` centrerar eller justerar texten

## Selektorer

CSS använder selektorer för att välja vilka element som ska påverkas.

### Elementselector

```css
p {
  color: blue;
}
```

Det här påverkar alla `<p>`-taggar.

### Klassselector

```css
.klassnamn {
  background-color: yellow;
}
```

Det här påverkar alla element som har klassen `klassnamn` i HTML.

```html
<p class="klassnamn">Detta är en stylad paragraf.</p>
```

### ID-selector

```css
#rubrik {
  color: purple;
}
```

Det här påverkar ett enda element med id:t `rubrik`.

```html
<h1 id="rubrik">Min rubrik</h1>
```

## Exempel med hela dokumentet

HTML:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Exempel</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1 class="rubrik">Välkommen</h1>
    <p class="text">Det här är text på sidan.</p>
  </body>
</html>
```

CSS:

```css
.rubrik {
  color: darkblue;
  font-size: 36px;
  text-align: center;
}

.text {
  color: gray;
  font-size: 18px;
}
```

## Viktigt att komma ihåg

- CSS styr hur sidan ser ut.
- CSS arbetar med regler och selektorer.
- Ett element kan ha flera egenskaper i samma CSS-block.
- Varje egenskap avslutas med semikolon `;`.

## Sammanfattning

En CSS-fil är där vi skriver regler som bestämmer utseendet på webbsidan. Den väljer element i HTML och ändrar saker som färg, storlek, avstånd och placering.

Kort sagt:

- HTML = innehåll
- CSS = stil

Tillsammans gör de en hemsida snygg och lätt att läsa.
