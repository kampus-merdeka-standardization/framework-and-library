## Definition

in-memory database (IMDB), adalah sistem manajemen basis data yang menyimpan dan memproses data langsung dalam memori komputer, tanpa perlu akses ke penyimpanan fisik seperti disk. Hal ini memungkinkan kueri dan transaksi untuk dieksekusi dengan sangat cepat karena data dapat diakses secara instan dari RAM. 

## Spring Data Redis

Spring Data Redis adalah bagian dari keluarga Spring Data yang lebih besar, yang menyediakan konfigurasi mudah dan akses ke Redis dari aplikasi Spring. Ini menawarkan abstraksi tingkat rendah dan tinggi untuk berinteraksi dengan toko, membebaskan pengguna dari kekhawatiran infrastruktural.

Berikut adalah beberapa fitur utama dari Spring Data Redis:
- Paket Koneksi sebagai abstraksi tingkat rendah di berbagai driver Redis (Lettuce dan Jedis).

- Terjemahan pengecualian ke hierarki pengecualian Akses Data portabel Spring untuk pengecualian driver Redis.

- RedisTemplate yang menyediakan abstraksi tingkat tinggi untuk melakukan berbagai operasi Redis, terjemahan pengecualian, dan dukungan serialisasi.

- Dukungan Pubsub (seperti MessageListenerContainer untuk POJO yang didorong pesan).

- Dukungan Redis Sentinel dan Redis Cluster.

- API Reaktif menggunakan driver Lettuce.

- Serialisasi JDK, String, JSON dan Pemetaan Objek/XML Spring.

- Implementasi Koleksi JDK di atas Redis.

- Kelas dukungan penghitung atomik.

- Fungsionalitas Pengurutan dan Pipelining.

- Dukungan khusus untuk SORT, pola SORT/GET dan nilai massal yang dikembalikan.

- Implementasi cache Spring 3.1 untuk Redis.

- Implementasi otomatis dari antarmuka Repository termasuk dukungan untuk metode query kustom menggunakan `@EnableRedisRepositories`.

- Dukungan CDI untuk repositori.

Kita dapat menggunakan Spring Data Redis untuk berbagai kebutuhan, seperti database, cache, _message broker_, dan lainnya. Kita juga dapat mengkonfigurasi dan menggunakan RedisTemplate atau salah satu dari opsForX() instances.

### Lettuce vs Jedis

Lettuce dan Jedis adalah dua klien Java yang populer untuk Redis. Berikut adalah beberapa perbedaan utama antara keduanya:

**Lettuce**:
- Lettuce adalah klien Redis Java yang sepenuhnya non-blocking.
- Mendukung komunikasi sinkron dan asinkron.
- Abstraksi kompleksnya memungkinkan Anda untuk meningkatkan skala produk dengan mudah.
- Dianggap sebagai klien yang lebih canggih yang mendukung Cluster, Sentinel, Pipelining, dan codec.
- Jika Anda membutuhkan sesuatu yang sangat dapat diskalakan, gunakan Lettuce.
- Lettuce menawarkan antarmuka alami untuk membuat permintaan asinkron dari server database Redis dan untuk membuat stream.

**Jedis**:
- Jedis adalah perpustakaan klien di dalam Redis yang dirancang untuk kinerja dan kemudahan penggunaan.
- Jedis adalah penawaran yang ringan dibandingkan dengan klien Java Redis lainnya; menawarkan fitur yang lebih sedikit tetapi masih dapat menangani sejumlah besar memori.
- Karena fungsionalitasnya yang lebih sederhana, Jedis lebih mudah digunakan, tetapi hanya bekerja dengan cluster secara sinkron.
- Jika Anda perlu membangun sesuatu dengan cepat dan skalabilitas bukanlah dan mungkin tidak akan menjadi masalah, gunakan Jedis.

### Scoring sheet

| Komponen          | Lettuce | Jedis |
| :---------------- | :-----: | :---: |
| Maintenance       | 4       | 4     |
| Reputable         | 4       | 4     |
| Compatibility     | 4       | 4     |
| Community         | 4       | 4     |
| Documentation     | 4       | 4     |
| Licensing         | 4       | 4     |
| Extensible        | 4       | 4     |
| Size              | 4       | 4     |
| **Total Score**   | 32      | 32    |
| **Average Score** | 4       | 4     |

## Conclusion

Memilih library **Spring Data Redis** sebagai library in-memory database. Karena library ini menyediakan konfigurasi dan akses yang mudah ke Redis dari aplikasi Spring.

Memilih lettuce sebagai klien java untuk redis. Karena **lettuce** menyediakan komunikasi yang non-blocking dan reaktif dengan server redis. **Lettuce** menggunakan netty untuk berkomunikasi dengan server, dan mendukung fitur-fitur redis yang canggih, seperti cluster, sentinel, pipelining, dan codec. **Lettuce** juga menawarkan API yang sinkron, asinkron, dan reaktif, yang dapat digunakan sesuai dengan kebutuhan aplikasi. **Lettuce** juga kompatibel dengan Java 8 atau lebih tinggi, dan dapat digunakan bersama dengan framework lain, seperti Spring Data Redis

## References

- [Spring Data Redis](https://spring.io/projects/spring-data-redis/)

- [Introduction to Spring Data Redis | Baeldung](https://www.baeldung.com/spring-data-redis-tutorial.)

- [Spring Data Redis](https://docs.spring.io/spring-data-redis/docs/current/reference/html/)

- [Jedis vs. Lettuce: An Exploration | Redis](https://redis.com/blog/jedis-vs-lettuce-an-exploration/)

- [Jedis vs. Lettuce: An Exploration – ODBMS.org](https://www.odbms.org/2020/03/jedis-vs-lettuce-an-exploration/)

- [Lettuce — An Advanced Java Client for Redis implementation](https://medium.com/globant/lettuce-an-advanced-java-client-for-redis-implementation-90c267424a01)