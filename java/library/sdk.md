## Definition

SDK, atau _Software Development Kit_, adalah seperangkat alat yang digunakan untuk mengembangkan aplikasi perangkat lunak. Dalam konteks Java, JDK, atau _Java Development Kit_, adalah bagian dari SDK yang digunakan khusus untuk pengembangan Java.  JDK memberikan alat dan perpustakaan yang diperlukan untuk mengembangkan aplikasi Java. Ini mencakup kompiler Java (javac), Java Virtual Machine (JVM), dan perpustakaan kelas Java standar. Oleh karena itu, jika Anda ingin mengembangkan aplikasi Java, Anda akan memerlukan JDK.

## Java 21

Java 21, yang dirilis pada 19 September 2023, adalah rilis dukungan jangka panjang (LTS) berikutnya dari implementasi Java standar Oracle. Berikut adalah beberapa fitur utama dari Java 21:

1. **Virtual Threads** telah diselesaikan. Virtual threads adalah thread ringan yang dikelola JVM yang akan membantu dalam menulis aplikasi konkuren berkinerja tinggi.
2. **Record Patterns (Project Amber)** telah diselesaikan.
3. **Pattern Matching untuk pernyataan switch** telah diselesaikan.
4. Sebuah koleksi baru, **SequencedCollection**, telah ditambahkan yang memberikan akses langsung ke elemen pertama dan terakhir dari koleksi yang diurutkan.
5. **String templates dan kelas & metode main instance tanpa nama** tersedia sebagai fitur pratinjau.
6. Fitur **Scoped values** sekarang adalah API pratinjau.
7. **Unnamed Patterns and Variables** diperkenalkan sebagai fitur pratinjau.
8. **Unnamed Classes and Instance Main Methods** diperkenalkan sebagai fitur pratinjau.
9. **Structured Concurrency** terus menjadi fitur pratinjau.

Selain itu, ada beberapa perubahan lain yang termasuk:
- **Generational ZGC** [JEP-439]
- **Pattern Matching for switch** [JEP-441]
- **Foreign Function & Memory API (Third Preview)** [JEP-442]
- **Vector API (Sixth Incubator)** [JEP-448]
- **Deprecate the Windows 32-bit x86 Port for Removal** [JEP-449]
- **Prepare to Disallow the Dynamic Loading of Agents** [JEP-451]
- **Key Encapsulation Mechanism API** [JEP-452]


## Java 17

Java 17 adalah rilis dukungan jangka panjang (LTS) terbaru untuk platform Java SE. JDK 17 dirilis pada 15 September 2021. Berikut adalah beberapa fitur utama dari Java 17:

1. **Restore Always-Strict Floating-Point Semantics (JEP 306)**: JEP ini terutama untuk aplikasi ilmiah, dan membuat operasi titik mengambang konsisten ketat.
2. **Enhanced Pseudo-Random Number Generators (JEP 356)**: JEP 356 menyediakan antarmuka dan implementasi baru untuk Pseudo-Random Number Generators (PRNG).
3. **New macOS Rendering Pipeline (JEP 382)**: JEP ini mengimplementasikan pipeline rendering internal Java 2D untuk macOS.
4. **macOS/AArch64 Port (JEP 391)**: JEP ini memindahkan JDK untuk berjalan pada AArch64 di platform macOS.
5. **Deprecate the Applet API for Removal (JEP 398)**.
6. **Switch Expressions (JEP 361)**
7. **Text Blocks (JEP 378)**
8. **Packaging Tool (JEP 392)**
9. **Pattern Matching for instanceof (JEP 394)**
10. **Records (JEP 395)**
11. **Sealed Classes (JEP 409)**

## Scoring sheet

| Komponen          | Java 21 | Java 17 |
| :---------------- | :-----: | :-----: |
| Maintenance       | 4       | 1       |
| Reputable         | 4       | 4       |
| Compatibility     | 4       | 4       |
| Community         | 4       | 4       |
| Documentation     | 4       | 4       |
| Licensing         | 4       | 4       |
| Extensible        | 4       | 4       |
| Size              | 1       | 1       |
| **Total Score**   | 29      | 26      |
| **Average Score** | 3.625   | 3.25    |

## Conclusion

Berdasarkan hasil skoring, terlihat bahwa java 21 memiliki nilai yang lebih baik. Untuk itu gunakanlah java versi 21. Java 21 juga mendukung banyak sekali fitur-fitur canggih yang sangat penting dalam proses pengembangan.

## References

- [Java 21 Features (LTS): Practical Examples and Insights - HowToDoInJava](https://howtodoinjava.com/java/java-21-new-features/)

- [JDK 17 - New Features in Java 17 - GeeksforGeeks](https://www.geeksforgeeks.org/jdk-17-new-features-in-java-17/)

- [New Features in Java 17 | Baeldung](https://www.baeldung.com/java-17-new-features)

- [New Features From Java 12 to 17 - DZone](https://dzone.com/articles/new-features-from-java-12-to-17)