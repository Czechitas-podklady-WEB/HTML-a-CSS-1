# Responzivní design

## Fixní layout

- Již dlouho překonaný styl
- Fixní = statický
- Většina elementů je v px
- Elementy se po stránce nepohybují
- Nezáleží na velikosti obrazovky

<img src="https://miro.medium.com/max/2000/1*dUZudP2xfPLzMiw5L8ieTQ.gif" style="max-height: 180vh;" />

## Fluidní layout

- Stále hodně používaný i když překonaný
- Většina velikostí je zapsána v %
- Elementy se po stránce nepohybují
- Záleží na velikosti obrazovky
- Není vhodný pro mobilní zařízení

<img src="https://miro.medium.com/max/2000/1*Hul4o5D73lpzVeVTk2Cuag.gif" style="max-height: 180vh;" />

## Adaptivní layout

- Před media queries asi nejpoužívanější
- Pro každou velikost definovaná verze
- Elementy už se na stránce pohybují
- Záleží na velikosti obrazovky
- Zbytečný kód pro každou verzi

<img src="https://miro.medium.com/max/2000/1*LP6jyJPC17EVOk8nKEHYzg.gif" style="max-height: 180vh;" />

## Responzivní layout

- Bere si to nejlepší z fluidního a adaptivního
- Používají se breakpointy media-queries
- Rozděluje rozlišení do rozmezí
- Elementy se přesouvají, mění pozici i velikost
- Minimalizuje zdrojový kód

<img src="https://miro.medium.com/max/2000/1*jGg5Y0CIZSGSTDTabsarbQ.gif" style="max-height: 180vh;" />

## Mobile first

<img src="https://content.altexsoft.com/media/2017/04/mobile-first-design-1024x404.png" style="max-height: 130vh;" />

## Media queries / breakpointy

<img src="https://www.vzhurudolu.cz/prirucka-content/dist/images/original/media-query.jpg" style="max-height: 130vh;" />

## Media queries / breakpointy

- Typ média - screen, all, print, only
- Logické operátory - and, (or = ,)
- Vlastnost média - min-width, max-width, atd.
- Hodnota zlomu - px, em

## Nejpoužívanější queries

- `@media (min-width: 1025px) { … }`
- `@media (min-width: 768px) and (max-width: 1025px) { … }`
- `@media (max-width: 767px) { … }`

## Cvičení 1

- [github.com/Czechitas-podklady-WEB/Cviceni-Media-query-banner](https://github.com/Czechitas-podklady-WEB/Cviceni-Media-query-banner)

## Cvičení 2

- [github.com/Czechitas-podklady-WEB/Cviceni-Media-query-sloupce](https://github.com/Czechitas-podklady-WEB/Cviceni-Media-query-sloupce)

## Cvičení 3

- [github.com/Czechitas-podklady-WEB/Cviceni-Media-query-galerie](https://github.com/Czechitas-podklady-WEB/Cviceni-Media-query-galerie)

## Cvičení 4

- Miniprojekt
- [github.com/Czechitas-podklady-WEB/Cviceni-Recepty](https://github.com/Czechitas-podklady-WEB/Cviceni-Recepty)
