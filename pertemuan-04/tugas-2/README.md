# Pertemuan 4 — Tugas 2: Peta Wilayah Administratif

Data poligon wilayah administratif, satu file per wilayah. Setiap wilayah tersedia dalam dua format: CSV dengan geometri `POLYGON` dalam format WKT (CRS: WGS 84 / EPSG:4326) yang dapat dimuat di QGIS sebagai *Delimited Text Layer*, dan KMZ yang dapat dibuka di Google Earth / Google My Maps.

| Wilayah | CSV | KMZ | Jenis Wilayah | Provinsi |
|---------|-----|-----|---------------|----------|
| DKI Jakarta | [wilayah-dki-jakarta.csv](wilayah-dki-jakarta.csv) | [wilayah-dki-jakarta.kmz](wilayah-dki-jakarta.kmz) | Daerah Khusus Ibu Kota | DKI Jakarta |
| Kota Depok | [wilayah-kota-depok.csv](wilayah-kota-depok.csv) | [wilayah-kota-depok.kmz](wilayah-kota-depok.kmz) | Kota Administrasi | Jawa Barat |
| DI Yogyakarta | [wilayah-di-yogyakarta.csv](wilayah-di-yogyakarta.csv) | [wilayah-di-yogyakarta.kmz](wilayah-di-yogyakarta.kmz) | Daerah Istimewa | DI Yogyakarta |

## Kolom

| Kolom | Keterangan |
|-------|------------|
| `name` | Nama wilayah |
| `description` | Deskripsi |
| `wkt_geometry` | Geometri area, `POLYGON ((longitude latitude, ...))` |
| `latitude_centroid` | Lintang titik tengah |
| `longitude_centroid` | Bujur titik tengah |
| `luas_km2` | Luas (km²) |
| `jenis_wilayah` | Jenis wilayah administratif |
| `provinsi` | Provinsi |
