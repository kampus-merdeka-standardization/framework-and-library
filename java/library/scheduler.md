## Definition

Library scheduler digunakan untuk menjadwalkan tugas atau pekerjaan dalam aplikasi. Dengan menggunakan library ini, pengembang dapat mengatur eksekusi tugas pada waktu yang ditentukan atau dengan interval tertentu. Hal ini berguna untuk otomatisasi tugas-tugas terjadwal seperti pemrosesan latar belakang atau pengiriman email berkala.

## Spring Scheduler

**Spring Scheduler** adalah lapisan abstraksi yang ditulis untuk menyembunyikan implementasi Executors dalam berbagai JDK. Jika semua yang Anda butuhkan adalah untuk mengeksekusi metode pada bean setiap X detik, atau pada jadwal `cron`, maka `@Scheduled` (atau berbagai opsi dalam skema konfigurasi _task_ Spring) mungkin cukup. Spring Scheduler adalah implementasi yang benar-benar ringan yang akan memadai untuk kebutuhan penjadwalan sederhana

## Quartz Scheduler

**Quartz Scheduler** adalah kerangka kerja penjadwalan pekerjaan open source yang dapat diintegrasikan dengan hampir semua aplikasi Java. Quartz dapat digunakan untuk membuat jadwal sederhana atau kompleks untuk menjalankan puluhan, ratusan, atau bahkan puluhan ribu pekerjaan. Quartz mendukung banyak fitur kelas enterprise, seperti dukungan untuk transaksi JTA dan klustering. Kita dapat membuat jadwal kompleks untuk menjalankan pekerjaan apa pun.


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

## References
- [A Guide to the Spring Task Scheduler | Baeldung](https://www.baeldung.com/spring-task-scheduler)
- [Quartz Enterprise Job Scheduler](https://www.quartz-scheduler.org/)
- [Introduction to Quartz | Baeldung](https://www.baeldung.com/quartz)