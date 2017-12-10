[![NPM](https://nodei.co/npm/prepend-react-dom.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/prepend-react-dom/)

# prependReactDOM

Prepend React DOM Node to an element.

## Installation

```bash
npm install prepend-react-dom --save
```

## Usage

```html
<div class="list">
	<div class="item item-1">item 1</div>
</div>
```

```js
import prependReactDOM from 'prepend-react-dom';
import ItemComponent from 'components/Item';

let el = document.querySelector('.list');

prependReactDOM(ItemComponent, el, {
	bar: 'bar',
	foo: 'foo'
});
```

Now the list become:

```html
<div class="list">
	<div data-reactroot class="item item-2">item 2</div>
	<div class="item item-1">item 1</div>
</div>
```

---

Copyright &copy; 2017 Sabri El Gueder.
