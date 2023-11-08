# Performance Monitoring

## Definition

Performance monitoring dalam backend adalah proses mengumpulkan dan menganalisis data tentang bagaimana sistem berfungsi. Ini melibatkan pengukuran berbagai metrik seperti latency (waktu yang dibutuhkan untuk memproses permintaan), throughput (jumlah permintaan yang dapat diproses dalam satu waktu), penggunaan CPU, uptime server, dan penggunaan memori.

Latency adalah waktu yang dibutuhkan oleh paket data untuk bepergian dari satu titik ke titik lainnya pada jaringan. Ini adalah metrik kinerja penting yang mengukur responsivitas sistem. Throughput mengukur volume lalu lintas yang dapat ditangani oleh aplikasi web tanpa breakdown. Penggunaan CPU adalah waktu layanan menggunakan CPU. Server uptime adalah waktu yang dihabiskan server dalam keadaan aktif dan berfungsi. Memory adalah jumlah memori yang digunakan oleh aplikasi.

## Zipkin

Zipkin adalah sistem penelusuran terdistribusi yang dirancang untuk memudahkan pelacakan masalah latensi dalam arsitektur berbasis mikroservis. Zipkin menangkap data tentang waktu yang dibutuhkan oleh permintaan saat mereka melewati berbagai layanan, memberikan visibilitas mendalam terhadap performa internal aplikasi. Dengan Zipkin, developer dapat mengisolasi permintaan yang lambat dan menganalisis jejak permintaan lintas layanan untuk mempercepat diagnosa dan pemecahan masalah, yang krusial dalam ekosistem aplikasi modern yang kompleks dan saling terkait.

## Scoring sheet


| Kriteria       | Zipkin |
| -------------- | ------ |
| Maintenance   | 4      |
| Reputable      | 4      |
| Compatibility | 4      |
| Community      | 4      |
| Documentation    | 4      |
| Licensing        | 4      |
| Extensible| 4      |
| Ukuran         | 4      |
| **Total Skor** | **32** |

- **Maintenance**: Zipkin mendapatkan skor 4 karena memiliki pemeliharaan yang rutin dan teratur.
- **Reputable**: Sebagai proyek open source yang awalnya dikembangkan oleh Twitter dan sekarang dikelola oleh organisasi sukarelawan OpenZipkin, Zipkin mendapatkan skor 4.
- **Compatibility**: Zipkin mendukung berbagai bahasa pemrograman dan protokol, termasuk HTTP dan gRPC, sehingga mendapatkan skor 4.
- **Community**: Dengan komunitas pengguna yang besar dan aktif, Zipkin mendapatkan skor 4.
- **Documentation**: Memiliki dokumentasi yang lengkap dan terstruktur dengan baik, Zipkin mendapatkan skor 4.
- **Licensing**: Sebagai perangkat lunak open source, Zipkin mendapatkan skor 4.
- **Extensible**: Dapat diperluas dengan berbagai cara, termasuk melalui pustaka pelacak atau instrumen, Zipkin mendapatkan skor 4.
- **Size**: Memiliki ukuran yang relatif kecil, Zipkin mendapatkan skor 4.


## Conclusion

Zipkin meraih skor total yang tinggi dalam evaluasi kriteria yang penting untuk performance monitoring sistem. Hal ini menunjukkan bahwa Zipkin adalah solusi monitoring yang kuat, andal, dan efisien, sangat cocok untuk arsitektur mikroservis. Dengan komunitas yang aktif, dokumentasi yang jelas, dan pemeliharaan yang teratur, Zipkin menjanjikan peningkatan visibilitas performa aplikasi dan efisiensi dalam pemecahan masalah. Kesimpulannya, Zipkin adalah pilihan yang direkomendasikan.

## Referensi

- [Zipkin](https://zipkin.io/)
- [OpenZipkin Community](https://zipkin.io/pages/community.html)
- [Zipkin Quickstart](https://zipkin.io/pages/quickstart)
- [GitHub - openzipkin/zipkin](https://github.com/openzipkin/zipkin)
- [Zipkin Tutorial: Get Started Easily With Distributed Tracing](https://www.sentinelone.com/blog/zipkin-tutorial-distributed-tracing/)