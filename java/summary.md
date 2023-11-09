# Summary

## Library

### Web



### Logging

Berdasarkan nilai skoring, tampak Logback memiliki penilaian yang lebih tinggi, akan tetapi Log4j2 memiliki sejumlah peningkatan dari Logback, terutama dalam hal vulnerabilities

### Rest Client

Dikarenakan `WebClient` akan menggantikan `RestTemplate`, maka direkomendasikan menggunakan `WebClient` sebagai library _Rest Client_ pada Java.

### Configuration



### Monitoring

Memilih library Spring Boot Actuator sebagai library monitoring. Karena library ini menyediakan fitur-fitur yang siap produksi untuk membantu kita memantau dan mengelola aplikasi Spring Boot. Library ini menggunakan endpoint HTTP untuk mengekspos informasi operasional tentang aplikasi yang sedang berjalan, seperti kesehatan, metrik, audit, tracing, dan lain-lain. Keuntungan dari menggunakan library ini adalah kita dapat mendapatkan informasi yang berguna untuk menganalisis dan meningkatkan kinerja, keamanan, dan ketersediaan aplikasi

Library Spring Boot Actuator juga mendukung integrasi dengan berbagai alat pemantauan eksternal, seperti Prometheus, Grafana, Micrometer, dan lain-lain. Alat-alat ini dapat mengumpulkan, menyimpan, dan memvisualisasikan data dari endpoint Actuator, serta memberikan notifikasi dan peringatan jika terjadi masalah. Dengan menggunakan alat-alat ini, kita dapat memantau aplikasi dari berbagai sudut pandang, seperti penggunaan sumber daya, permintaan HTTP, event audit, dan lain-lain

### RDBMS

#### Gunakan Spring Data JPA ketika:
1. Bekerja dengan aplikasi berbasis blok `(synchronous)` dan memerlukan fitur lengkap JPA.
2. Memerlukan fitur seperti caching level kedua, lazy loading, write-behind, dan auditing.
3. Ingin mengintegrasikan dengan Hibernate atau penyedia JPA lainnya.
4. Memerlukan dukungan untuk Querydsl predicates dan query JPA yang aman secara tipe, serta dukungan untuk audit domain class, dukungan pagination, eksekusi query dinamis, dan kemampuan untuk mengintegrasikan kode akses data kustom.

#### Gunakan Spring Data R2DBC ketika:
1. Bekerja dengan aplikasi berbasis non-blok `(asynchronous)` dan memerlukan akses data yang efisien dan skalabel.
2. Memerlukan dukungan untuk MySQL menggunakan jasync-sql, manajer transaksi reaktif, API Fluent untuk operasi insert/update/delete, ekstensi Coroutine, dukungan untuk konversi kustom, dan parameter bernama yang diterjemahkan ke penanda bind asli menggunakan instansi Dialect.
3. Tidak memerlukan fitur seperti caching level kedua, lazy loading, dan write-behind.

### Document Based DB

Memilih library Spring Data sebagai library document database. Karena library ini menyediakan dukungan untuk berbagai database yang berbasis dokumen, seperti MongoDB, Elasticsearch, Couchbase, dan lain-lain. Spring Data juga menyediakan fitur-fitur tambahan, seperti konversi, indeks, auditing, paging, sorting, dan lain-lain. 

### In-memory DB

Memilih library **Spring Data Redis** sebagai library in-memory database. Karena library ini menyediakan konfigurasi dan akses yang mudah ke Redis dari aplikasi Spring.

