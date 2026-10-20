# Pertemuan 5 — Tugas 1: Import Polygon KML ke QGIS

Praktikum terbimbing Aplikasi Quantum GIS 1. Project QGIS `praktikum_sig1` berisi peta dasar dari XYZ Tiles (OpenStreetMap dan Google Map) serta area polygon DKI Jakarta yang diimpor dari file KML menggunakan plugin KML Tools, lalu diekspor ke ESRI Shapefile.

| File | Keterangan |
|------|------------|
| [praktikum_sig1.qgz](praktikum_sig1.qgz) | Project QGIS (QGIS 4.2.3) |
| [wilayah-dki-jakarta.kml](wilayah-dki-jakarta.kml) | Data input: polygon wilayah daratan DKI Jakarta (WGS 84 / EPSG:4326) |
| `wilayah_dki_jakarta.*` | Hasil ekspor ESRI Shapefile (`.shp`, `.shx`, `.dbf`, `.prj`, `.cpg`, `.qmd`) |

## Sumber Peta (XYZ Tiles)

| Nama | URL |
|------|-----|
| OpenStreetMap | `https://tile.openstreetmap.org/{z}/{x}/{y}.png` |
| Google Map | `https://mt1.google.com/vt/lyrs=r&x={x}&y={y}&z={z}` |
| Google Hybrid | `http://mt0.google.com/vt/lyrs=y&hl=en&x={x}&y={y}&z={z}` |
| Google Map Satellite | `http://www.google.cn/maps/vt?lyrs=s@189&gl=cn&x={x}&y={y}&z={z}` |
| Google Road | `https://mt1.google.com/vt/lyrs=h&x={x}&y={y}&z={z}` |
| Google Terrain | `https://mt1.google.com/vt/lyrs=p&x={x}&y={y}&z={z}` |
| Arcgis Map | `https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}` |
