## Definition

Concurrency adalah konsep dalam pemrograman yang mengacu pada kemampuan sebuah program untuk menjalankan beberapa tugas atau potongan kode secara bersamaan, tanpa harus menunggu tugas sebelumnya selesai. Ini dapat diterapkan untuk meningkatkan efisiensi dan kinerja dalam aplikasi, terutama pada sistem dengan banyak prosesor atau pada tugas yang melibatkan I/O.

## Go Standard Library

Go (Golang) memiliki dukungan konkurensi yang kuat dalam standar library-nya dengan menggunakan goroutines dan channel. Goroutines adalah fungsi yang dapat dijalankan secara konkuren (mirip dengan thread), sedangkan channel adalah struktur data yang digunakan untuk komunikasi antara goroutines.

## [Heimdall](https://github.com/gojek/heimdall)

Heimdall adalah HTTP client yang membantu aplikasi untuk membuat permintaan dalam jumlah besar, dalam skala besar.

## Scoring sheet

| Komponen        | Go Standard Library | Heimdall |
|-----------------|-----|---------|
| Maintenance     |  1  |    1    |
| Reputable       |  4  |    4    |
| Compatibility   |  4  |    3    |
| Community       |  4  |    3    |
| Documentation   |  4  |    3    |
| Licensing       |  4  |    4    |
| Extensible      |  4  |    4    |
| Size            |  4  |    4    |
| **Total Score** |  29 |    26   |

## Conclusion

Berdasarkan score yang didapat, Go Standard Library memiliki angka yang paling besar. Concurrency di Golang sendiri sudah sangat baik sehingga tidak perlu menggunakan library tambahan. Jadi pilihan yang tepat untuk library concurrency adalah Go Standard Library.