## Definition
Relational Database Management System (RDBMS) adalah jenis sistem manajemen basis data yang menggunakan model data relasional untuk mengorganisasi dan mengelola informasi. Ini didasarkan pada tabel yang terdiri dari baris dan kolom, di mana data disimpan dan diakses dengan menggunakan bahasa SQL (Structured Query Language).

## Spring Data JPA

**Spring Data JPA** adalah teknologi yang memfasilitasi pembuatan lapisan akses data dalam aplikasi Java. Ini adalah ekstensi dari Java Persistence API (JPA), yang merupakan spesifikasi standar Java untuk pemetaan objek-relasional. Spring Data JPA menambahkan lapisan abstraksi lain di atas JPA, mendefinisikan desain berbasis standar untuk mendukung Lapisan Persistensi dalam konteks Spring.

## Spring Data R2DBC

**Spring Data JPA R2DBC** adalah bagian dari inisiatif Spring yang bertujuan untuk membawa teknologi _non-blocking_ ke data akses, memungkinkan aplikasi untuk menangani lebih banyak koneksi secara bersamaan. Ini sangat berbeda dari JPA dan semua yang dibangun di atasnya, karena JPA memiliki cache sebagai bagian integral dari sistem yang akan menghasilkan efek menarik ketika Anda mencampur JPA dan akses JDBC langsung dalam satu transaksi.

## Scoring sheet

| Komponen          | Spring Data JPA | Spring Data R2DBC |
| :---------------- | :-------------: | :---------------: |
| Maintenance       | 4               | 4                 |
| Reputable         | 4               | 4                 |
| Compatibility     | 3               | 3                 |
| Community         | 4               | 4                 |
| Documentation     | 4               | 4                 |
| Licensing         | 4               | 4                 |
| Extensible        | 4               | 4                 |
| Size              | 4               | 4                 |
| **Total Score**   | 31              | 31                |
| **Average Score** | 3.875           | 3.875             |

## Conclusion
### Gunakan Spring Data JPA ketika:
1. Bekerja dengan aplikasi berbasis blok `(synchronous)` dan memerlukan fitur lengkap JPA.
2. Memerlukan fitur seperti caching level kedua, lazy loading, write-behind, dan auditing.
3. Ingin mengintegrasikan dengan Hibernate atau penyedia JPA lainnya.
4. Memerlukan dukungan untuk Querydsl predicates dan query JPA yang aman secara tipe, serta dukungan untuk audit domain class, dukungan pagination, eksekusi query dinamis, dan kemampuan untuk mengintegrasikan kode akses data kustom.

### Gunakan Spring Data R2DBC ketika:
1. Bekerja dengan aplikasi berbasis non-blok `(asynchronous)` dan memerlukan akses data yang efisien dan skalabel.
2. Memerlukan dukungan untuk MySQL menggunakan jasync-sql, manajer transaksi reaktif, API Fluent untuk operasi insert/update/delete, ekstensi Coroutine, dukungan untuk konversi kustom, dan parameter bernama yang diterjemahkan ke penanda bind asli menggunakan instansi Dialect.
3. Tidak memerlukan fitur seperti caching level kedua, lazy loading, dan write-behind.