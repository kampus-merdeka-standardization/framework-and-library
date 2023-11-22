## Definition

Library performance monitoring membantu pengembang mengukur kinerja aplikasi mereka dengan mengumpulkan metrik dan statistik. Hal ini memungkinkan pengembang untuk mendeteksi masalah kinerja, mengoptimalkan aplikasi, dan memahami bagaimana aplikasi berperilaku di bawah beban tertentu.

## Spring Boot Actuator

Spring Boot Actuator adalah fitur dari Spring Boot yang membawa fitur siap produksi ke aplikasi kita. Dengan Actuator, pemantauan aplikasi, pengumpulan metrik, dan pemahaman lalu lintas atau status database kita menjadi sangat mudah.

Fitur utama dari pustaka ini adalah kita bisa mendapatkan alat tingkat produksi tanpa perlu mengimplementasikan fitur ini sendiri. Actuator terutama mengekspos informasi operasional tentang aplikasi yang sedang berjalan — kesehatan, metrik, info, dump, env, dll. Ini menggunakan titik akhir HTTP atau bean JMX untuk memungkinkan kita berinteraksi dengannya.

Untuk memulai menggunakan Spring Boot Actuator, kita perlu menambahkan dependensi `spring-boot-actuator` ke manajer paket kita. Berikut adalah cara menambahkannya di Maven:
```xml
<dependency>
    <groupId> org.springframework.boot </groupId>
    <artifactId> spring-boot-starter-actuator </artifactId>
</dependency>
```
Dalam versi 2.x, Actuator mempertahankan tujuan dasarnya tetapi menyederhanakan modelnya, memperluas kemampuannya, dan menggabungkan default yang lebih baik. Versi ini menjadi agnostik teknologi. Selain itu, ia juga menyederhanakan model keamanannya dengan menggabungkannya dengan aplikasi.

## Conclusion

Memilih library Spring Boot Actuator sebagai library monitoring. Karena library ini menyediakan fitur-fitur yang siap produksi untuk membantu kita memantau dan mengelola aplikasi Spring Boot. Library ini menggunakan endpoint HTTP untuk mengekspos informasi operasional tentang aplikasi yang sedang berjalan, seperti kesehatan, metrik, audit, tracing, dan lain-lain. Keuntungan dari menggunakan library ini adalah kita dapat mendapatkan informasi yang berguna untuk menganalisis dan meningkatkan kinerja, keamanan, dan ketersediaan aplikasi

Library Spring Boot Actuator juga mendukung integrasi dengan berbagai alat pemantauan eksternal, seperti Prometheus, Grafana, Micrometer, dan lain-lain. Alat-alat ini dapat mengumpulkan, menyimpan, dan memvisualisasikan data dari endpoint Actuator, serta memberikan notifikasi dan peringatan jika terjadi masalah. Dengan menggunakan alat-alat ini, kita dapat memantau aplikasi dari berbagai sudut pandang, seperti penggunaan sumber daya, permintaan HTTP, event audit, dan lain-lain

## References

Source: Conversation with Bing, 11/9/2023
- [Spring Boot Actuator | Baeldung](https://www.baeldung.com/spring-boot-actuators)

- [Spring Boot Actuator: Production-ready Features](https://docs.spring.io/spring-boot/docs/2.5.6/reference/html/actuator.html)

- [Production-ready Features - Spring | Home](https://docs.spring.io/spring-boot/docs/current/reference/html/actuator.html)

- [Monitoring Applications with Prometheus + Grafana + Spring Boot Actuator](https://www.springcloud.io/post/2022-02/monitoring-springboot-applications/)

- [Application Monitoring With Spring Boot Actuator - DZone](https://dzone.com/articles/application-monitoring-with-spring-boot)

- [Actuator in Spring Boot - Spring Framework Guru](https://springframework.guru/actuator-in-spring-boot/)

- [Spring Boot Actuator: Health check, Auditing, Metrics gathering and ...](https://www.callicoder.com/spring-boot-actuator/)