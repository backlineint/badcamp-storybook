# Generic Drupal Web Components

Inspired by [@generic-components/components](https://www.npmjs.com/package/@generic-components/components) this project aims to create a library of generic web components that are accessible, framework agnostic, possible to style, and easy to use with data provided by [Drupal](https://www.drupal.org).

## Usage

### Via NPM
Components can be installed via NPM (View [example on Codesandbox](https://codesandbox.io/s/gdwc-import-joowy)):

```bash
npm i @gdwc/components
```

And imported in your code via ES imports:

```js
import '@gdwc/components/menu';
```

### Via CDN
Alternatively you can load the components from a CDN and drop them in your HTML file as a script tag. (View [example on Codepen](https://codepen.io/brianperry/pen/QWdyONQ))

```html
<script type="module">
  import gdwcComponents from 'https://cdn.skypack.dev/@gdwc/components';
</script>
```

```html
<gdwc-menu branding="Menu Heading" baseUrl="https://decoupled-menus.jsonapi.dev" menuId="main"></gdwc-menu>
```

## Guiding Principles
* It should be easy to use these web components in decoupled Drupal projects with JSON:API data provided by Drupal Core.
* It should also be possible to use these same components within Drupal's traditional Twig based templating engine.
* While additional components may be contributed, this project will primarily focus on creating components following along with [related strategic Drupal initiatives](https://www.drupal.org/project/decoupled_menus_initiative).