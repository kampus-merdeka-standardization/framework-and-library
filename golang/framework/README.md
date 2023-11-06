# Framework Golang

Pada bagian *framework* ini, hanya akan membahas 3 framework yang cukup populer di Golang. Dintaranya adalah [Gin](https://github.com/gin-gonic/gin), [Fiber](https://github.com/gofiber/fiber), dan [Gorilla Mux](https://github.com/gorilla/mux).

## Gin

Gin adalah _framework_ web yang ditulis dalam [Go](https://go.dev/). Ini menampilkan API seperti martini dengan kinerja hingga 40 kali lebih cepat berkat [httprouter](https://github.com/julienschmidt/httprouter). Jika membutuhkan performa dan produktivitas yang baik, Gin sangatlah cocok.

### Fitur utama Gin:
1. Zero allocation router
2. Fast
3. Middleware support
4. Crash-free
5. JSON validation
6. Routes grouping
7. Error management
8. Rendering built-in
9. Extendable

## Fiber

Fiber adalah kerangka kerja web yang terinspirasi dari [Express](https://github.com/expressjs/express) yang berbasiskan [Fasthttp](https://github.com/valyala/fasthttp), HTTP engine paling cepat untuk Go. Dirancang untuk mempermudah, mempercepat pengembangan aplikasi dengan alokasi memori nol-nya serta kinerja yang selalu diperhatikan.

### Fitur

- Sistem [Routing](https://docs.gofiber.io/guide/routing) yang padu
- Menyajikan [file statis](https://docs.gofiber.io/api/app#static)
- [Kinerja](https://docs.gofiber.io/extra/benchmarks) ekstrim
- [Penggunaan memori](https://docs.gofiber.io/extra/benchmarks) yang kecil
- Cocok untuk [API](https://docs.gofiber.io/api/ctx)
- Mendukung Middleware & [Next](https://docs.gofiber.io/api/ctx#next) seperti Express
- Kembangkan aplikasi dengan [Cepat](https://dev.to/koddr/welcome-to-fiber-an-express-js-styled-fastest-web-framework-written-with-on-golang-497)
- [Template engines](https://github.com/gofiber/template)
- [Mendukung WebSocket](https://github.com/gofiber/websocket)
- [Server-Sent events](https://github.com/gofiber/recipes/tree/master/sse)
- [Rate Limiter](https://docs.gofiber.io/api/middleware/limiter)
- Tersedia dalam [19 bahasa](https://docs.gofiber.io/)
- Dan masih banyak lagi, [kunjungi Fiber](https://docs.gofiber.io/)

### Filosofi

Bagi yang baru yang beralih dari [Node.js](https://nodejs.org/en/about/) ke [Go](https://go.dev/doc/) terkadang perlu waktu yang cukup lama sebelum mereka mampu membuat aplikasi web dengan Go. Fiber, sebagai **kerangka kerja web** dirancang secara **minimalis** dan mengikuti filosofi dari **UNIX**, sehingga pengguna baru dapat dengan cepat memasuki dunia Go dengan sambutan yang hangat dan dapat diandalkan. Fiber terinspirasi dari Express, salah satu kerangka kerja web yang paling terkenal di
Internet. Kami menggabungkan **kemudahan** dari Express dan **kinerja luar biasa** dari Go. Apabila anda pernah membuat aplikasi dengan Node.js (_dengan Express atau yang lainnya_), maka banyak metode dan prinsip yang akan terasa **sangat umum**
bagi anda.

## Gorilla-mux

Gorilla Mux adalah framework yang sangat berguna dalam ekosistem bahasa pemrograman Go (Golang) untuk membangun aplikasi web berbasis HTTP. Salah satu fitur utamanya adalah kemampuan untuk mengelola routing dengan fleksibilitas tinggi, memungkinkan Anda untuk mendefinisikan pola rute yang kompleks dan menghubungkannya dengan fungsi pengendali yang sesuai. Anda dapat dengan mudah mengekstrak parameter dari URL, memungkinkan Anda untuk mengambil data dari URL dan menggunakannya dalam pemrosesan permintaan.

Nama "mux" dalam Gorilla Mux merupakan singkatan dari "HTTP request multiplexer" atau pemusat penggandaan permintaan HTTP. Mirip dengan http.ServeMux standar, mux.Router pada dasarnya adalah sebuah alat yang digunakan untuk mencocokkan permintaan HTTP yang masuk dengan daftar rute yang telah didaftarkan, dan kemudian memanggil sebuah pengendali (handler) yang sesuai dengan rute yang cocok dengan URL atau kondisi lainnya. 

## pros & cons

| Aspek      | Gin                      | Fiber                              | Gorilla Mux                      |
|------------|--------------------------|------------------------------------|----------------------------------|
| Kelebihan  | - Kinerja tinggi         | - Kinerja tinggi                   | - Routing yang kuat              |
|            | - Routing yang sederhana | - Sintaks mudah dipahami           | - Fleksibilitas                  |
|            | - Middleware yang kuat   | - Middleware yang kuat             |                                  |
|            | - Banyak plugin tersedia | - Sintaks mirip Express.js         |                                  |
| Kekurangan | - Kurangnya fitur penuh  | - Kurangnya ekosistem yang matang  | - Tidak secanggih framework lain |
|            |                          | - Beberapa fitur mungkin belum ada | - Belajar curva tinggi           |

## scoring list

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

## conclusion

Saat ini framework yang sedang ramai dibicarakan adalan Gin dan Fiber. Jika ingin memprioritaskan kinerja tinggi dan memiliki pengalaman dengan Go, Gin mungkin merupakan pilihan yang lebih baik untuk aplikasi yang kompleks dan *high traffic*. Di sisi lain, jika menginginkan kesederhanaan, *asynchronus handling*, dan minimalis, Fiber bisa menjadi pilihan yang tepat, terutama untuk proyek berukuran kecil hingga menengah. Berdasarkan score yang didapat, Fiber memiliki angka yang lebih besar. Fiber juga sudah digunakan di hampir semua project milik Telkomsel. Jadi untuk framework gunakan Fiber.

## Reference

- [Gin](https://github.com/gin-gonic/gin)
- [Fiber](https://github.com/gofiber/fiber)
- [Gorilla Mux](https://github.com/gorilla/mux)
- [Gin vs Fiber](https://medium.com/@ksandeeptech07/golang-gin-vs-fiber-explained-1ca0e7a97bad)