# Simple Online Clock on GitHub Pages

Simple customisable online clock (on GitHub Pages) which can be configured through query parameters. Optimised for the OBS Studio "browser" source type.

Taken from [Chessset5's browser overlay](https://obsproject.com/forum/resources/time-and-date-overlay-updated.1461/) with query params inspired by [pablopunk/time](https://github.com/pablopunk/time?tab=readme-ov-file).

- `fg`: Foreground colour

  - defaults to `white`

- `bg`: Page-wide background colour

  - defaults to `black`

- `box`: Text-box padding colour

  - defaults to `transparent`

- `font`: Font family

  - defaults to `sans-serif`

- `fontSize`: The size of the font in the clock

- `position`: Position on the screen

  - defaults to `center`

- `bpad`: Text-box padding width

- `brad`: Text-box border radius

```
top-left      top       top-right
left                        right
bottom-left  bottom  bottom-right
```

- `format`: _Moment.js_ [format string](https://momentjs.com/docs/?/displaying/format/#/parsing/string-format/)

- `offsetMs`: Number of milliseconds to add to the current UTC.

  - defaults to your local time-zone offset

- `useOnline`: If `true`, extracts the current time from a remote server upon page load.

  - defaults to `false`

---

Parameters can be passed either in the query string:

https://windows81.github.io/Simple-Online-Clock-on-Pages/?font=Inconsolata&fg=white&format=YYYY-MM-DD%20HH:mm:ss:SS

Or as _Custom CSS_ in an instance of OBS Studio's _Browser_ source:

```css
props {
--font: Inconsolata;
--fg: white;
--format: YYYY-MM-DD HH:mm:ss:SS;
}
```

The underlying HTML structure is the same as in [Chessset5's version](https://obsproject.com/forum/resources/time-and-date-overlay-updated.1461/). So any existing custom CSS should work as-is.
