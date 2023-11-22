## Definition

Library logging digunakan untuk mencatat peristiwa yang terjadi dalam aplikasi. Ini sangat berguna untuk pemantauan, debugging, dan analisis saat pengembang perlu mengetahui apa yang terjadi dalam aplikasi, termasuk pesan kesalahan, informasi debugging, dan jejak aktivitas.

## [Zap](https://github.com/uber-go/zap)

Zap adalah library logging yang sangat efisien dan fleksibel untuk bahasa pemrograman Go (Golang). Dirancang untuk kinerja tinggi, Zap memungkinkan pengembang untuk dengan mudah menggabungkan log ke dalam aplikasi mereka dengan overhead yang minimal. Dengan fitur-fitur seperti log level, rotasi log, dan dukungan untuk multiple output, Zap memberikan kontrol tinggi atas bagaimana dan di mana log disimpan. Zap sering digunakan dalam pengembangan aplikasi Go yang memerlukan penanganan log yang cepat dan andal.

## [Zerolog](https://github.com/rs/zerolog)

Paket zerolog menyediakan logger yang cepat dan sederhana yang ditujukan untuk keluaran JSON. API Zerolog dirancang untuk memberikan pengalaman pengembangan yang baik dan kinerja yang luar biasa. API rantai yang unik memungkinkan zerolog untuk menulis peristiwa log JSON (atau CBOR) dengan menghindari alokasi dan refleksi. Perpustakaan zap dari Uber memunculkan pendekatan ini. Zerolog mengambil konsep ini ke level berikutnya dengan API yang lebih mudah digunakan dan kinerja yang bahkan lebih baik.

## [Logrus](https://github.com/sirupsen/logrus)

Logrus adalah logger terstruktur untuk Go (golang), sepenuhnya kompatibel dengan API standar dari library logger Go. Saat ini, Logrus berada dalam mode pemeliharaan. Logrus tidak akan memperkenalkan fitur-fitur baru. Namun, ini tidak berarti Logrus sudah mati. Logrus akan tetap dipelihara untuk keamanan, perbaikan bug (dengan kompatibilitas ke belakang), dan peningkatan kinerja.

## Scoring sheet

| Komponen        | Zap | Zerolog | Logrus |
|-----------------|-----|---------|--------|
| Maintenance     | 4   | 4       | 2      |
| Reputable       | 4   | 3       | 3      |
| Compatibility   | 4   | 4       | 4      |
| Community       | 4   | 3       | 4      |
| Documentation   | 4   | 3       | 3      |
| Licensing       | 4   | 4       | 4      |
| Extensible      | 4   | 2       | 2      |
| Size            | 4   | 4       | 4      |
| **Total Score** | 32  | 27      | 26     |

## Conclusion

Dari ketiga library logging ini, Zap adalah pilihan terbaik. Zap masih terus dan sering dilakukan update. Zap juga dibuat dan didukung oleh perusahaan besar, yaitu Uber. Zap juga sudah digunakan di banyak project milik Telkomsel.