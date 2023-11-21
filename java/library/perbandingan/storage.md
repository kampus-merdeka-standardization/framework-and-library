## Definition

Network storage adalah layanan penyimpanan awan yang memungkinkan pengguna untuk menyimpan dan mengelola data secara terdistribusi melalui internet. Data disimpan di dalam "bucket" yang dapat diakses dari mana saja melalui API web. Layanan ini menyediakan skala tak terbatas, durabilitas tinggi, dan ketersediaan data yang kuat, serta memungkinkan penyimpanan berbagai jenis data, termasuk gambar, video, file teks, dan data aplikasi.

## Spring Integration 
Spring Integration adalah ekstensi dari model pemrograman Spring yang mendukung Pola Integrasi Perusahaan yang ternama. Ini memungkinkan pesan ringan dalam aplikasi berbasis Spring dan mendukung integrasi dengan sistem eksternal melalui adaptor deklaratif. Adaptor tersebut memberikan tingkat abstraksi yang lebih tinggi atas dukungan Spring untuk remote, pesan, dan penjadwalan.

Spring Integration mengambil konsep ini selangkah lebih maju, di mana POJO (Plain Old Java Object) dihubungkan bersama menggunakan paradigma pesan dan komponen individu mungkin tidak menyadari komponen lain dalam aplikasi. Aplikasi semacam itu dibangun dengan merakit komponen yang dapat digunakan kembali untuk membentuk tingkat fungsionalitas yang lebih tinggi. Dengan desain yang hati-hati, aliran ini dapat dimodularisasi dan juga digunakan kembali pada tingkat yang lebih tinggi.

Selain menghubungkan komponen berskala kecil, Spring Integration menyediakan berbagai pilihan adaptor saluran dan gateway untuk berkomunikasi dengan sistem eksternal. Adaptor Saluran digunakan untuk integrasi satu arah (kirim atau terima); gateway digunakan untuk skenario permintaan/balasan (masuk atau keluar).

Spring Integration juga digunakan sebagai mesin untuk _microservice_ yang didorong oleh pesan dalam proyek Spring Cloud Stream.

Spring Integration dapat digunakan untuk operasi penyimpanan. Spring Integration mendukung berbagai layanan penyimpanan, termasuk Azure Storage Queue dan Google Cloud Storage.

Untuk Azure Storage Queue, Spring Integration menyediakan adaptor untuk mengirim dan menerima pesan. Kita dapat menggunakan adaptor ini untuk berinteraksi dengan Azure Storage Queue melalui API Spring Messaging. Spring Integration juga mendukung operasi batch-consuming.

Untuk Google Cloud Storage, Spring Integration menyediakan dukungan melalui Spring Resource dan Spring Integration.

Dengan demikian, Spring Integration dapat menjadi pilihan yang kuat untuk operasi penyimpanan dalam aplikasi kita.

## Conclusion

Memilih library Spring Integration sebagai library Storage adalah karena library ini menyediakan berbagai komponen yang dapat memudahkan dan memperkaya integrasi file dengan sistem penyimpanan eksternal, seperti Azure Storage. Azure Storage adalah layanan cloud yang menyediakan solusi penyimpanan yang andal, aman, dan skalabel untuk berbagai jenis data, seperti blob, file, queue, table, dan disk. Dengan menggunakan komponen-komponen yang disediakan oleh library Spring Integration, developer dapat mengirim dan menerima file dari Azure Storage melalui protokol yang sesuai, seperti FTP, SFTP, HTTP, atau HTTPS

## References

- [Spring Integration](https://spring.io/projects/spring-integration/)

- [Introduction to Spring Integration | Baeldung](https://www.baeldung.com/spring-integration)

- [Overview of Spring Integration Framework](https://docs.spring.io/spring-integration/docs/current/reference/html/overview.html)

- [Spring Cloud Azure support for Spring Integration - Java on Azure](https://learn.microsoft.com/en-us/azure/developer/java/spring-framework/spring-integration-support)

- [Use Azure Storage Queue in Spring applications - Java on Azure](https://learn.microsoft.com/en-us/azure/developer/java/spring-framework/using-storage-queue-in-spring-applications)

- [Spring Cloud GCP](https://spring.io/projects/spring-cloud-gcp/)

- [Spring Cloud Azure overview - Java on Azure | Microsoft Learn](https://learn.microsoft.com/en-us/azure/developer/java/spring-framework/developer-guide-overview)