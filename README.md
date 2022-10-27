[![JaneOri](https://img.shields.io/badge/JaneOri%20%F0%9F%91%BD-I%20made%20a%20thing!-blueviolet.svg?labelColor=222222)](https://twitter.com/Jane0ri)

# CSS-Peeps
One CSS file | One &lt;div> | 5 Million Open Peeps combinations | Infinite Customization

## Set up

CSS-Peeps only requires a single CSS file and is less than 1/10th of Twitter's max gif size.

### Install

`$ npm install css-peeps`

Then include `/node_modules/css-peeps/css-peeps.css`

### OR Use your favorite NPM CDN for small projects

From html:

```html
<link rel="stylesheet" type="text/css" href="https://unpkg.com/css-peeps@1/css-peeps.css">
```

or directly from your CSS:

```css
@import url(https://unpkg.com/css-peeps@1/css-peeps.css);
```

## Usage

Using the [Type Grinding](https://www.bitovi.com/blog/css-only-type-grinding-casting-tokens-into-useful-values) API where style variations are set from your CSS:

HTML:
```html
<div class="css-peeps"></div>
```

CSS:
```css
div {
  --peep-head: bangs1;
  --peep-face: talking;
  --peep-body: explaining;

  --peep-hat-color: #FC03C2;
  --peep-hair-color: #7300E6;
  --peep-skin-color: #87ceeb;
  --peep-accessory-color: #00ff00;
  --peep-facial-hair-color: #ffd700;
  --peep-object-color: #ffa500;
  --peep-clothes-color: #ff00c8;

  width: 317px;
  height: 343px;
}
```

Result:
![picture the css-peeps character displayed from the above code](https://i.imgur.com/3IAobKP.png)

Or, use the old school, backwards compatible API where style variants are all set from markup:

HTML:
```html
<div data-css-peeps="bangs1 talking explaining"></div>
```

CSS:
```css
div {
  --peep-hat-color: #FC03C2;
  --peep-hair-color: #7300E6;
  --peep-skin-color: #87ceeb;
  --peep-accessory-color: #00ff00;
  --peep-facial-hair-color: #ffd700;
  --peep-object-color: #ffa500;
  --peep-clothes-color: #ff00c8;

  width: 317px;
  height: 343px;
}
```

And the result is the same.

CSS-Peeps renders everything on the ::before and ::after pseudo elements, square and centered in the element, so you can still customize the element itself further with border, border-radius, backgrounds, etc.

### css-peeps.css vs css-peeps.compat.css

The main `css-peeps.css` file currently has a [global user reach of ~72.95%](https://caniuse.com/mdn-css_at-rules_property) and includes both the [Type Grinding](https://www.bitovi.com/blog/css-only-type-grinding-casting-tokens-into-useful-values) API and the classic backwards compatible [data-attr](https://elisehe.in/2022/10/16/attribute-selectors) API.

For the largest user reach [(<b>~92.33%</b> of global users)](https://caniuse.com/mdn-css_selectors_where), include the compatibility-focused API `css-peeps.compat.css` instead of `css-peeps.css` but you'll lose the Type Grinding API (data-attr API only).

## Links

[Online CSS-Peeps WYSIWYG Builder](https://css-peeps.com)

[CSS-Peeps Documentation](https://css-peeps.com/#docs)

[Leave a star for CSS-Peeps on github!](https://github.com/propjockey/css-peeps)

[Follow the author, Jane Ori, on twitter!](https://twitter.com/Jane0ri)

[CSS-Peeps on npm](https://www.npmjs.com/package/css-peeps)

[CSS-Peeps is free and open source with the BSD-2-Clause license](https://opensource.org/licenses/BSD-2-Clause)

---

Original black & white SVG character line drawings by [Open Peeps](https://www.openpeeps.com/)

Open Peeps license: [CC0 License](https://creativecommons.org/publicdomain/zero/1.0/)

## Supporting CSS-Peeps

[Through paypal](https://www.paypal.com/donate/?hosted_button_id=9Z925L3SJJ8BS)
([augmented-ui](https://augmented-ui.com) is another library from Jane @ PropJockey)

BTC address:
bc1qe2ss8hvmskcxpmk046msrjpmy9qults2yusgn9

XRP address + tag:
rw2ciyaNshpHe7bCHo4bRWq6pqqynnWKQg + 459777128

ETH address:
0x674D4191dEBf9793e743D21a4B8c4cf1cC3beF54
