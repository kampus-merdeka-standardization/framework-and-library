## Definition

Library configuration membantu pengembang mengelola pengaturan aplikasi, seperti variabel lingkungan, koneksi database, atau parameter lainnya. Dengan library ini, pengembang dapat dengan mudah membaca dan mengubah pengaturan tanpa harus mengubah kode sumber aplikasi.

## Spring Config

Spring Config adalah bagian dari Spring Cloud yang menyediakan dukungan server dan klien untuk konfigurasi eksternal dalam sistem terdistribusi. Dengan Server Config, Kita memiliki tempat pusat untuk mengelola properti eksternal untuk aplikasi di semua lingkungan. Konsep pada klien dan server sama persis dengan abstraksi Spring Environment dan PropertySource, sehingga sangat cocok dengan aplikasi Spring, tetapi dapat digunakan dengan aplikasi apa pun yang berjalan dalam bahasa apa pun.

Implementasi default dari backend penyimpanan server menggunakan git sehingga dengan mudah mendukung versi berlabel dari lingkungan konfigurasi, serta dapat diakses oleh berbagai alat untuk mengelola kontennya1. Sangat mudah untuk menambahkan implementasi alternatif dan mencolokkannya dengan konfigurasi Spring.

## Spring Cloud Consul

Spring Cloud Consul adalah sebuah proyek open-source yang menyediakan integrasi Consul untuk aplikasi Spring Boot melalui autoconfiguration dan binding ke Spring Environment dan idiom pemrograman Spring lainnya. Dengan beberapa anotasi sederhana, Anda dapat dengan cepat mengaktifkan dan mengkonfigurasi pola umum di dalam aplikasi Anda dan membangun sistem terdistribusi besar dengan Consul dari Hashicorp. Pola yang disediakan meliputi Service Discovery, Distributed Configuration, dan Control Bus.

Spring Cloud Consul Config adalah alternatif untuk Config Server dan Client. Konfigurasi dimuat ke dalam Spring Environment selama fase “bootstrap” khusus. Konfigurasi disimpan di folder /config secara default.

## Scoring sheet

| Komponen          | Spring Config | Spring Cloud Consul |
| :---------------- | :-----------: | :-----------------: |
| Maintenance       | 4             | 1                   |
| Reputable         | 4             | 4                   |
| Compatibility     | 4             | 4                   |
| Community         | 4             | 4                   |
| Documentation     | 4             | 4                   |
| Licensing         | 4             | 4                   |
| Extensible        | 4             | 4                   |
| Size              | 4             | 4                   |
| **Total Score**   | 32            | 32                  |
| **Average Score** | 4             | 4                   |

## Conclusion

Memilih Spring Cloud Consul dipilih sebagai library configuration karena menyediakan integrasi Consul untuk aplikasi Spring Boot melalui autoconfiguration dan binding ke Spring Environment dan idiom pemrograman Spring lainnya. Dengan beberapa anotasi sederhana, kita dapat dengan cepat mengaktifkan dan mengkonfigurasi pola umum di dalam aplikasi kita dan membangun sistem terdistribusi besar dengan Consul dari Hashicorp. Pola yang disediakan meliputi Service Discovery, Distributed Configuration, dan Control Bus 


## References

- [Spring Cloud Config](https://spring.io/projects/spring-cloud-config/)

- [Spring Cloud Consul](https://spring.io/projects/spring-cloud-consul/)

- [Spring Cloud Consul](https://docs.spring.io/spring-cloud-consul/docs/current/reference/html/)

- [Spring Cloud Consul](https://cloud.spring.io/spring-cloud-consul/reference/html/)