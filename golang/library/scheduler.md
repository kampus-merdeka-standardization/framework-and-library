## Definition

Library scheduler digunakan untuk menjadwalkan tugas atau pekerjaan dalam aplikasi. Dengan menggunakan library ini, pengembang dapat mengatur eksekusi tugas pada waktu yang ditentukan atau dengan interval tertentu. Hal ini berguna untuk otomatisasi tugas-tugas terjadwal seperti pemrosesan latar belakang atau pengiriman email berkala.

## [Gocron](https://github.com/go-co-op/gocron)

Gocron adalah package scheduler yang memungkinkan menjalankan fungsi-fungsi Go pada interval yang telah ditentukan 
menggunakan sintaks yang sederhana dan mudah dimengerti. Gocron adalah implementasi penjadwalan tugas dalam bahasa Go yang mirip dengan modul clockwork dalam Ruby dan paket penjadwalan tugas schedule dalam Python.

## [Obfigcron](https://github.com/robfig/cron)

Library cron untuk go, yang merupakan proyek open source yang dapat digunakan untuk menjadwalkan pekerjaan yang berulang berdasarkan ekspresi cron.

## Scoring sheet

| Komponen        | Gocron | Obfigcron |
|-----------------|-----|---------|
| Maintenance     | 4   | 1       |
| Reputable       |  2  |  1      |
| Compatibility   |  4  |  4      |
| Community       | 3   |   2     |
| Documentation   |  3  |   3     |
| Licensing       |  4  |   4     |
| Extensible      | 4   |   4     |
| Size            | 4   |    4    |
| **Total Score** | 28  | 23      |

## Conclusion

Dari kedua library scheduler ini, Gocron adalah pilihan terbaik. Gocron masih terus dan sering dilakukan update. Gocron memiliki jumlah star yang cukup banyak, yaitu 4.2k di repository github. Gocron juga sudah digunakan di banyak project milik Telkomsel.