## Definition

Routing adalah pemetaan permintaan HTTP ke metode tertentu pada kelas kontroler. Dengan kata lain, routing memungkinkan aplikasi untuk menentukan bagaimana permintaan dari klien harus ditangani.

## Spring Web

Cocok untuk aplikasi web tradisional yang memerlukan komunikasi sinkron. Dalam Spring MVC, kita biasanya mendefinisikan _controller_ dengan anotasi seperti `@RestController` dan `@RequestMapping` atau `@GetMapping`, `@PostMapping`, dll. untuk menangani rute tertentu.

## Spring WebFlux

Kerangka kerja web reaktif yang dibangun di atas _Reactive Streams_. Ini dirancang untuk menangani I/O _non-blocking_, di mana _thread_ tidak diblokir saat menunggu respons dari database atau layanan lain. Dalam WebFlux, kita dapat mendefinisikan _controller_ dengan cara yang sama seperti Spring MVC, atau dapat menggunakan API fungsional yang memungkinkan kita untuk mendefinisikan rute dalam kode dengan cara yang lebih fungsional. Misalnya, kita dapat menggunakan `RouterFunction` dan `HandlerFunction` untuk mendefinisikan rute dan penanganannya.

## Scoring sheet

| Komponen          | Spring Web | Spring WebFlux |
| :---------------- | :--------: | :------------: | 
| Maintenance       | 4          | 4              |
| Reputable         | 4          | 4              |
| Compatibility     | 4          | 4              |
| Community         | 4          | 4              |
| Documentation     | 4          | 4              |
| Licensing         | 4          | 4              |
| Extensible        | 4          | 4              |
| Size              | 4          | 4              |
| **Total Score**   | 32         | 32             |
| **Average Score** | 4          | 4              |

## Conclusion

Spring Web dan Spring WebFlux merupakan _library_ didalam keluarga _Spring Framework_, maka tidak heran apabila memiliki _score_ yang sama tingginya. Untuk itu, Spring Web ataupun Spring WebFlux digunakan berdasarkan kasus yang dimilikinya.

- **Spring Web** Cocok untuk aplikasi yang memanfaatkan arsitektur berbasis blok dan sinkronisasi, di mana setiap permintaan diproses satu per satu. Ini adalah pendekatan yang baik untuk aplikasi yang tidak memerlukan skalabilitas tinggi atau penanganan permintaan simultan.

- **Spring WebFlux** Cocok untuk aplikasi yang memerlukan penanganan permintaan non-blocking dan asinkron, di mana banyak permintaan dapat diproses secara bersamaan. Ini adalah pendekatan yang baik untuk aplikasi dengan beban tinggi atau aplikasi yang memerlukan penanganan permintaan real-time.

Perlu dicatat bahwa kedua kerangka kerja ini dapat digunakan bersamaan dalam satu aplikasi, dan kita dapat memilih pendekatan mana yang paling sesuai dengan kebutuhan aplikasi yang kita kembangkan.