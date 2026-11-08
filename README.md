# Apps d'estudi

Aplicacions web per estudiar i preparar exàmens des del mòbil.

## Estructura

```
index.html                      ← índex de temes (pàgina d'entrada)
historia/
  revolucio-industrial.html     ← La Revolució Industrial
```

## Afegir un tema nou

1. Desa l'arxiu `.html` del tema a la carpeta de l'assignatura (crea-la si no existeix, p. ex. `geografia/`).
2. Obre `index.html` i afegeix una entrada a la llista `TEMES`:

```js
{
  assignatura: "Història",
  titol: "Les revolucions liberals",
  descripcio: "Breu descripció del que conté.",
  url: "historia/revolucions-liberals.html",
  curs: "",      // opcional
  ordre: 2,      // ordre dins l'assignatura
  nou: true      // opcional: mostra l'etiqueta "Nou"
}
```

3. Si l'app del tema ha de tenir el botó «Índex», posa a la capçalera un enllaç a `../index.html`.

Quan hi hagi més d'una assignatura, l'índex mostra automàticament els filtres per assignatura.

## Publicar amb GitHub Pages

Settings › Pages › Source: *Deploy from a branch* › Branch `main`, carpeta `/ (root)`.
