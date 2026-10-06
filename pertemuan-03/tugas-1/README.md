# Pertemuan 3 — Tugas 1: Provinsi Berdasarkan Wilayah

Data titik (centroid) provinsi di Indonesia, dikelompokkan per wilayah. Setiap file berisi geometri `POINT` dalam format WKT (CRS: WGS 84 / EPSG:4326) sehingga dapat langsung dimuat di QGIS sebagai *Delimited Text Layer*.

| File | Wilayah | Jumlah Provinsi |
|------|---------|-----------------|
| [provinsi-sumatera.csv](provinsi-sumatera.csv) | Sumatera | 10 |
| [provinsi-jawa-bali.csv](provinsi-jawa-bali.csv) | Jawa & Bali | 7 |
| [provinsi-kalimantan.csv](provinsi-kalimantan.csv) | Kalimantan | 5 |
| [provinsi-sulawesi.csv](provinsi-sulawesi.csv) | Sulawesi | 6 |
| [provinsi-indonesia-timur.csv](provinsi-indonesia-timur.csv) | Nusa Tenggara, Maluku & Papua | 6 |

## Kolom

| Kolom | Keterangan |
|-------|------------|
| `WKT` | Geometri titik, `POINT (longitude latitude)` |
| `id` | Kode provinsi (BPS) |
| `name` | Nama provinsi |
| `alt_name` | Nama alternatif |
| `latitude` | Lintang |
| `longitude` | Bujur |
