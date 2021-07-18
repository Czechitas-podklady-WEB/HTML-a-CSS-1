# Box model

## Vlastnost `display`

- Základní `block`, `inline`, `inline-block`, `none`
- Každý element má výchozí typ
- Pomocí CSS lze měnit

### Blokové elementy

- Nadpisy, seznamy, odstavce, divy, strukturální prvky (header, footer, section)

  <div style="color:black;background-color:orange;">&lt;div&gt;každý zabere&lt;/div&gt;</div>
  <div style="color:black;background-color:cyan;">&lt;div&gt;celou dostupnou šířku&lt;/div&gt;</div>
  <div style="color:black;background-color:yellow;">&lt;div&gt;řadí se pod sebe&lt;/div&gt;</div>

### Řádkové elementy

- Nejsou samostatně na řádku => řadí se za sebou jako slova ve větě
- Nejde jim nastavit některé vlastnosti z box modelu (šířka, výška, horní/dolní margin)
- Odkazy, nebo důležitý text (`strong`)
- Ony jim ty vlastnosti nastavit jdou, ale neprojeví se očekávaným způsobem
- Lze ale například úspěšně nastavit pravý/levý margin
- Zaberou <span style="color:black;background-color:orange;">jen tolik </span><span style="color:black;background-color:cyan;padding:0 1em;">místa</span>, <span style="color:black;background-color:yellow;">kolik potřebují pro svůj obsah</span> a víc nic.

### Řádkově-blokové elementy

- Řádkový <span style="display:inline-block; color:black;background-color:orange;">hybrid</span> <span style="display:inline-block; color:black;background-color:cyan;padding:1em 0;">s některými</span> vlastnostmi blokového: <span style="display:inline-block; color:black;background-color:yellow;">řadí se za sebou,</span> ale lze mu nastavit šířku, výšku a okraje.

- Typicky se tak chovají obrázky

## Vlastnosti box modelu

### Rozměry

- `width`, `height`
- `min-width`, `min-height`
- `max-width`, `max-height`

  ```css
  img {
  	width: 300px;
  	max-width: 100%;
  }
  ```

- Vyhýbáme se omezování výšky, stránka je z principu na výšku nekonečná
- Využíváme procenta v kombinaci s explicitní hodnotou
- Responzivní/pružný obrázek

### Odsazení

- Vnitřní: `padding`
- Vnější: `margin`

  ```css
  p {
  	margin: 1rem 2rem 0.5rem 1.25rem;
  }
  ```

- `margin` může nabývat i záporných hodnot
- Lze psát jednotlivě pro strany boxu (top, right, bottom, left)
- Zkrácené vlastnosti:
  - 1 hodnota: všecky 4 strany shodně (`margin: 10px`)
  - 2 hodnoty: první nastavuje vertikální odszení, druhá horizontální (`margin: 10px 20px`)
  - 3 hodnoty: totéž co 2 hodnoty, třetí hodnota je spodní odsazení
  - 4 hodnoty: nastaví všechny strany po směru hodinových ručiček, počínaje top

### Ohraničení

- `border-width`
- `border-style`
- `border-color`
- `border: 1px solid aqua`
- `border-radius`
- Lze nastavit jednotlivé strany: `border-left: 3px solid silver;`
- Lze i nastavit konkrétní vlatnost ohraničení pro každou stranu: `border-right-width: 0;`
- I `border-radius` s jednou hodnotou je zkratka pro všecky rohy, lze je rozepsat
- `border-radius: 50%;` vytvoří vizuální kruh, ale prvek zůstává obdélníkem (čtvercem)!
- Více o `border-radius`: [Jak vytvořit ovál/elipsu](https://jecas.cz/oval), [oblé rohy na steriodech](https://jecas.cz/border-radius)
