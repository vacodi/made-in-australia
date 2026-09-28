# Made in Australia badge

A small, original "Made in Australia" mark: the Southern Cross as five
sparkle stars, monochrome, using `currentColor` so it takes the colour of
whatever text sits next to it. Dedicated to the public domain (CC0) by
[Vacodi](https://vacodi.com) — use it on your own site, product or README,
no attribution required, no licence fee, no asking.

![Made in Australia](svg/made-in-australia.svg)

## Why this exists, and why it isn't *the* Australian Made logo

The green-and-gold kangaroo "Australian Made" logo is a registered
certification trademark owned by Australian Made Campaign Limited. It needs
a paid licence, an eligibility check, and is built for physical goods that
are grown, made or substantially transformed in Australia — not really a fit
for software. This badge is a completely different, original mark: nobody
owns it, nobody licenses it, and there is no eligibility test beyond it
being true.

## Use it

Two files, one icon each:

| File | What it is |
| --- | --- |
| `svg/made-in-australia.svg` | The full badge: mark + "Made in Australia" text, sized for a footer |
| `svg/made-in-australia-icon.svg` | The mark alone, for a compact spot (a favicon corner, an app's about screen) |

**Inline (recommended)** — copy the SVG's contents directly into your page
so it inherits your site's text colour and needs no network request:

```html
<a href="https://github.com/vacodi/made-in-australia" aria-label="Made in Australia">
  <!-- paste the contents of svg/made-in-australia.svg here -->
</a>
```

**Hosted**, if you'd rather not vendor the file (served from GitHub via
jsDelivr, cached, no build step):

```html
<img
  src="https://cdn.jsdelivr.net/gh/vacodi/made-in-australia@main/svg/made-in-australia.svg"
  alt="Made in Australia"
  height="24"
/>
```

The SVG has no fill colour baked in beyond `currentColor`, so wrap it in an
element with the text colour you want, or set `color` on the `<img>`'s
container (note: `currentColor` does not apply through an `<img>` tag —
inline the SVG if you need it to follow dark/light mode).

## Design notes

- Viewbox `0 0 40 40` for the icon, `0 0 <width> 24` for the badge with text,
  so it drops into a 24px-tall footer row without further scaling.
- Uses the system font stack for the label; swap `font-family` if you inline
  it and want your own type.
- No official symbol, flag artwork, coat of arms or state emblem is used or
  referenced — this is an original five-star sparkle arrangement evoking the
  Southern Cross, not a reproduction of the Australian flag or any
  government insignia.

## License

[CC0 1.0](LICENSE) — public domain. Do whatever you like with it.
