# Google Material icons

Google LLC, Apache License 2.0 (see LICENSE).
Official SVG geometry is embedded in the shared `src/js/chartToolbar.js` with `fill="currentColor"` for offline and file:// use. Bar and stacked-bar icons are rotated 90 degrees to match horizontal charts.

Source repository: https://github.com/google/material-design-icons

- `tune_fill1.svg`: Google Material Icons Filled `tune`, geometria local de 24px, preenchimento inativo PATRI `#a6a6a6`; usado no rail de Configurações.

- `palette_fill1.svg`: official `symbols/web/palette/materialsymbolsoutlined/palette_fill1_24px.svg`, Material Symbols FILL=1. Geometry unchanged; local inactive fill is PATRI gray `#a6a6a6`.

The shared zoom in `src/js/chartControls.js` also embeds the Filled `src/content/remove/materialicons/24px.svg` and `src/content/add/materialicons/24px.svg` geometry, using `currentColor`. The glyphs are centered in the 24px viewBox.

- `src/editor/bar_chart/materialicons/24px.svg` — Filled
- `src/editor/show_chart/materialicons/24px.svg` — Filled
- `src/editor/pie_chart/materialicons/24px.svg` — Filled
- `src/action/donut_large/materialicons/24px.svg` — Filled
- `src/image/grid_on/materialicons/24px.svg` — Filled (heatmap representation)
- `symbols/web/stacked_bar_chart/materialsymbolsoutlined/stacked_bar_chart_fill1_24px.svg` — Material Symbols, FILL=1

The eight grouped chart selectors use the following official Material Symbols, all FILL=1:
`bar_chart`, `stacked_bar_chart`, `full_stacked_bar_chart`, `show_chart`, `area_chart`, `pie_chart`, `donut_large`, `view_quilt`, `bubble_chart`, `line_end_circle`, `device_thermostat`, `table_rows`.
The local `*_fill1.svg` files are unchanged upstream copies from
`https://raw.githubusercontent.com/google/material-design-icons/master/symbols/web/{name}/materialsymbolsoutlined/{name}_fill1_24px.svg`.
Their geometry is embedded in `chartToolbar.js`; horizontal variants rotate the vertical symbol 90 degrees.
`view_quilt` represents treemap, `line_end_circle` represents lollipop and `device_thermostat` represents heatmap, matching the user's reference.

The table's compact tools and sheet tabs use the same official FILL=1 sources:
`payments`, `percent`, `123`, `decimal_increase`, `decimal_decrease`, `content_paste_go`, `delete_sweep`, `table_view`, `add`, `close`.
They are loaded as local SVG images by `chartsGridTools.js`/`chartsPage.js`; no remote fonts or runtime requests to Google are required.

`pivot_table_chart_fill1.svg` (same upstream source pattern) now represents transposition in the table tools, replacing the paste button. Clipboard paste remains available through Ctrl+V and the native grid context menu.

`star_fill1.svg` and `label_fill1.svg` use the same official source pattern for the experimental item highlight and the Items rail. Item visibility reuses the existing `assets/icons/visibilidade.svg` and `visibilidade_off.svg` assets.
