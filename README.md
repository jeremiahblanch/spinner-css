# spinner-css

Simple CSS only spinner configurable with CSS variables.

# Usage

1. Install from npm

```
npm i spinner-css
```

2. Ensure the CSS is referenced in your project

```html
<link rel="stylesheet" href="node-modules/spinner-css/spinner.css" />
```

3. Put the class `spinner-css` on an element:

```html
<div class="spinner-css"></div>
```

## Configuration

Use the CSS variables! By default these are the values:

```CSS
:root {
  --spinner-css-color: #000;
  --spinner-css-duration: 1s;
  --spinner-css-position: fixed;
  --spinner-css-size: 2rem;
  --spinner-css-thickness: 0.25rem;
}
```

If you want to override the values, just use more specific CSS eg with a container, `body` or the spinner itself, eg

```CSS
.spinner-css {
  --spinner-css-color: coral;
  --spinner-css-duration: 3s;
  --spinner-css-size: 12rem;
  --spinner-css-thickness: 1rem;
}
```

### Position: `fixed` or `absolute`

By default the spinner is `position:fixed` so it is centered on the window. You can set it to `absolute` so that it sits within a container:

```CSS
.spinner-css {
  --spinner-css-position: absolute;
}
```

**Be sure to set the container to be `position: relative`!**

## Example

Open [the demo](//jeremiahblanch.github.io/spinner-css) and see how simple it is.

## Browser support

IE10+ and all the modern browsers

## License

[MIT](LICENSE)
