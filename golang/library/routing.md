## Definition

Library routing adalah kumpulan alat atau modul yang dirancang khusus untuk mengelola routing dan penanganan permintaan dalam aplikasi web atau jaringan. Library routing membantu pengembang mengatur bagaimana permintaan dari pengguna atau klien akan dipetakan ke fungsi-fungsi pengendali yang sesuai berdasarkan pola-pola rute yang telah ditentukan. Dengan memanfaatkan library routing, pengembang dapat dengan efisien menangani permintaan HTTP, mengelola parameter URL, dan menerapkan logika bisnis dalam aplikasi web.

## [Fiber](https://github.com/gofiber/fiber)

Fiber adalah kerangka kerja web yang terinspirasi dari [Express](https://github.com/expressjs/express) yang berbasiskan [Fasthttp](https://github.com/valyala/fasthttp), HTTP engine paling cepat untuk Go. Dirancang untuk mempermudah, mempercepat pengembangan aplikasi dengan alokasi memori nol-nya serta kinerja yang selalu diperhatikan.

## [Chi](https://github.com/go-chi/chi)

Chi adalah library routing dan middleware yang sangat ringan dan fleksibel untuk bahasa pemrograman Go (Golang). Chi memungkinkan pengembang untuk dengan mudah membuat routing yang kuat dan kompleks serta menggabungkan middleware dengan cara yang modular.  Dengan pendekatan yang minimalis dan fokus pada kecepatan eksekusi, Chi sangat cocok untuk pengembangan aplikasi web yang memerlukan kontrol tinggi atas proses routing dan penanganan middleware.

## Go Standard Library

Golang memiliki standard package untuk routing HTTP. Library yang digunakan adalah "net/http".

## Scoring sheet

| Komponen        | Fiber | Chi | Go Standard Library |
|-----------------|-----------|-----|----------|
| Maintenance     | 4         | 3   | 3        |
| Reputable       | 4         | 2   | 4        |
| Compatibility   | 4         | 3   | 4        |
| Community       | 4         | 4   | 4        |
| Documentation   | 3         | 4   | 4        |
| Licensing       | 4         | 4   | 4        |
| Extensible      | 4         | 4   | 4        |
| Size            | 1         | 4   | 4        |
| **Total Score** | 29        | 28  | 31       |

## Conclusion

Berdasarkan score yang didapat, Go Standard Library memiliki angka yang paling besar. Routing di Golang sendiri sudah sangat baik sehingga tidak perlu menggunakan library tambahan. Tetapi jika ingin menggunakan routing pada framework, maka disarankan menggunakan Fiber. Jadi pilihan yang tepat untuk library routing adalah Go Standard Library.