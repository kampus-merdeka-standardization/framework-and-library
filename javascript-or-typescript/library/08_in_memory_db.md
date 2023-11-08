# In Memory Database

## Definition

In-Memory Database (IMDB), adalah sistem manajemen database yang sebagian besar mengandalkan memori utama untuk penyimpanan data komputer. Ini berlawanan dengan sistem manajemen database yang menggunakan mekanisme penyimpanan disk.

Database In-Memory lebih cepat daripada database yang dioptimalkan untuk disk karena akses disk lebih lambat daripada akses memori dan algoritma optimasi internal lebih sederhana dan menjalankan instruksi CPU lebih sedikit. Mengakses data dalam memori menghilangkan waktu pencarian saat melakukan query data, yang memberikan kinerja yang lebih cepat dan lebih dapat diprediksi daripada dis¹.

## ioredis

**ioredis** adalah Redis yang kuat, berfokus pada kinerja, dan berfitur lengkap untuk Node.js. ioredis mendukung Cluster, Sentinel, Streams, dll. 100% ditulis dalam TypeScript dan declaration resmi disediakan¹.

Hubungan antara Redis dan In-Memory Database (IMDB) adalah bahwa Redis adalah jenis IMDB. Ini berarti Redis mengandalkan memori utama komputer untuk penyimpanan data. Oleh karena itu, Redis lebih cepat daripada database yang dioptimalkan untuk disk karena akses disk lebih lambat daripada akses memori. Oleh karena itu, ioredis digunakan untuk berinteraksi dengan Redis, database dalam memori, dalam aplikasi Node.js.

## Scoring sheet

| Kriteria       | ioredis |
| -------------- | ------- |
| Maintenance   | 2       |
| Reputable       | 4       |
| Compatibility | 4       |
| Community      | 4       |
| Documentation    | 4       |
| Licensing        | 4       |
| Extensible| 4       |
| Size         | 4       |
| **Total Skor** | **30**  |

- **Maintenance**: ioredis mendapatkan skor 2 karena rilis terakhir pada tanggal 15 April 2023 (7 Bulan dari saat dokumen ini dibuat).
- **Reputable**: Sebagai klien Redis yang kuat dan berfokus pada kinerja untuk Node.js, ioredis mendapatkan skor 4.
- **Compatibility**: ioredis mendukung Cluster, Sentinel, Streams, Pipelining, dan tentu saja scripting Lua, Redis Functions, Pub/Sub (dengan dukungan pesan biner), sehingga mendapatkan skor 4.
- **Community**: Dengan komunitas pengguna yang besar dan aktif, ioredis mendapatkan skor 4.
- **Documentation**: Memiliki dokumentasi yang lengkap dan terstruktur dengan baik, ioredis mendapatkan skor 4.
- **Licensing**: Sebagai perangkat lunak open source, ioredis mendapatkan skor 4.
- **Extensible**: ioredis mudah diperluas dan mendukung berbagai fitur, sehingga mendapatkan skor 4.
- **Size**: Ukuran library ioredis relatif kecil, sehingga mendapatkan skor 4.

## Conclusion

Berdasarkan skor yang tinggi pada setiap kriteria penilaian, ioredis terpilih sebagai klien Redis utama untuk pengembangan backend menggunakan NestJS. Kemampuannya yang kuat, fitur-fitur lengkap, dan dukungan komunitas yang solid menjadikannya pilihan yang handal untuk proyek-proyek yang memerlukan database in-memory dengan akses yang cepat dan efisien.

## Referensi

- [ioredis - npm](https://www.npmjs.com/package/ioredis)
- [How to implement Redis pipelining in Node.Js using ioredis](https://medium.com/@239yash/how-to-implement-redis-pipelining-in-node-js-using-ioredis-ba3eab32f1a7)
- [In-memory database](https://en.wikipedia.org/wiki/In-memory_database)
- [ioredis - github](https://github.com/redis/ioredis)
