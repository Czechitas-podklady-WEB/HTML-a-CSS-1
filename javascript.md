# Javascript

- Soubory s příponou `.js`
- Zapojení do stránky přes tag `<script>`
- `<script src="muj-script.js"></script>`
- Dodává stránce větší míru interaktivity
- Umí manipulovat s HTML i CSS

```js
const mujButton = document.querySelector('#muj-button')

const prepniSvetlo = () => {
	document.querySelector('body').classList.toggle('rozsviceno')
}

mujButton.addEventListener('click', prepniSvetlo)
```

- Online kurz [czechitas.cz/blog/online-kurz-javascript](https://www.czechitas.cz/blog/online-kurz-javascript)
