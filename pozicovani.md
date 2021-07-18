# Pozicování

![CSS Position Property](https://miro.medium.com/max/2000/1*8OQ7qwYSCuVVwGFTC82KrQ.png)

<small>Credit for [Geronimo Morisot Morla
](https://medium.com/@geromorla/css-position-property-starters-guide-3602431df059)</small>

# Vlastnost `position`

- Říkáme jak má být prvek na stránce umístěný

## Position: `static`

- Mají implicitně všechny prvky
- Prvek se zobrazí tam, kde na něj vyjde řada

## Position: `relative`

- Prvek posunu relativně vůči jeho výchozí pozici, zabírá své původní místo
- Vlastnosti `top`, `left`, `right`, `bottom` určují posun vůči výchozí pozici
- Vybírám si hranu, v jejímž směru posouvám
- Záporná hodnota posouvá v opačném směru

## Position: `absolute`

- Prvek zcela vyjme z toku dokumentu a lze jej libovolně umístit
- Pozicuje se vzhledem ke svému nejbližšímu rodiči který nemá `position: static`
- Pokud takový rodič neexistuje, pozicuje se vůči stránce

## Vzájemné překrývání prvků

- Standardní pořadí, jak jsou v dokumentu
- Prvky které nemají `position: static` jsou ve vrstvě nahoře
- Lze řídit přes vlastnost [z-index](https://developer.mozilla.org/en-US/docs/Web/CSS/z-index)

## Position: `fixed`

- Zůstává na obrazovce i když posouváme stránkou/scrollujeme
- Zabírá použitelný prostor na obrazovce
- Pozor na mobily!

## Position: `sticky`

- Kombinace static a fixed
- Prvek se posouvá tak, aby byl vidět uvnitř svého rodiče
