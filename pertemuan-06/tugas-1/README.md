# Pertemuan 6 — Tugas 1: Dataset Point GeoJSON Jabodetabek

Titik pusat kota Jabodetabek dibuat di [geojson.io](https://geojson.io) dan diekspor sebagai GeoJSON, lalu dimasukkan ke QGIS (project `praktikum_qgis2`) di atas peta dasar Google Map, diekspor ke ESRI Shapefile, dan ditambah field `GDP` melalui Attribute Table.

| File | Keterangan |
|------|------------|
| [jabotabek.geojson](jabotabek.geojson) | Hasil ekspor geojson.io: 6 titik pusat kota (WGS 84 / EPSG:4326) |
| `jabotabek.*` | ESRI Shapefile hasil ekspor dari QGIS, sudah ditambah field `GDP` |
| [praktikum_qgis2.qgz](praktikum_qgis2.qgz) | Project QGIS (QGIS 4.2.3) |

## Atribut

| Kota | penduduk (ribu jiwa, 2024) | luas_km2 | GDP (triliun Rp, PDRB 2021) |
|------|---------------------------:|---------:|----------------------------:|
| Jakarta | 10684.95 | 660.98 | 3679.359 |
| Bogor | 1078.35 | 111.39 | 57.004 |
| Kota Tangerang | 1927.82 | 178.35 | 206.597 |
| Tangerang Selatan | 1429.53 | 164.86 | 104.388 |
| Depok | 2163.64 | 199.91 | 87.569 |
| Bekasi | 2644.06 | 213.12 | 118.963 |

Sumber: penduduk pertengahan 2024 dan luas wilayah dari BPS (via Wikipedia *Jakarta metropolitan area*); GDP dari Wikipedia *List of Indonesian cities by GDP*.
