# Framework Java

Pada bagian *framework* ini, hanya akan membahas 2 framework yang cukup populer di Java. Yaitu [Spring](https://spring.io/) dan [Quarkus](https://quarkus.io/)

## Spring

Spring Framework adalah sebuah kerangka kerja (framework) berbasis Java yang bersifat open source. Framework ini menyediakan infrastruktur yang komprehensif untuk memudahkan dan mempercepat pengembangan aplikasi Java. Spring pertama kali ditulis dan dirilis oleh Rod Johnson dengan lisensi Apache 2.0 pada bulan Juni 2003.

Spring Framework dirancang untuk mendukung paradigma pemrograman berorientasi objek, memungkinkan pengembang untuk fokus pada logika bisnis aplikasi tanpa harus khawatir tentang banyak masalah infrastruktur. Salah satu fitur kunci dari Spring Framework adalah Inversion of Control (IoC), yang memisahkan komponen aplikasi dari pengelolaan siklus hidupnya dan memungkinkan aplikasi untuk menjadi lebih longgar dikaitkan.

Spring Framework juga menyediakan Dependency Injection (DI), yang memungkinkan penggunaan komponen dengan cara menginjeksikan (mengisi) dependensi mereka ke dalam komponen lain. Selain itu, Spring Framework juga menyediakan modul-modul yang mencakup berbagai aspek pengembangan aplikasi, seperti keamanan, manajemen transaksi, akses ke basis data, pengembangan web, dan banyak lagi.

Secara keseluruhan, Spring Framework telah menjadi salah satu kerangka kerja yang sangat populer di dunia Java untuk pengembangan aplikasi yang efisien, mudah dipelajari, dan berskala baik.

## Quarkus

Quarkus adalah kerangka kerja Java yang dibangun di atas pustaka dan pola Java terbaik. Tujuan utama Quarkus adalah memungkinkan pengembangan dan inisialisasi aplikasi yang lebih cepat, menjadi lebih kecil dan mengonsumsi lebih sedikit sumber daya mesin  . Quarkus lahir dengan ide untuk menjadi Cloud Native, digunakan dalam proyek Microservices dan Serverless.

Quarkus adalah kerangka kerja sumber terbuka untuk membangun aplikasi Java modern dengan konfigurasi nol². Ini menggunakan kompiler untuk menghasilkan kode asli untuk platform yang Anda jalankan, jadi Anda tidak perlu melakukan apa pun selain menulis kode Anda. Proyek Quarkus adalah inisiatif berbasis komunitas yang bertujuan untuk membuat kerangka kerja yang memungkinkan Anda membangun dan menerapkan aplikasi Java modern².

Anda dapat menganggap Quarkus sebagai alternatif sumber terbuka yang ringan untuk Spring Boot. Anda dapat menggunakan Quarkus untuk membangun layanan mikro dan aplikasi reaktif yang diterapkan di cloud. Quarkus juga memiliki mekanisme plugin, yang memungkinkan Anda untuk memperluas Quarkus dengan menambahkan fitur baru ke aplikasi Anda.

Secara keseluruhan, Quarkus adalah kerangka kerja yang sangat baik untuk pengembangan aplikasi Java modern, terutama untuk aplikasi yang diterapkan di lingkungan cloud, Kubernetes, dan serverless.

## pros & cons

|          | Spring Framework | Quarkus Framework |
| :------- | :--------------- | :---------------- |
| **Pros** | Memiliki komunitas yang besar dan ekosistem plugin dan library yang luas | Menawarkan kinerja yang superior dan fitur live-to-reload yang unik |
|          | Matang, terkenal, dan stabil | Memiliki waktu boot aplikasi yang cepat, fitur live coding, dan pengalaman pengembang yang sangat baik |
|          | Mendukung Java, Kotlin, dan Groovy | Dioptimalkan untuk cloud, serverless, dan lingkungan kontainer |
|  | Ringan karena implementasi POJO | Dokumentasi sederhana |
|  | Fleksibel dengan pustaka yang dipercaya oleh pengembang di seluruh dunia | Waktu boot yang cepat |
|  | Mendukung injeksi dependensi yang membuat pengujian lebih mudah | Fitur live coding dan pengalaman pengembang yang sangat baik |
|  | Menyediakan abstraksi yang kuat untuk spesifikasi JEE seperti JMS, JDBC, JPA, dan JTA | Dukungan untuk GraalVM |
|  | Dukungan deklaratif untuk caching, validasi, transaksi, dan pemformatan | Lebih inovatif dibandingkan Spring Boot |
| **Cons** | Membutuhkan lebih banyak konfigurasi dan boilerplate | Memiliki dukungan komunitas yang kurang dan kurangnya sumber daya yang ramah pemula |
|          | Memiliki jejak memori yang lebih besar dan waktu startup yang lebih lambat daripada Quarkus | Masih baru dan kurang inovatif daripada Spring Boot |
|          | Memiliki jejak memori yang lebih besar dan waktu startup yang lebih lambat daripada Quarkus | Memerlukan GraalVM untuk membuat native image |
|  | Kerangka kerja ini memiliki banyak variabel dan komplikasi | Kurangnya dukungan komunitas dan kurangnya sumber daya yang ramah pemula |
|  | Memerlukan server, sedangkan aplikasi EJB dan Struts memerlukan server |  |


## scoring list

| Komponen          | Spring | Quarkus |
| :---------------- | :----- | :------ |
| Maintenance       | 4      | 4       |
| Reputable         | 4      | 4       |
| Compatibility     | 4      | 4       |
| Community         | 4      | 3       |
| Documentation     | 4      | 4       |
| Licensing         | 4      | 4       |
| Extensible        | 4      | 4       |
| Size              | 3      | 2       |
| **Total Score**   | 31     | 29      |
| **Average Score** | 3.875  | 3.625   |

## conclusion

Memilih Spring Framework jika memerlukan kerangka kerja yang mapan dengan komunitas besar, fleksibilitas untuk berbagai jenis aplikasi, atau jika sudah memiliki pengalaman dengan ekosistem Spring. Juga, Spring cocok untuk aplikasi Java stand-alone yang lebih umum.

Sementara itu, Quarkus Framework lebih cocok jika kita perlu fokus pada pengoptimalan waktu boot dan penggunaan memori rendah, terutama untuk aplikasi yang akan dijalankan di lingkungan cloud atau serverless. Juga, jika kita memerlukan fitur hot reload dan alat observasi secara out-of-the-box, Quarkus dapat menjadi pilihan yang baik.

## Reference

- [Framework Spring Bikin Aplikasi Java Lebih Gampang - Codepolitan](https://www.codepolitan.com/blog/framework-spring.)

- [Spring Framework - Wikipedia bahasa Indonesia, ensiklopedia bebas](https://id.wikipedia.org/wiki/Spring_Framework)

- [Framework Spring Java - School of Computer Science](https://socs.binus.ac.id/2017/10/04/framework-spring-java/)

- [JAVA LEBIH MUDAH DENGAN SPRING FRAMEWORK - School of Computer Science](https://socs.binus.ac.id/2018/12/06/java-lebih-mudah-dengan-spring-framework/)

- [Quarkus Apa? Mengapa? dan bagaimana? - ICHI.PRO](https://ichi.pro/id/quarkus-apa-mengapa-dan-bagaimana-19017280308335.)

- [Apa itu Quarkus? - HashDork](https://hashdork.com/id/kuarkus/)

- [What is Quarkus? - Red Hat](https://www.redhat.com/en/topics/cloud-native-apps/what-is-quarkus)

- [Kerangka Quarkus menghadirkan Java ke Kubernetes | Dari Linux - Desde Linux](https://blog.desdelinux.net/id/kerangka-kerja-quarkus-membawa-java-ke-kubernetes/)

- [Quarkus - Supersonic Subatomic Java](https://quarkus.io)

- [Quarkus vs. Spring Boot: A head-to-head comparison - Medium](https://medium.com/@samuelcatalano/quarkus-vs-spring-boot-a-head-to-head-comparison-3b9502c0a345)

- [Quarkus vs Spring Boot: Which Framework is Right for You - Rollbar](https://rollbar.com/blog/quarkus-vs-spring-boot/)

- [Spring Boot vs Quarkus | Baeldung](https://www.baeldung.com/spring-boot-vs-quarkus.)


- [Spring Boot vs Quarkus: Which Framework to Choose](https://maddevs.io/blog/spring-boot-vs-quarkus/)


- [Difference between Spring and Quarkus | by Hiten Pratap Singh - Medium](https://medium.com/hprog99/difference-between-spring-and-quarkus-bc55d7ad2c80.)

- [Java Spring Pros and Cons - Javatpoint](https://www.javatpoint.com/java-spring-pros-and-cons)

- [Java Spring Framework – Pros, Cons, Common Mistakes](https://skywell.software/blog/java-spring-framework-pros-cons-mistakes/)

- [Quarkus vs SpringBoot - Knoldus Blogs](https://blog.knoldus.com/quarkus-vs-springboot/)

- [Quarkus - Reviews, Pros & Cons | Companies using Quarkus - StackShare](https://stackshare.io/quarkus)

- [Quarkus vs Spring Boot: Which Framework is Right for You - Rollbar](https://rollbar.com/blog/quarkus-vs-spring-boot/)

- [What are pros and cons of using Spring in Swing based frontend](https://stackoverflow.com/questions/5325690/what-are-pros-and-cons-of-using-spring-in-swing-based-frontend)

- [Quarkus: The new Java framework makes the language fit for the cloud ....](https://www.ionos.com/digitalguide/server/configuration/what-is-quarkus/)

- [Microservices: Benefits of Quarkas vs. Spring | Red Hat Developer](https://developers.redhat.com/articles/2021/08/31/why-should-i-choose-quarkus-over-spring-my-microservices)