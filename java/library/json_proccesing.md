## Definition

Pemrosesan JSON (JavaScript Object Notation) adalah proses yang melibatkan pengambilan, penguraian, dan manipulasi data yang disimpan dalam format JSON, yang merupakan format data ringan dan mudah dibaca oleh manusia dan mesin. Pemrosesan JSON melibatkan parsing JSON untuk mengonversi data JSON menjadi struktur data yang dapat diakses dan dimanipulasi oleh aplikasi, serta menghasilkan data JSON dari struktur data aplikasi.

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

## Conclusion
Memilih library `Jackson Core`. Karena `Jackson Core` memberikan kontrol penuh dan fleksibilitas kepada developer untuk memproses JSON sesuai dengan kebutuhan aplikasi. Developer dapat menentukan bagaimana cara mengurai, memvalidasi, mengubah, atau memanipulasi data JSON dengan mudah dan efisien. Selain itu, library Jackson Core juga mendukung berbagai format JSON, seperti JSON standar, JSON kompak (Smile), JSON biner (CBOR), dan JSON dengan komentar. Library Jackson Core juga kompatibel dengan library Jackson lainnya, seperti Jackson Databind dan Jackson Annotation, yang menyediakan fitur tambahan seperti data binding, konversi, dan anotasi.

- [FasterXML/jackson-core: Core part of Jackson that defines Streaming API as well as basic shared abstractions](https://github.com/FasterXML/jackson-core)
- [FasterXML/jackson: Main Portal page for the Jackson project - GitHub](https://github.com/FasterXML/jackson)
- [Releases · FasterXML/jackson-core · GitHub](https://github.com/FasterXML/jackson-core/releases)
- [Processing JSON With Jackson - DZone](https://dzone.com/articles/processing-json-with-jackson)
- [FasterXML/jackson: Main Portal page for the Jackson project - GitHub](https://github.com/FasterXML/jackson)