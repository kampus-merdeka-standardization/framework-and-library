## Definition

Pemrosesan XML (Extensible Markup Language) adalah proses mengambil, memanipulasi, atau menganalisis data yang disimpan dalam format XML, yang digunakan untuk merepresentasikan struktur data hierarkis dengan elemen-elemen yang memiliki tag dan nilai terkait. Ini melibatkan parsing XML untuk mengurai dokumen XML ke dalam struktur data yang dapat diakses dan dimanipulasi oleh aplikasi.

## Jackson Core

Jackson Core adalah bagian inti dari Jackson yang mendefinisikan API Streaming serta abstraksi dasar yang digunakan oleh Jackson Data Processor. Ini juga mencakup implementasi default dari jenis handler (parser, generator) yang menangani format JSON. Abstraksi inti ini tidak spesifik JSON, meskipun penamaan mengandung 'JSON' di banyak tempat, karena alasan historis.

Paket ini adalah dasar di mana paket data-binding Jackson dibangun. Implementasi format data alternatif (seperti Smile (binary JSON), XML, CSV, Protobuf, dan CBOR) juga dibangun di atas paket dasar ini, mengimplementasikan antarmuka inti, sehingga memungkinkan penggunaan paket data-binding standar terlepas dari format data yang mendasarinya.

Untuk menggunakan paket ini, Anda perlu menggunakan dependensi Maven berikut:
```xml
<dependency>
  <groupId>com.fasterxml.jackson.core</groupId>
  <artifactId>jackson-core</artifactId>
  <version>${jackson.version.core}</version>
</dependency>
```
Kita juga dapat mengunduh jar dari repositori Maven atau tautan di Wiki. Paket ini tidak memiliki dependensi eksternal, kecuali untuk pengujian (yang menggunakan JUnit).

- [FasterXML/jackson-core: Core part of Jackson that defines Streaming API as well as basic shared abstractions](https://github.com/FasterXML/jackson-core)
- [FasterXML/jackson: Main Portal page for the Jackson project - GitHub](https://github.com/FasterXML/jackson)
- [Releases · FasterXML/jackson-core · GitHub](https://github.com/FasterXML/jackson-core/releases)