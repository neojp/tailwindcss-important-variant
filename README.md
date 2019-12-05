<p align="center">
    <a href="https://tailwindcss.com/" target="_blank"><img width="200" src="https://tailwindcss.com/img/tailwind.svg"></a><br>
    A utility-first CSS framework for rapidly building custom user interfaces.
</p>

---

<br>

# Tailwind CSS `!important` variant

This is a Tailwind CSS plugin that adds an `!important` variant.

Maintained by: [Joan Piedra](https://joanpiedra.com) → [@neojp](https://twitter.com/neojp)

## Installation

Install as a node module with either `npm` or `yarn` on your command line

```bash
# Install via npm
npm install --save-dev @neojp/tailwindcss-important-variant

# Install via yarn
yarn add --dev @neojp/tailwindcss-important-variant
```

Add this module as a plugin on your [Tailwind configuration file](https://tailwindcss.com/docs/configuration#plugins) (`tailwind.config.js`).

```js
module.exports = {
  plugins: [
      require('@neojp/tailwindcss-important-variant')
  ]
};
```

Use this plugin in your list of [variants](https://tailwindcss.com/docs/configuring-variants), either globally

```js
module.exports = {
  variants: ['responsive', 'important']
};
```

Or per utility:

```js
module.exports = {
  variants: {
    borderRadius: ['responsive', 'important']
  }
};
```

## Usage

Use your Tailwind utility classes with an exclamation mark ( `!` ) as a suffix.

```html
<div class="rounded!"></div>
```

## Output

Tailwind will be outputed as follows.

```css
.rounded\! {
  border-radius: 0.25rem !important
}
```

## Contributing

Feel free to submit a PR request, and send me a message on Twitter ([@neojp](https://twitter.com/neojp)) about it.

## License
This project has been licensed under [the Hippocratic License](https://firstdonoharm.dev/).