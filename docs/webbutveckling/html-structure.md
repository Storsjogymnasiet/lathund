# Hur en HTML-fil är uppbyggd

HTML (*Hypertext Markup Language*) är ett språk som används för att strukturera innehållet på en hemsida. 

En HTML-fil sparas med filtillägget `.html`.

## Grundläggande struktur

Varje HTML-fil börjar med en deklaration som berättar att dokumentet är HTML:

```html
<!DOCTYPE html>
```

Sedan kommer hela dokumentet inneslutet i taggen `<html>`, som berättar att allt innehåll ligger i ett HTML-dokument.

```html
<!DOCTYPE html>
<html>

</html>
```

## `<head>` och `<body>`

En HTML-fil delas oftast in i två huvuddelar:

- `<head>`: innehåller information om sidan, till exempel titel och länkar till CSS-filer.
- `<body>`: innehåller allt som användaren kan se på sidan.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Min första hemsida</title>
  </head>
  <body>
    <h1>Hej världen!</h1>
    <p>Detta är en paragraf.</p>
  </body>
</html>
```

## Vad betyder det?

- `<!DOCTYPE html>` säger att dokumentet är HTML5.
- `<html>` startar HTML-dokumentet.
- `<head>` innehåller metadata och inställningar.
- `<title>` visar texten i webbläsarens flik.
- `<body>` innehåller det som visas på sidan.
- `<h1>` är en rubrik.
- `<p>` är ett stycke text.

## Exempel med lite mer innehåll

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Min sida</title>
  </head>
  <body>
    <h1>Välkommen till min sida</h1>
    <p>Här skriver jag text som alla ska kunna läsa.</p>
    <a href="https://example.com">Länk till exempel</a>
  </body>
</html>
```

## Viktigt att komma ihåg

- HTML beskriver struktur, inte utseende.
- Alla taggar ska oftast ha en start- och sluttag, till exempel `<p>text</p>`.
- Taggar kan ligga i olika nivåer, som i ett träd:

```html
<div>
  <h1>Rubrik</h1>
  <p>Text</p>
</div>
```

## Sammanfattning

En HTML-fil är grunden för alla hemsidor. Den beskriver vad som finns på sidan, men inte hur den ser ut.

En vanlig HTML-fil byggs upp så här:

1. `<!DOCTYPE html>` berättar att det är en HTML5-fil.
2. `<html>` börjar själva dokumentet.
3. `<head>` innehåller information om sidan, till exempel titel och teckenkod.
4. `<body>` innehåller allt som användaren ser på hemsidan.
5. Innehållet i kroppen kan vara rubriker, text, länkar, bilder, listor mm.

Kort sagt: HTML bestämmer innehållet, medan CSS bestämmer utseendet.
