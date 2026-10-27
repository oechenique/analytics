# legacy/

Original notebooks of this repo (2023–2024), kept untouched. Replaced by [`notebooks/01_caba_subway_apartments.ipynb`](../notebooks/01_caba_subway_apartments.ipynb).

| File | What it was |
|---|---|
| `gis_analytics.ipynb` | Properati listings in Buenos Aires, apartments within "800 m" of Congreso de Tucumán station. It ran in 2023 (outputs kept), but the 800 m buffer was drawn in degrees (`0.0072°`), which at 34.6°S is an ellipse of ~800 × 660 m, and the price heatmap mixed ARS and USD per m². Today it also depends on the INDEC WFS (not responding on 2026-10-27) and `mpl_toolkits.basemap`. |
| `01_getting_started_with_geoDataFrames.ipynb` | Kyoto temples. Draft, never executed. Uses `ox.geometries_from_place` (removed in osmnx 2). |
| `02_spatial_operations_with_geoDataFrames.ipynb` | Tokyo transit. Draft, never executed. Uses the old `graph_from_bbox` signature and `momepy.clusters`, which does not exist. |
| `03_advanced_spatial_analysis.ipynb` | Japanese metro demographics. Draft, never executed: reads an e-Stat web page as if it were a file and defines functions that are never called. |
| `data/geoanalytics.png` | The 2023 heatmap (the ellipse is visible). |

Also removed from the tree: `temp5.geojson` (INDEC provinces, an intermediate file), `geoanalytics.html` (Plotly export) and the osmnx `cache/`. The listings zip moved to [`data/`](../data/).
