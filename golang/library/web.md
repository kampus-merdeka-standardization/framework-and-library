## Definition

Library web adalah seperangkat alat, modul, atau fungsi yang digunakan oleh pengembang perangkat lunak untuk membangun dan mengelola aplikasi web. Library web bertujuan untuk menyederhanakan pengembangan aplikasi web dengan menyediakan solusi umum untuk tugas-tugas yang sering diperlukan dalam pembangunan situs web atau aplikasi web, sehingga pengembang dapat fokus pada logika bisnis inti tanpa harus memulai dari nol dalam setiap proyek.

## Gin

Gin adalah _framework_ web yang ditulis dalam [Go](https://go.dev/). Ini menampilkan API seperti martini dengan kinerja hingga 40 kali lebih cepat berkat [httprouter](https://github.com/julienschmidt/httprouter). Jika membutuhkan performa dan produktivitas yang baik, Gin sangatlah cocok.

## Fiber

Fiber adalah kerangka kerja web yang terinspirasi dari [Express](https://github.com/expressjs/express) yang berbasiskan [Fasthttp](https://github.com/valyala/fasthttp), HTTP engine paling cepat untuk Go. Dirancang untuk mempermudah, mempercepat pengembangan aplikasi dengan alokasi memori nol-nya serta kinerja yang selalu diperhatikan.

## Gorilla-mux

Gorilla Mux adalah framework yang sangat berguna dalam ekosistem bahasa pemrograman Go (Golang) untuk membangun aplikasi web berbasis HTTP. Salah satu fitur utamanya adalah kemampuan untuk mengelola routing dengan fleksibilitas tinggi, memungkinkan Anda untuk mendefinisikan pola rute yang kompleks dan menghubungkannya dengan fungsi pengendali yang sesuai. Anda dapat dengan mudah mengekstrak parameter dari URL, memungkinkan Anda untuk mengambil data dari URL dan menggunakannya dalam pemrosesan permintaan.

## Scoring sheet

| Komponen        | Gin | Fiber | Gorilla Mux |
|-----------------|-----|-------|-------------|
| Maintenance     | 4   | 4     | 4           |
| Reputable       | 4   | 4     | 4           |
| Compatibility   | 4   | 4     | 4           |
| Community       | 3   | 4     | 3           |
| Documentation   | 4   | 4     | 3           |
| Licensing       | 4   | 4     | 4           |
| Extensible      | 3   | 4     | 3           |
| Size            | 4   | 3     | 4           |
| **Total Score** | 30  | 31    | 29          |

## Conclusion

Berdasarkan hasil scoring, Fiber memiliki angka yang paling besar. Fiber memiliki hasil yang paling baik dalam benchmark. Fiber juga sudah digunakan di banyak project di Telkomsel. Jadi Fiber adalah pilihan yang baik untuk library Web