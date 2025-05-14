# Simple Online Clock on GitHub Pages

Simple customisable online clock (on GitHub Pages) which can be configured through query parameters. Optimised for the OBS Studio "browser" source type.

Taken from https://obsproject.com/forum/resources/time-and-date-overlay-updated.1461/ with query params inspired by https://github.com/pablopunk/time?tab=readme-ov-file.

- `fg`: Font colour
- `bg`: Background colour

- `font`: Font family

- `fontSize`: The size of the font in the clock

- `position`: Position on the screen. Defaults to `center`

```
top-left      top       top-right
left                        right
bottom-left  bottom  bottom-right
```

- `format`: _Moment.js_ [format string](https://momentjs.com/docs/?/displaying/format/#/parsing/string-format/)

---

Parameters can be passed either in the query string:

https://windows81.github.io/Simple-Online-Clock-on-Pages/?font=Inconsolata&fg=white&format=YYYY-MM-DD%20HH:mm:ss:SS

Or as _Custom CSS_:

```css
props {
--font: Inconsolata;
--fg: white;
--format: YYYY-MM-DD HH:mm:ss:SS;
}
```
