## Definition

Library performance monitoring membantu pengembang mengukur kinerja aplikasi mereka dengan mengumpulkan metrik dan statistik. Hal ini memungkinkan pengembang untuk mendeteksi masalah kinerja, mengoptimalkan aplikasi, dan memahami bagaimana aplikasi berperilaku di bawah beban tertentu.

## [Fiberprometheus](https://github.com/ansrivas/fiberprometheus)

Library "fiberprometheus" dalam bahasa pemrograman Go (Golang) adalah sebuah middleware yang dirancang untuk digunakan dengan framework web "Fiber." Middleware ini berfungsi untuk mengumpulkan metrik Prometheus dari aplikasi web Anda yang menggunakan Fiber. Dengan menggunakan "fiberprometheus," Anda dapat dengan mudah memantau dan mengukur kinerja aplikasi web Anda, termasuk jumlah permintaan HTTP, kode status respons, dan statistik lainnya. Ini memungkinkan pengembang untuk mendapatkan wawasan yang mendalam tentang bagaimana aplikasi beroperasi dalam lingkungan produksi, yang dapat membantu dalam pemecahan masalah, peningkatan kinerja, dan manajemen aplikasi secara keseluruhan.

## [New Relic Go Agent](https://github.com/newrelic/go-agent)

Agen Go New Relic memungkinkan Anda untuk memantau aplikasi Go Anda dengan New Relic. Ini membantu Anda melacak transaksi, permintaan keluar, panggilan database, dan bagian-bagian lain dari perilaku aplikasi Go Anda, serta memberikan gambaran berkelanjutan tentang pengumpulan sampah, aktivitas goroutine, dan penggunaan memori. Go adalah bahasa yang dikompilasi dan tidak menggunakan mesin virtual. Ini berarti bahwa mengatur New Relic untuk aplikasi Golang Anda memerlukan penggunaan API agen Go kami dan penambahan metode-metode New Relic ke dalam kode sumber Anda secara manual. API kami memberikan fleksibilitas dan kontrol yang luar biasa terhadap apa yang akan diinstrumentasi.

## [Gin Metrics](https://github.com/penglongli/gin-metrics)

Dalam bahasa pemrograman Go (Golang), terdapat library yang dikenal sebagai "gin-metrics," yang berfungsi sebagai middleware spesifik untuk framework web Gin. Middleware ini memiliki peran utama dalam mengumpulkan data metrik dan statistik yang berkaitan dengan kinerja aplikasi web yang telah dibangun menggunakan Gin. Integrasi "gin-metrics" mempermudah pemantauan berbagai parameter penting seperti jumlah permintaan HTTP, waktu respons rata-rata, serta sejumlah metrik penting lainnya. Informasi ini memberikan pemahaman yang lebih mendalam tentang bagaimana performa aplikasi Anda berkinerja dalam lingkungan produksi. Data ini dapat digunakan sebagai dasar untuk melakukan perbaikan kinerja, mengatasi masalah, dan membuat keputusan yang lebih cerdas terkait dengan skalabilitas dan kapasitas server Anda.

## Scoring sheet

| Komponen        | Fiberprometheus | New Relic Go Agent | Gin Metrics |
|-----------------|----------|--------|-------|
| Maintenance     |    4     |   4    |   1   |
| Reputable       |    2     |    2   |   2   |
| Compatibility   |    4     |   3    |  4    |
| Community       |     4    |   3    |   4   |
| Documentation   |     3    |  3     |  3    |
| Licensing       |    4     |   4    |   4   |
| Extensible      |     4    |    3   |   4   |
| Size            |    4     |     4  |   4   |
| **Total Score** |      29    |    26    |   26    |


## Conclusion

Berdasarkan score yang didapat, library fiberprometheus memiliki angka yang paling besar. Selain itu, fiberprometheus juga compatible dengan project-project yang ada di **T** karena kebanyakan sudah memakai framework Fiber. Jadi pilihan yang tepat untuk library monitoring adalah Fiber.