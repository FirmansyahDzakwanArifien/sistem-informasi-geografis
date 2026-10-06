# Pertemuan 3 — Tugas 2: Layer Kabupaten/Kota Pulau Jawa

Data titik kabupaten/kota di Pulau Jawa, dipisah per provinsi (satu file = satu layer). Setiap file berisi geometri `POINT` dalam format WKT (CRS: WGS 84 / EPSG:4326) sehingga dapat dimuat di QGIS sebagai *Delimited Text Layer*.

| File | Provinsi | Jumlah Kab/Kota |
|------|----------|-----------------|
| [kabkota-dki-jakarta-kep-seribu.csv](kabkota-dki-jakarta-kep-seribu.csv) | DKI Jakarta | 6 |
| [kabkota-banten.csv](kabkota-banten.csv) | Banten | 8 |
| [kabkota-jawa-barat.csv](kabkota-jawa-barat.csv) | Jawa Barat | 27 |
| [kabkota-jawa-tengah.csv](kabkota-jawa-tengah.csv) | Jawa Tengah | 35 |
| [kabkota-di-yogyakarta.csv](kabkota-di-yogyakarta.csv) | DI Yogyakarta | 5 |
| [kabkota-jawa-timur.csv](kabkota-jawa-timur.csv) | Jawa Timur | 38 |
| **Total** | | **119** |

## Kolom

| Kolom | Keterangan |
|-------|------------|
| `WKT` | Geometri titik, `POINT (longitude latitude)` |
| `Layer` | Nama layer |
| `Provinsi` | Nama provinsi |
| `Nama` | Nama kabupaten/kota |
| `Jenis` | `Kabupaten` atau `Kota` |
| `Alamat` | Alamat lengkap |
| `Latitude` | Lintang |
| `Longitude` | Bujur |
