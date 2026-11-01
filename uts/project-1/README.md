# UTS — Project 1: Peta Tematik Indonesia 2025

Peta tematik 38 provinsi di Indonesia menggunakan QGIS. Batas wilayah diambil dari repositori [yusufsyaifudin/wilayah-indonesia](https://github.com/yusufsyaifudin/wilayah-indonesia): 32 provinsi dari `data/geojson/province` dan enam provinsi di Tanah Papua disusun dari file kabupaten (`data/geojson/regency`, kode `91xx` dan `94xx`) dengan **Merge Vector Layers** + **Dissolve**, karena repositori masih memakai pembagian 34 provinsi. Data non-spasial BPS 2025 dimasukkan lewat **Join Attributes by Field Value** (field `kode`), `kepadatan` dihitung dengan Field Calculator (`"populasi" / "luas_wilayah"`), lalu setiap tema divisualisasikan dengan simbologi **Graduated** dan Print Layout A4.

| File | Keterangan |
|------|------------|
| `provinsi_indonesia.gpkg` | Polygon 38 provinsi (WGS 84) beserta atribut non-spasial |
| `data_provinsi_2025.csv` | Tabel data BPS 2025 yang di-join ke layer provinsi |
| [peta_tematik_indonesia.qgz](peta_tematik_indonesia.qgz) | Project QGIS (QGIS 4.2.3), enam layer tematik dan enam Print Layout |
| [peta_1_jumlah_penduduk.png](peta_1_jumlah_penduduk.png) | Peta jumlah penduduk |
| [peta_2_kepadatan_penduduk.png](peta_2_kepadatan_penduduk.png) | Peta kepadatan penduduk |
| [peta_3_ipm.png](peta_3_ipm.png) | Peta Indeks Pembangunan Manusia (kategori BPS) |
| [peta_4_penduduk_miskin.png](peta_4_penduduk_miskin.png) | Peta persentase penduduk miskin September 2025 |
| [peta_5_tingkat_pengangguran.png](peta_5_tingkat_pengangguran.png) | Peta Tingkat Pengangguran Terbuka Agustus 2025 |
| [peta_6_pdrb_per_kapita.png](peta_6_pdrb_per_kapita.png) | Peta PDRB per kapita ADHB |

GeoPackage dipakai supaya nama field seperti `luas_wilayah` dan `pdrb_perkapita` tidak terpotong 10 karakter seperti di Shapefile.

## Atribut

| Field | Keterangan | Sumber |
|-------|------------|--------|
| `kode` | Kode provinsi BPS | – |
| `nama_wilayah` | Nama provinsi | BPS |
| `ibukota` | Ibu kota provinsi | BPS |
| `tahun` | Tahun data (2025) | – |
| `luas_wilayah` | Luas wilayah (km²) | BPS, Luas Daerah dan Jumlah Pulau Menurut Provinsi 2025 |
| `populasi` | Penduduk pertengahan tahun (jiwa) | BPS, Proyeksi Penduduk 2025 |
| `kepadatan` | `populasi / luas_wilayah` (jiwa/km²) | Field Calculator |
| `ipm` | Indeks Pembangunan Manusia | BPS, IPM Menurut Provinsi 2025 |
| `persen_miskin` | Persentase penduduk miskin, September 2025 (%) | BPS |
| `tpt` | Tingkat Pengangguran Terbuka, Agustus 2025 (%) | BPS (Sakernas) |
| `pdrb_perkapita` | PDRB per kapita ADHB (juta rupiah) | BPS |
| `uhh` | Umur harapan hidup saat lahir (tahun) | BPS |
| `rls` | Rata-rata lama sekolah (tahun) | BPS |
| `jumlah_pulau` | Jumlah pulau | BPS |

## Provinsi di Tanah Papua

| Kode | Provinsi | File kabupaten yang digabung |
|------|----------|------------------------------|
| 91 | Papua Barat | 9101, 9102, 9103, 9104, 9105 |
| 92 | Papua Barat Daya | 9106, 9107, 9108, 9171 |
| 94 | Papua | 9403, 9408, 9409, 9419, 9420, 9426, 9427, 9471 |
| 95 | Papua Selatan | 9401, 9413, 9414, 9415 |
| 96 | Papua Tengah | 9404, 9410, 9411, 9412 |
| 97 | Papua Pegunungan | 9402, 9416, 9417, 9418 |

Kabupaten hasil pemekaran (Tambrauw, Maybrat, Nduga, Puncak, dan lain-lain) belum punya file sendiri di repositori sehingga masih ikut kabupaten induknya. Batas Papua Barat dan Papua Barat Daya jadi sedikit bergeser, jadi kepadatan tetap dihitung dari luas resmi BPS.
