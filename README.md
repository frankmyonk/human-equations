# Human Equations

Interactive world map of every *Homo* species from 2.8 million years ago to the present: range waves, ice sheets, sea-level coastlines, sapiens–Neanderthal–Denisovan contact zones, and brain-size and stature trends. One self-contained HTML page.

Open `index.html` in a browser (it loads D3 and topojson from cdnjs).

## Rebuild

```
python3 src/build.py
```

`src/page.html` (layout and CSS), `src/data.js` (species, range paths, sites, contact events) and `src/app.js` (rendering) are inlined together with `data/` into `homo-atlas.html`.

## Notes

- Ranges are schematic, drawn from fossil, archaeological and ancient-DNA evidence published up to 2025. Sea level and ice extent are approximations.
- Elevation grid: NOAA ETOPO 2022 sampled at 0.5° (`data/elev.b64`, 8-bit, −300 to +60 m). Coastlines: Natural Earth via `world-atlas` 50 m.
