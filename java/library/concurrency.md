## Definition

Concurrency adalah konsep dalam pemrograman yang mengacu pada kemampuan sebuah program untuk menjalankan beberapa tugas atau potongan kode secara bersamaan, tanpa harus menunggu tugas sebelumnya selesai. Ini dapat diterapkan untuk meningkatkan efisiensi dan kinerja dalam aplikasi, terutama pada sistem dengan banyak prosesor atau pada tugas yang melibatkan I/O.

## Spring Context

Spring Context, juga dikenal sebagai Spring IoC (Inversion of Control) container, adalah konstruksi pemrograman yang digunakan oleh Spring Framework untuk mengakses komponen dari kontainer IoC. Kontainer Spring IoC bertanggung jawab untuk mengelola objek dari suatu aplikasi. Kontainer ini menggunakan dependency injection untuk mencapai inversion of control.

Ada dua antarmuka utama yang mewakili kontainer Spring IoC, yaitu `BeanFactory` dan `ApplicationContext`. Di sini, `BeanFactory` adalah antarmuka root untuk mengakses kontainer Spring dan menyediakan fungsi dasar untuk mengelola bean. Di sisi lain, `ApplicationContext` adalah sub-antarmuka dari `BeanFactory`, sehingga menawarkan semua fungsi `BeanFactory` dan juga menyediakan fungsi yang lebih spesifik untuk enterprise.

Fitur penting dari `ApplicationContext` meliputi penyelesaian pesan, dukungan internasionalisasi, penerbitan event, dan konteks spesifik lapisan aplikasi. Oleh karena itu, kita biasanya menggunakan `ApplicationContext` sebagai kontainer Spring default.

Dalam Spring, bean adalah objek yang diinstansiasi, dirakit, dan dikelola oleh kontainer Spring. Sebagai praktik terbaik, kita seharusnya tidak mendefinisikan semua objek aplikasi kita sebagai bean Spring. Biasanya, kita harus mendefinisikan bean untuk objek lapisan layanan, objek akses data (DAO), objek presentasi, objek infrastruktur seperti `Hibernate SessionFactories`, `JMS Queues`, dan sebagainya.

Spring Context menangani concurrency dengan beberapa cara:

1. **Model Thread-per-Request**: Dalam aplikasi web tradisional, setiap permintaan pengguna ke server web dapat ditangani oleh thread yang berbeda. Ini dikenal sebagai model thread-per-request.

2. **Pemrograman Reaktif**: Pemrograman reaktif membantu kita merancang program dalam hal aliran data dan propagasi perubahan melalui mereka. Dalam lingkungan yang sepenuhnya non-blocking, ini dapat memungkinkan kita mencapai concurrency yang lebih tinggi dengan penggunaan sumber daya yang lebih baik. Misalnya, dalam model reaktif, panggilan baca ke database tidak memblokir thread yang memanggil sementara data diambil.

3. **Spring WebFlux**: Spring WebFlux menawarkan abstraksi concurrency atas berbagai pustaka server reaktif.

4. **Spring Security**: Dalam sebagian besar lingkungan, Keamanan disimpan berdasarkan Thread. Ini berarti bahwa ketika pekerjaan dilakukan pada Thread baru, SecurityContext hilang. Spring Security menyediakan beberapa infrastruktur untuk membantu membuat ini jauh lebih mudah bagi pengguna.

5. **Singleton Bean**: Ketika kontainer Spring membuat bean dengan lingkup singleton, bean tersebut disimpan di heap. Dengan cara ini, semua thread concurrent dapat menunjuk ke instance bean yang sama.

6. **TaskExecutor**: Spring Framework menyediakan abstraksi untuk eksekusi asinkron tugas dengan menggunakan antarmuka TaskExecutor. Executor adalah nama Java SE untuk konsep thread pool.

Dengan demikian, Spring Context menawarkan berbagai cara untuk menangani concurrency.

- [What is the meaning of "context" in Spring? - Stack Overflow](https://stackoverflow.com/questions/58245160/what-is-the-meaning-of-context-in-spring)
- [What Is a Spring Context? - DZone](https://dzone.com/articles/what-is-a-spring-context)
- [The Spring ApplicationContext | Baeldung](https://www.baeldung.com/spring-application-context)
- [Concurrency in Spring WebFlux | Baeldung](https://www.baeldung.com/spring-webflux-concurrency)
- [Concurrency Support :: Spring Security](https://docs.spring.io/spring-security/reference/features/integrations/concurrency.html)
- [How Does the Spring Singleton Bean Serve Concurrent Requests?](https://www.baeldung.com/spring-singleton-concurrent-requests)
- [Threading and Concurrency in Spring Boot applications - IBM](https://www.ibm.com/docs/en/cics-ts/5.6?topic=applications-threading-concurrency-in-spring-boot)
- [How does Spring bean Handle concurrency - Stack Overflow](https://stackoverflow.com/questions/13776728/how-does-spring-bean-handle-concurrency)