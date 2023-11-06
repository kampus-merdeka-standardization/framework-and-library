## Definition

Library rest client adalah perangkat lunak atau modul yang memungkinkan pengembang untuk berinteraksi dengan layanan RESTful API (Application Programming Interface) menggunakan bahasa pemrograman tertentu dengan mudah. Ini menyediakan fungsi dan abstraksi yang memungkinkan pengiriman permintaan HTTP seperti GET, POST, PUT, dan DELETE ke endpoint API, serta pengolahan respons yang diterima. Library rest client membantu mengotomatiskan sebagian besar tugas yang terkait dengan komunikasi dengan API, termasuk manajemen autentikasi, pengelolaan sesi, pemrosesan format data seperti JSON atau XML, serta penanganan kesalahan.

## [Fiber](https://github.com/gofiber/fiber)

Fiber adalah kerangka kerja web yang terinspirasi dari [Express](https://github.com/expressjs/express) yang berbasiskan [Fasthttp](https://github.com/valyala/fasthttp), HTTP engine paling cepat untuk Go. Dirancang untuk mempermudah, mempercepat pengembangan aplikasi dengan alokasi memori nol-nya serta kinerja yang selalu diperhatikan.

## [Resty](https://github.com/go-resty/resty)

HTTP dan REST client library sederhana untuk Go (terinspirasi oleh Ruby rest-client)

## [Heimdall](https://github.com/gojek/heimdall)

Heimdall adalah HTTP client yang membantu aplikasi untuk membuat permintaan dalam jumlah besar, dalam skala besar.

## Scoring sheet

| Komponen        | Fiber | Resty | Heimdall |
|-----------------|-----| -------- |---------|
| Maintenance     |  4  |     4     |    1    |
| Reputable       |  3  |     2     |    4    |
| Compatibility   |  4  |    3      |    4    |
| Community       |  4  |     2     |    4    |
| Documentation   |  4  |     3     |    3    |
| Licensing       |  4  |     4     |    4    |
| Extensible      |  3  |     3     |    4    |
| Size            |  1  |    4      |    4    |
| **Total Score** |  27 |     25     |    28   |

## Conclusion

Berdasarkan score yang didapat, Heimdall memiliki angka yang paling besar. Selain itu, Heimdall dibuat oleh perusahaan besar yaitu Gojek. Jadi pilihan yang tepat untuk library Rest Client adalah Heimdall.