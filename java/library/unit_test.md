## Definition

Unit testing adalah proses pengujian pada tingkat komponen atau unit individu dalam backend. Unit yang dimaksud bisa berupa kode, fungsi, metode, prosedur, modul, atau objek tersendiri. Tujuan dari pengujian ini adalah untuk memvalidasi bahwa setiap unit kode software sudah bisa bekerja sesuai harapan.

## JUnit

JUnit adalah kerangka kerja _unit testing_ untuk bahasa pemrograman Java. Pengembang Java menggunakan kerangka kerja ini untuk menulis dan menjalankan tes otomatis. Dalam Java, ada kasus tes yang harus dijalankan ulang setiap kali kode baru ditambahkan. Ini dilakukan untuk memastikan bahwa tidak ada yang rusak dalam kode.

JUnit memiliki banyak grafik yang mewakili kemajuan tes. Ketika tes berjalan lancar, grafik menampilkan warna hijau, dan berubah menjadi merah ketika tes gagal. Tes JUnit memungkinkan pengembang mengembangkan kode yang sangat andal dan bebas bug.

## Spring Boot Test

`spring-boot-starter-test` adalah dependensi utama untuk pengujian dalam aplikasi Spring Boot. Ini berisi sebagian besar pustaka yang diperlukan untuk pengujian, termasuk `JUnit Jupiter`, `Hamcrest`, dan `Mockito`.

`spring-boot-starter-test` adalah paket agregat untuk perpustakaan yang sering digunakan bersama-sama untuk pengujian dalam aplikasi Spring. Seperti yang dinyatakan dalam dokumentasi referensi versi terbaru, `spring-boot-starter-test` berisi:
- JUnit 5 (termasuk mesin vintage untuk kompatibilitas mundur dengan JUnit 4)
- Spring Test & Spring Boot Test
- AssertJ, Hamcrest, Mockito, JSONassert, dan JsonPath.

Jadi, jika kita menggunakan `spring-boot-starter-test`, kita tidak perlu mendefinisikan dependensi `spring-boot-test` secara eksplisit. Kita juga tidak perlu dependensi `junit` secara terpisah dalam `pom.xml` Anda jika kita menggunakan `spring-boot-starter-test`, karena sudah termasuk di dalamnya.

## Conclusion

Menggunakan Spring Boot Starter Test karena didalamnya sudah terdapat berbagai library _unit testing_ yang dibutuhkan dalam tahap pengembangan, seperti Junit, Spring Test, Spring Boot Test, AssertJ, Hamcrest, Mockito, JSONassert, dan JsonPath.

## References

- [What is Junit and How it works? An Overview and Its Use Cases](https://www.devopsschool.com/blog/what-is-junit-and-how-it-works-an-overview-and-its-use-cases/)

- [JUnit Tutorial | Testing Framework for java - javatpoint](https://www.javatpoint.com/junit-tutorial)

- [JUnit Tutorial for Beginners: Learn in 3 Days - Guru99](https://www.guru99.com/junit-tutorial.html)

- [Spring Boot - Starter Test - GeeksforGeeks](https://www.geeksforgeeks.org/spring-boot-starter-test/)

- [what's the difference between spring-boot-test vs spring-boot-starter ...](https://stackoverflow.com/questions/61117933/whats-the-difference-between-spring-boot-test-vs-spring-boot-starter-test)

- [Testing in Spring Boot | Baeldung](https://www.baeldung.com/spring-boot-testing)
