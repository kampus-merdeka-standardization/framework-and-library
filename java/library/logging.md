## Definition

Library logging digunakan untuk mencatat peristiwa yang terjadi dalam aplikasi. Ini sangat berguna untuk pemantauan, debugging, dan analisis saat pengembang perlu mengetahui apa yang terjadi dalam aplikasi, termasuk pesan kesalahan, informasi debugging, dan jejak aktivitas.

## Logback

Logback adalah salah satu kerangka kerja logging yang paling banyak digunakan dalam Komunitas Java. Ini adalah pengganti untuk pendahulunya, Log4j. Logback menawarkan implementasi yang lebih cepat, memberikan lebih banyak opsi untuk konfigurasi, dan lebih fleksibel dalam mengarsipkan file log lama.

Logback menggunakan Simple Logging Facade for Java (SLF4J) sebagai antarmuka aslinya.

## Log4j2

Log4j2 adalah peningkatan dari Log4j yang memberikan peningkatan signifikan dibandingkan pendahulunya, Log4j 1.x. Log4j2 menyediakan banyak peningkatan yang tersedia di Logback sambil memperbaiki beberapa masalah inheren dalam arsitektur Logback.

Berikut adalah beberapa fitur utama dari Log4j21:

- **Pemisahan API**: API untuk Log4j terpisah dari implementasinya, menjadikannya jelas bagi pengembang aplikasi kelas dan metode mana yang dapat mereka gunakan sambil memastikan kompatibilitas ke depan.

- **Performa yang Ditingkatkan**: Log4j2 berisi Logger Asinkron generasi berikutnya berdasarkan perpustakaan LMAX Disruptor. Dalam skenario multi-threaded, Logger Asinkron memiliki throughput 18 kali lebih tinggi dan latensi yang jauh lebih rendah dibandingkan dengan Log4j 1.x dan Logback.

- **Dukungan untuk Beberapa API**: Meskipun API Log4j2 akan memberikan kinerja terbaik, Log4j2 memberikan dukungan untuk API Log4j 1.2, SLF4J, Commons Logging dan java.util.logging (JUL).

## Scoring sheet

| Komponen          | Logback | Log4j2 |
| :---------------- | :-----: | :----: |
| Maintenance       | 4       | 4      |
| Reputable         | 4       | 4      |
| Compatibility     | 4       | 4      |
| Community         | 4       | 4      |
| Documentation     | 4       | 4      |
| Licensing         | 4       | 4      |
| Extensible        | 4       | 4      |
| Size              | 4       | 3      |
| **Total Score**   | 32      | 31     |
| **Average Score** | 4       | 3.875  |

## Conclusion
Berdasarkan nilai skoring, tampak Logback memiliki penilaian yang lebih tinggi, akan tetapi Log4j2 memiliki sejumlah peningkatan dari Logback, terutama dalam hal vurnabilities

## References
- [A Guide To Logback | Baeldung](https://www.baeldung.com/logback)
- [Log4j – Apache Log4j™ 2](https://logging.apache.org/log4j/2.x/)