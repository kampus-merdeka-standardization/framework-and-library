## Definition

Library scheduler digunakan untuk menjadwalkan tugas atau pekerjaan dalam aplikasi. Dengan menggunakan library ini, pengembang dapat mengatur eksekusi tugas pada waktu yang ditentukan atau dengan interval tertentu. Hal ini berguna untuk otomatisasi tugas-tugas terjadwal seperti pemrosesan latar belakang atau pengiriman email berkala.

## Spring Scheduler

**Spring Scheduler** adalah lapisan abstraksi yang ditulis untuk menyembunyikan implementasi Executors dalam berbagai JDK. Jika semua yang Anda butuhkan adalah untuk mengeksekusi metode pada bean setiap X detik, atau pada jadwal `cron`, maka `@Scheduled` (atau berbagai opsi dalam skema konfigurasi _task_ Spring) mungkin cukup. Spring Scheduler adalah implementasi yang benar-benar ringan yang akan memadai untuk kebutuhan penjadwalan sederhana

## Quartz Scheduler

**Quartz Scheduler** adalah kerangka kerja penjadwalan yang lengkap yang memungkinkan eksekusi tugas berbasis CRON atau periodik sederhana. Quartz adalah orde lebih kompleks daripada penjadwal bawaan Spring, termasuk dukungan untuk pekerjaan persisten, transaksional, dan terdistribusi. Quartz mungkin sedikit sulit, bahkan dengan dukungan API Spring. Namun, Quartz memberikan dukungan untuk fitur tingkat perusahaan seperti JTA dan clustering; ini datang dengan JobPersistence (penyimpanan JDBC & RAM) yang dapat digunakan untuk tujuan Fail-safe & Load Balancing.



## Scoring sheet
| Komponen          | Spring Scheduler | Quartz Scheduler |
| :---------------- | :--------------: | :--------------: | 
| Maintenance       | 3                | 1                |
| Reputable         | 4                | 3                |
| Compatibility     | 4                | 4                |
| Community         | 4                | 3                |
| Documentation     | 4                | 4                |
| Licensing         | 4                | 4                |
| Extensible        | 4                | 4                |
| Size              | 4                | 4                |
| **Total Score**   | 31               | 27               |
| **Average Score** | 3.875            | 3.375            |

## Conclusion

Berdasarkan Score di atas, _Spring scheduler_ memiliki penilaian yang lebih besar. Walau begitu _Quartz Scheduler_ memiliki lebih banyak fitur yang tidak dimiliki _Spring Scheduler_