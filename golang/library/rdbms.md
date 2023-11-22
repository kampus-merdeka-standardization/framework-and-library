## Definition

Relational Database Management System (RDBMS) adalah jenis sistem manajemen basis data yang menggunakan model data relasional untuk mengorganisasi dan mengelola informasi. Ini didasarkan pada tabel yang terdiri dari baris dan kolom, di mana data disimpan dan diakses dengan menggunakan bahasa SQL (Structured Query Language).

## [pgx](https://github.com/jackc/pgx)

pgx adalah driver dan toolkit murni dalam bahasa pemrograman Go untuk PostgreSQL. Driver pgx adalah antarmuka tingkat rendah 
yang memiliki kinerja tinggi dan mengekspos fitur-fitur khusus PostgreSQL seperti LISTEN / NOTIFY dan COPY. Ini juga mencakup 
sebuah adapter untuk antarmuka database/sql standar. Komponen toolkit adalah seperangkat paket terkait yang mengimplementasikan 
fungsi-fungsi PostgreSQL seperti pemrosesan protokol wire dan pemetaan tipe antara PostgreSQL dan Go. Paket-paket dasar ini 
dapat digunakan untuk mengimplementasikan driver alternatif, proxy, load balancer, klien replikasi logis, dan sebagainya.

## [GORM](https://github.com/go-gorm/gorm)

GORM adalah library ORM (Object-Relational Mapping) yang sangat populer dalam bahasa pemrograman Go (Golang). GORM memungkinkan 
pengembang untuk berinteraksi dengan basis data relasional seperti MySQL, PostgreSQL, dan SQLite dengan cara yang lebih mudah 
dan lebih abstrak. Dengan GORM, Anda dapat mendefinisikan model data dalam kode Go dan menggunakan operasi berorientasi objek 
untuk melakukan pembuatan, pembacaan, pembaruan, dan penghapusan data dalam basis data. Ini memungkinkan pengembang untuk 
fokus pada logika bisnis mereka daripada detail teknis dari SQL. GORM juga menyediakan fitur-fitur canggih seperti pengelolaan 
hubungan antar tabel, migrasi basis data, dan dukungan untuk transaksi.

## [SQLx](https://github.com/jmoiron/sqlx)

SQLx adalah sebuah library yang menyediakan serangkaian ekstensi pada library database/sql standar Go. Versi SQLx dari sql.DB, 
sql.TX, sql.Stmt, dan lain-lain, semuanya menjaga antarmuka dasarnya tidak berubah, sehingga antarmuka mereka adalah himpunan 
data yang lebih lengkap dari versi standar. Hal ini membuat integrasi kode-kode yang sudah ada yang menggunakan database/sql 
dengan SQLx menjadi relatif tidak menyakitkan.

## Scoring sheet

| Komponen        | pgx | GORM | SQLx |
|-----------------|----------|--------|-------|
| Maintenance     |    4     |   4    |   2   |
| Reputable       |     2    |    2   |  3    |
| Compatibility   |     3    |   3    |  4    |
| Community       |     3    |   4    |   4   |
| Documentation   |     3    |    4   |  4    |
| Licensing       |      4   |    4   |  4    |
| Extensible      |      3   |    3   |   4   |
| Size            |     4    |    4   |  4    |
| **Total Score** |     26     |   28     |   29    |

## Conclusion

Berdasarkan score yang didapat, library SQLx memiliki angka yang paling besar. Library SQLx dirancang untuk mendukung berbagai sistem database yang kompatibel dengan Golang. Jadi pilihan yang tepat untuk library RDMS adalah SQLx.