## Definition

Library configuration membantu pengembang mengelola pengaturan aplikasi, seperti variabel lingkungan, koneksi database, atau parameter lainnya. Dengan library ini, pengembang dapat dengan mudah membaca dan mengubah pengaturan tanpa harus mengubah kode sumber aplikasi.

## [GoDotEnv](https://github.com/joho/godotenv)

Sebuah port Go (golang) dari proyek Ruby dotenv (yang memuat variabel lingkungan dari file .env). Menyimpan konfigurasi dalam lingkungan adalah salah satu prinsip dari aplikasi dengan dua belas faktor. Segala sesuatu yang mungkin berubah antara lingkungan implementasi, seperti handle sumber daya untuk basis data atau kredensial untuk layanan eksternal, seharusnya diekstraksi dari kode ke dalam variabel lingkungan. Namun, tidak selalu praktis untuk mengatur variabel lingkungan di mesin pengembangan atau server integrasi berkelanjutan di mana beberapa proyek dijalankan. Dotenv memuat variabel dari file .env ke dalam ENV saat lingkungan diinisialisasi.

## [Consul](https://github.com/hashicorp/consul/tree/main)

Library Consul untuk Golang adalah sebuah library yang memungkinkan pengembang Golang untuk berinteraksi dengan 
konsul, sebuah sistem penyimpanan dan manajemen konfigurasi yang digunakan untuk tujuan penemuan layanan, konfigurasi dinamis, dan koordinasi layanan dalam arsitektur mikro atau lingkungan terdistribusi. Dengan menggunakan library ini, pengembang dapat membuat aplikasi yang dapat mendaftar layanan mereka dengan Konsul, menemukan layanan lainnya, mengambil konfigurasi yang dikelola oleh Konsul, dan melakukan berbagai operasi lainnya terkait manajemen layanan dan konfigurasi. Library ini menyediakan API yang memudahkan integrasi aplikasi Golang dengan Konsul, sehingga memungkinkan pengembang untuk membangun sistem yang lebih dinamis, terdistribusi, dan terkelola dengan baik.

## [Viper](https://github.com/spf13/viper)

Viper adalah solusi konfigurasi lengkap untuk aplikasi Go, termasuk aplikasi yang mengikuti prinsip-prinsip 12-Factor. Ini dirancang untuk bekerja di dalam aplikasi dan dapat mengatasi semua jenis kebutuhan dan format konfigurasi. Viper mendukung berbagai fitur seperti mengatur nilai default, membaca dari berkas konfigurasi JSON, TOML, YAML, HCL, envfile, dan Java properties, pemantauan langsung dan pembacaan ulang berkas konfigurasi secara real-time (opsional), membaca dari variabel lingkungan, membaca dari sistem konfigurasi jarak jauh (seperti etcd atau Consul) dan pemantauan perubahan, membaca dari bendera baris perintah, membaca dari buffer, serta menetapkan nilai-nilai eksplisit sesuai kebutuhan aplikasi Anda. Dengan Viper, pengembang Go dapat dengan mudah mengelola konfigurasi aplikasi mereka dengan fleksibilitas yang tinggi.

## Scoring sheet

| Komponen        | GoDotEnv | Consul | Viper |
|-----------------|----------|--------|-------|
| Maintenance     | 2        | 4      | 4     |
| Reputable       | 2        | 4      | 3     |
| Compatibility   | 4        | 3      | 4     |
| Community       | 4        | 3      | 4     |
| Documentation   | 4        | 4      | 3     |
| Licensing       | 4        | 3      | 4     |
| Extensible      | 4        | 4      | 4     |
| Size            | 4        | 1      | 4     |
| **Total Score** | 28       | 26     | 30    |

## Conclusion

Berdasarkan score yang didapat, library Viper memiliki angka yang paling besar. Selain itu, Viper juga compatible dengan Consul dan Vault. Jadi pilihan yang tepat untuk library logging adalah Viper.