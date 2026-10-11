# Pertemuan 4 — Tugas 1: Taman Kota Jakarta

Data poligon ruang terbuka hijau (taman kota) di DKI Jakarta. Setiap taman tersedia dalam dua format: CSV dengan geometri `POLYGON` dalam format WKT (CRS: WGS 84 / EPSG:4326) yang dapat dimuat di QGIS sebagai *Delimited Text Layer*, dan KMZ yang dapat dibuka di Google Earth / Google My Maps.

| Taman | CSV | KMZ | Kota | Luas (ha) |
|-------|-----|-----|------|-----------|
| Taman Monas | [taman-monas.csv](taman-monas.csv) | [taman-monas.kmz](taman-monas.kmz) | Jakarta Pusat | 73 |
| Gelora Bung Karno | [taman-gelora-bung-karno.csv](taman-gelora-bung-karno.csv) | [taman-gelora-bung-karno.kmz](taman-gelora-bung-karno.kmz) | Jakarta Pusat | 279 |
| Kebun Binatang Ragunan | [taman-ragunan.csv](taman-ragunan.csv) | [taman-ragunan.kmz](taman-ragunan.kmz) | Jakarta Selatan | 147 |
| Tebet Eco Park | [taman-tebet-eco-park.csv](taman-tebet-eco-park.csv) | [taman-tebet-eco-park.kmz](taman-tebet-eco-park.kmz) | Jakarta Selatan | 7 |
| Taman Mini Indonesia Indah | [taman-mini-indonesia-indah.csv](taman-mini-indonesia-indah.csv) | [taman-mini-indonesia-indah.kmz](taman-mini-indonesia-indah.kmz) | Jakarta Timur | 150 |

## Kolom

| Kolom | Keterangan |
|-------|------------|
| `name` | Nama taman |
| `description` | Deskripsi |
| `wkt_geometry` | Geometri area, `POLYGON ((longitude latitude, ...))` |
| `latitude_centroid` | Lintang titik tengah |
| `longitude_centroid` | Bujur titik tengah |
| `area_ha` | Luas (hektare) |
| `kecamatan` | Kecamatan |
| `kota` | Kota administrasi |
| `provinsi` | Provinsi |