Memilih lettuce sebagai klien java untuk redis. Karena **lettuce** menyediakan komunikasi yang non-blocking dan reaktif dengan server redis. **Lettuce** menggunakan netty untuk berkomunikasi dengan server, dan mendukung fitur-fitur redis yang canggih, seperti cluster, sentinel, pipelining, dan codec. **Lettuce** juga menawarkan API yang sinkron, asinkron, dan reaktif, yang dapat digunakan sesuai dengan kebutuhan aplikasi. **Lettuce** juga kompatibel dengan Java 8 atau lebih tinggi, dan dapat digunakan bersama dengan framework lain, seperti Spring Data Redis`

### GraphDB

Gunakanlah **Spring Data** untuk berkomunikasi dengan Graph Database.

Spring Data dapat digunakan untuk Graph Database. Salah satu implementasinya adalah **Spring Data Neo4j**.

**Neo4j** adalah sistem manajemen database grafik populer yang dirancang untuk menyimpan, mengelola, dan melakukan query data menggunakan model berbasis grafik. **Spring Data Neo4j** memudahkan kita untuk berinteraksi dengan database **Neo4j**.

Jadi, dengan Spring Data, kita dapat bekerja dengan berbagai jenis database, termasuk database relasional, non-relasional, dan database berbasis grafik.

### Storage

Memilih library Spring Integration sebagai library Storage adalah karena library ini menyediakan berbagai komponen yang dapat memudahkan dan memperkaya integrasi file dengan sistem penyimpanan eksternal, seperti Azure Storage. Azure Storage adalah layanan cloud yang menyediakan solusi penyimpanan yang andal, aman, dan skalabel untuk berbagai jenis data, seperti blob, file, queue, table, dan disk. Dengan menggunakan komponen-komponen yang disediakan oleh library Spring Integration, developer dapat mengirim dan menerima file dari Azure Storage melalui protokol yang sesuai, seperti FTP, SFTP, HTTP, atau HTTPS

### File Operation

Memilih Spring Integration sebagai library File Operation. Karena library ini menyediakan berbagai komponen yang dapat memudahkan dan memperkaya integrasi file dalam aplikasi Spring. Library ini mengimplementasikan pola-pola integrasi enterprise, seperti messaging, routing, transformation, filtering, dan lain-lain, yang dapat meningkatkan fleksibilitas, modularitas, dan keterbukaan aplikasi. Selain itu Spring integration juga mendukung operasi _non-blocking_

### Concurrency

Memilih library Spring Context sebagai library concurrency. Karena library ini menyediakan dukungan untuk pemrograman reaktif, yang merupakan paradigma pemrograman yang memungkinkan aplikasi untuk menangani banyak permintaan secara asinkron dan non-blocking. Pemrograman reaktif dapat meningkatkan kinerja, skalabilitas, dan efisiensi sumber daya aplikasi, terutama dalam skenario dengan beban tinggi atau latensi tinggi.  Library Spring Context sebagai dapat memberikan keuntungan berupa kemampuan untuk membangun aplikasi web reaktif yang responsif, resilien, dan elastis.

### Routing

Berdasarkan hasil penilaian, **Spring Web** dan **Spring WebFlux** memiliki nilai yang sama. Spring Web dan Spring WebFlux merupakan _library_ didalam ekosistem _Spring Framework_, maka tidak heran apabila memiliki _score_ yang sama tingginya. Untuk itu, Spring Web ataupun Spring WebFlux digunakan berdasarkan kasus yang dimilikinya.

- **Spring Web** Cocok untuk aplikasi yang memanfaatkan arsitektur berbasis blok dan sinkronisasi, di mana setiap permintaan diproses satu per satu. Ini adalah pendekatan yang baik untuk aplikasi yang tidak memerlukan skalabilitas tinggi atau penanganan permintaan simultan.

- **Spring WebFlux** Cocok untuk aplikasi yang memerlukan penanganan permintaan non-blocking dan asinkron, di mana banyak permintaan dapat diproses secara bersamaan. Ini adalah pendekatan yang baik untuk aplikasi dengan beban tinggi atau aplikasi yang memerlukan penanganan permintaan real-time.

Perlu dicatat bahwa kedua kerangka kerja ini dapat digunakan bersamaan dalam satu aplikasi, dan kita dapat memilih pendekatan mana yang paling sesuai dengan kebutuhan aplikasi yang kita kembangkan.

### Queueing

Memilih library Camel Spring Boot sebagai library Queueing. Karena library ini menyediakan integrasi yang mudah dan cepat antara Apache Camel dan Spring Boot. Apache Camel adalah framework open source yang mendukung berbagai pola integrasi enterprise, seperti routing, transformation, filtering, splitting, aggregation, dan lain-lain. Spring Boot adalah framework yang memungkinkan pembuatan aplikasi Spring berbasis Java dengan konfigurasi minimal. Dengan menggunakan library Camel Spring Boot, developer dapat memanfaatkan fitur-fitur dari kedua framework tersebut, seperti auto-configuration, dependency injection, component scanning, dan lain-lain.

Library Camel Spring Boot juga mendukung berbagai komponen Camel yang dapat digunakan untuk berkomunikasi dengan berbagai sistem eksternal, seperti `ActiveMQ`, `RabbitMQ`, `Kafka`, dan lain-lain. Komponen-komponen ini memungkinkan developer untuk mengirim dan menerima pesan Queueing melalui protokol yang sesuai dengan sistem yang digunakan. Queueing adalah metode komunikasi yang menggunakan antrian pesan untuk menyimpan dan mengirim data secara asinkron dan andal. Dengan menggunakan komponen Camel Queueing, developer dapat mengimplementasikan pola-pola Queueing, seperti point-to-point, publish-subscribe, request-reply, dan lain-lain.

### PubSub

Memilih library Camel Spring Boot sebagai library PubSub. Karena library ini menyediakan integrasi yang mudah dan cepat antara Apache Camel dan Spring Boot. Apache Camel adalah framework open source yang mendukung berbagai pola integrasi enterprise, seperti routing, transformation, filtering, splitting, aggregation, dan lain-lain. Dengan menggunakan library Camel Spring Boot, developer dapat memanfaatkan fitur-fitur dari kedua framework tersebut, seperti auto-configuration, dependency injection, component scanning, dan lain-lain.

### Scheduler

Berdasarkan penilaian, _Spring scheduler_ memiliki penilaian yang lebih besar. Walau begitu _Quartz Scheduler_ memiliki lebih banyak fitur yang tidak dimiliki _Spring Scheduler_

### CLI

### XML Processing

Memilih library `Jackson Core` sebagai library XML Processing. Karena memberikan kontrol penuh dan fleksibilitas kepada developer untuk memproses XML sesuai dengan kebutuhan aplikasi. Developer dapat menentukan bagaimana cara mengurai, memvalidasi, mengubah, atau memanipulasi data XML dengan mudah dan efisien. Selain itu, library Jackson Core juga mendukung berbagai format XML, seperti XML standar, XML kompak (Smile), XML biner (CBOR), dan XML dengan komentar. Library Jackson Core juga kompatibel dengan library Jackson lainnya, seperti Jackson Databind dan Jackson Annotation, yang menyediakan fitur tambahan seperti data binding, konversi, dan anotasi. Library Jackson Core juga dapat digunakan untuk mengonversi data antara JSON dan XML, atau antara format lain yang didukung oleh Jackson

### JSON Processing

Memilih library `Jackson Core`. Karena memberikan kontrol penuh dan fleksibilitas kepada developer untuk memproses JSON sesuai dengan kebutuhan aplikasi. Developer dapat menentukan bagaimana cara mengurai, memvalidasi, mengubah, atau memanipulasi data JSON dengan mudah dan efisien. Selain itu, library Jackson Core juga mendukung berbagai format JSON, seperti JSON standar, JSON kompak (Smile), JSON biner (CBOR), dan JSON dengan komentar. Library Jackson Core juga kompatibel dengan library Jackson lainnya, seperti Jackson Databind dan Jackson Annotation, yang menyediakan fitur tambahan seperti data binding, konversi, dan anotasi.
### Packaging Tools

### SDK

## Framework

Memilih Spring Framework, karena Spring merupakan kerangka kerja yang mapan dengan komunitas besar, fleksibilitas untuk berbagai jenis aplikasi. Selain itu, Spring sangat sesuai untuk pengembangan aplikasi Java stand-alone yang umum digunakan.
