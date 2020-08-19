[![Actions Status](https://github.com/UziTech/atom-modal-views/workflows/tests/badge.svg)](https://github.com/UziTech/atom-modal-views/actions)
[![Dependency Status](https://david-dm.org/UziTech/atom-modal-views.svg)](https://david-dm.org/UziTech/atom-modal-views)

# atom-modal-views

Modal Input Views for Atom packages

## InputView

Single line input view

### Usage

```js
const { InputView } = require("atom-modal-views");

const inputView = new InputView({
	title: "Title text",
	description: "Description can use **markdown**",
	placeholder: "placeholder text",
	value: "initial value",
});

const value = await inputView.getInput();
```

### Options

| Name        | Default | Description                                  |
|:------------|:-------:|:---------------------------------------------|
| title       |   `""`  | Title inside `<h1>` tag                      |
| description |   `""`  | Description can contain markdown             |
| placeholder |   `""`  | Placeholder text to show when input is empty |
| value       |   `""`  | The initial value                            |
