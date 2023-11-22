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

## Unit Test Rules

Dalam mengembangkan unit test, terdapat beberapa praktik terbaik yang membentuk aturan-aturan umum untuk memastikan efektivitas dan keterpeliharaan tes tersebut.

Unit test bersifat independen dan terisolasi, artinya setiap tes berdiri sendiri dan tidak bergantung pada hasil tes lainnya. Disarankan menggunakan mock untuk mengisolasi dependensi eksternal. Kemudian setiap unit test harus berfokus pada satu fitur atau kasus penggunaan spesifik, dengan nama tes yang jelas dan deskriptif untuk memudahkan pemahaman.

Penting juga untuk memperhatikan cakupan (*coverage*) dari unit test yang dibuat. Cakupan mengacu pada sejauh mana kode sumber aplikasi yang diuji oleh unit test. Praktik terbaik adalah *coverage* mencapai 85% atau lebih.

Praktik terbaik dalam penerapan unit test pada Java adalah menamakan class berakhiran **Test**, misal **AuthControllerTest**. Dan juga, gunakan _default package visibility_ untuk meningkatkan _readability_ baik pada **class**, maupun **method**. Maksudnya adalah tidak perlu menulis seperti **public**, **protected**, dan lain-lainnya baik pada **class** maupun **method**.

## How To Install

Untuk library _unit testing_ Java yang digunakan adalah **Spring Boot Test**. Cara menggunakannya adalah dengan menambahkan dependency berikut pada `pom.xml` bila menggunakan _build tool_ `maven`

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-test</artifactId>
    <scope>test</scope>
</dependency>
```

apa bila menggunakan gradle, tambahkan dependency berikut pada `build.gradle`

```kotlin
testImplementation("org.springframework.boot:spring-boot-starter-test")
```

_Note_: Biasanya kita tidak perlu menambahkan _dependency_ tersebut bila membuat proyek spring melalui [Spring Initializer](https://start.spring.io/), karena sudah ditambahkan otomatis.

## How To Use
Karena Spring boot test berisikan berbagai library test yang kita butuhkan, kita cukup meng-`import` _library_ yang sedang kita butuhkan. Seperti:

```java
import org.junit.jupiter.api.Assertions;
import org.hamcrest;
```

gunakan perintah `./mvnw test` pada terminal:
```sh
./mvnw test
```

### true/false
```java
import org.junit.jupiter.api.Assertions;
import org.junit.jupiter.api.Test;

class TrueAndFalseTest {
    @Test
    void testTrueAndFalse() {
        var trueResult = (1 == 1);
        var falseResult = (1 == 2);
        Assertions.assertTrue(trueResult);
        Assertions.assertFalse(falseResult);
    }
}
```


### same/diff
```java
import org.junit.jupiter.api.Assertions;
import org.junit.jupiter.api.Test;

class SameOrDiffTest {

    @Test
    void testValuesAreEquals() {
        var value1 = 42;
        var value2 = 42;
        
        Assertions.assertEquals(value1, value2);
    }

    @Test
    void testValuesAreNotEquals() {
        var value1 = 42;
        var value2 = 24;

        Assertions.assertNotEquals(value1, value2);
    }

    @Test
    void testValuesAreSame() {
        var name1 = new String("Naufal");
        var name2 = name1;

        Assertions.assertSame(name1, name2);
    }

    @Test
    void testValuesAreNotSame() {
        var name1 = new String("Naufal");
        var name2 = new String("Naufal");

        Assertions.assertNotSame(name1, name2);
    }

}
```

Perbedaan penggunaan `Equals` dengan `Same`, adalah:
- `Equals`: Membandingkan nilainya, apakah sama, apakah berbeda.
- `Same`: Memeriksa apakah kedua referensi objek merujuk pada objek yang sama di memori.

### error/not-error
```java
import org.junit.jupiter.api.Assertions;
import org.junit.jupiter.api.Test;

class ErrorAndNotErrorTest {

    @Test
    void TestErrorOccured() {
        var error = "ERROR";

        Assertions.assertThrows(Error.class, () -> {
            switch (error) {
                case "ERROR" -> throw new Error("Terjadi kesalahan");
            }
        });
    }

    @Test
    void TestNoErrorOccured() {
        var error = "NOT_ERROR";

        Assertions.assertDoesNotThrow(() -> {
            switch (error) {
                case "ERROR" -> throw new Error("Terjadi kesalahan");
            }
        });
    }

}
```

### null/not null
```java
import org.junit.jupiter.api.Assertions;
import org.junit.jupiter.api.Test;

class NullAndNotNullTest {

    @Test
    void TestNull() {
        String name = null;
        Assertions.assertNull(name);
    }

    @Test
    void TestNotNull() {
        String name = "Naufal";
        Assertions.assertNotNull(name);
    }

}
```

## References

- [What is Junit and How it works? An Overview and Its Use Cases](https://www.devopsschool.com/blog/what-is-junit-and-how-it-works-an-overview-and-its-use-cases/)

- [JUnit Tutorial | Testing Framework for java - javatpoint](https://www.javatpoint.com/junit-tutorial)

- [JUnit Tutorial for Beginners: Learn in 3 Days - Guru99](https://www.guru99.com/junit-tutorial.html)

- [Spring Boot - Starter Test - GeeksforGeeks](https://www.geeksforgeeks.org/spring-boot-starter-test/)

- [what's the difference between spring-boot-test vs spring-boot-starter ...](https://stackoverflow.com/questions/61117933/whats-the-difference-between-spring-boot-test-vs-spring-boot-starter-test)

- [Testing in Spring Boot | Baeldung](https://www.baeldung.com/spring-boot-testing)
