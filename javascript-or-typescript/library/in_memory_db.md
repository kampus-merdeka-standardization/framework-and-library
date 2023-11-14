# In Memory Database

## Definition

In-Memory Database (IMDB), adalah sistem manajemen database yang sebagian besar mengandalkan memori utama untuk penyimpanan data komputer. Ini berlawanan dengan sistem manajemen database yang menggunakan mekanisme penyimpanan disk.

Database In-Memory lebih cepat daripada database yang dioptimalkan untuk disk karena akses disk lebih lambat daripada akses memori dan algoritma optimasi internal lebih sederhana dan menjalankan instruksi CPU lebih sedikit. Mengakses data dalam memori menghilangkan waktu pencarian saat melakukan query data, yang memberikan kinerja yang lebih cepat dan lebih dapat diprediksi.

## ioredis

**ioredis** adalah Redis yang kuat, berfokus pada kinerja, dan berfitur lengkap untuk Node.js. ioredis mendukung Cluster, Sentinel, Streams, dll. 100% ditulis dalam TypeScript dan declaration resmi disediakan.

Hubungan antara Redis dan In-Memory Database (IMDB) adalah bahwa Redis adalah jenis IMDB. Ini berarti Redis mengandalkan memori utama komputer untuk penyimpanan data. Oleh karena itu, Redis lebih cepat daripada database yang dioptimalkan untuk disk karena akses disk lebih lambat daripada akses memori. Oleh karena itu, ioredis digunakan untuk berinteraksi dengan Redis, database dalam memori, dalam aplikasi Node.js.

## liaoliaots/nestjs-redis

`@liaoliaots/nestjs-redis` adalah modul Redis (ioredis) untuk framework Nest (node.js). Modul ini diterbitkan oleh pengguna GitHub dengan nama `liaoliaots`. Anda dapat mulai menggunakan `@liaoliaots/nestjs-redis` di proyek Anda dengan menjalankan `npm i @liaoliaots/nestjs-redis`. Terdapat 39 proyek lain di registri npm yang menggunakan `@liaoliaots/nestjs-redis`.

## Scoring sheet

| Kriteria       | ioredis | liaoliaots/nestjs-redis |
| -------------- | ------- | ----------------------- |
| Maintenance    | 2       | 1                       |
| Reputable      | 4       | 3                       |
| Compatibility  | 4       | 4                       |
| Community      | 4       | 4                       |
| Documentation  | 4       | 3                       |
| Licensing      | 4       | 4                       |
| Extensible     | 4       | 3                       |
| Size           | 4       | 4                       |
| **Total Skor** | **30**  | **26**                  |

## Conclusion

Berdasarkan skor yang tinggi pada setiap kriteria penilaian, ioredis terpilih sebagai klien Redis utama untuk pengembangan backend menggunakan NestJS. Kemampuannya yang kuat, fitur-fitur lengkap, dan dukungan komunitas yang solid menjadikannya pilihan yang handal untuk proyek-proyek yang memerlukan database in-memory dengan akses yang cepat dan efisien.

## Referensi

- [ioredis - npm](https://www.npmjs.com/package/ioredis)
- [How to implement Redis pipelining in Node.Js using ioredis](https://medium.com/@239yash/how-to-implement-redis-pipelining-in-node-js-using-ioredis-ba3eab32f1a7)
- [In-memory database](https://en.wikipedia.org/wiki/In-memory_database)
- [ioredis - github](https://github.com/redis/ioredis)
- [liaoliaots/nestjs-redis - github](https://github.com/liaoliaots/nestjs-redis)
