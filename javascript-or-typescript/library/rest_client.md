# Rest client : Fetch vs Axios

## Definition
Dalam era pengembangan aplikasi web modern, metode pengambilan data dari server atau API menjadi salah satu komponen kritis dalam arsitektur aplikasi. Get data dari sumber eksternal melalui HTTP adalah salah satu kegiatan yang sering dilakukan oleh aplikasi berbasis web, dan dalam JavaScript, Axios dan Fetch adalah dua pendekatan yang populer dalam menangani tugas tersebut. 

## Axios

Axios adalah library JavaScript populer yang digunakan untuk membuat get HTTP. Ini menawarkan API yang konsisten di seluruh peramban dan Node.js, mendukung fitur seperti transformasi get dan respons, pembatalan get, serta penanganan kesalahan otomatis. Berkat desainnya yang berbasis Promise, Axios memudahkan penanganan respons dan kesalahan dengan metode `then()`, `catch()`, dan `finally()`. Selain itu, Axios memiliki kemampuan untuk mengintersep get dan respons, yang memungkinkan developer untuk memodifikasi get dan respons sebelum mereka ditangani atau dikirim.

## Fetch

Fetch adalah API bawaan dari sebagian besar browser modern yang memberikan cara yang lebih modern untuk mengambil sumber daya secara asinkron melalui jaringan. Dibandingkan dengan XMLHttpRequest, pendekatan lama untuk tugas ini, Fetch menawarkan sintaks yang lebih bersih dan ringkas dengan dukungan Promise yang inheren. Dengan Fetch, developer memiliki kontrol penuh atas get, termasuk kemampuan untuk memodifikasi header, mode CORS, integritas sumber daya, dan lainnya. Sebagai bagian dari platform web, Fetch tidak memerlukan dependensi tambahan, tetapi untuk menggunakannya di lingkungan tertentu, seperti Node.js, Anda mungkin memerlukan polyfill atau implementasi alternatif.

## Scoring sheet

| Kriteria      | Axios | Fetch |
|---------------|-------|-------|
| Maintenance   | 4     | 3     |
| Reputable     | 4     | 3     |
| Compatibility | 4     | 3     |
| Community     | 4     | 3     |
| Documentation | 4     | 3     |
| Licensing     | 4     | 4     |
| Extensible    | 4     | 3     |
| Size          | 4     | 3     |
| **Total Score**   | **32**  | **25**    |

- **Maintenance**: Axios mendapatkan skor 4 karena pemeliharaannya yang rutin dan teratur. Fetch mendapatkan skor 3 karena meskipun masih dipelihara, frekuensinya tidak sebanyak Axios.
- **Reputable**: Axios dan Fetch dikembangkan oleh tim pengembang yang dikenal dan memiliki reputasi baik di komunitas JavaScript, namun Axios sedikit lebih dikenal sehingga mendapatkan skor 4, sementara Fetch mendapatkan skor 3.
- **Compatibility**: Axios sangat kompatibel dengan berbagai lingkungan JavaScript dan dapat digunakan bersamaan dengan berbagai library lainnya, sehingga mendapatkan skor 4. Fetch juga cukup kompatibel, namun mungkin memerlukan polyfill di beberapa lingkungan, sehingga mendapatkan skor 3.
- **Community**: Axios memiliki komunitas pengguna yang besar dan aktif, baik di tingkat lokal maupun global, sehingga mendapatkan skor 4. Fetch juga memiliki komunitas yang aktif, namun tidak sebesar Axios, sehingga mendapatkan skor 3.
- **Documentation**: Axios memiliki dokumentasi yang lengkap dan terstruktur dengan baik, sehingga mendapatkan skor 4. Fetch juga memiliki dokumentasi, namun mungkin tidak sejelas Axios, sehingga mendapatkan skor 3.
- **Licensing**: Axios dan Fetch adalah perangkat lunak open source, sehingga keduanya mendapatkan skor 4.
- **Extensible**: Axios mudah diperluas dan disesuaikan sesuai kebutuhan pengguna, sehingga mendapatkan skor 4. Fetch juga dapat diperluas, namun mungkin memerlukan upaya lebih, sehingga mendapatkan skor 3.
- **Size**: Ukuran Axios sangat kecil, yang membuatnya ideal untuk penggunaan di cloud, sehingga mendapatkan skor 4. Fetch juga memiliki ukuran yang kecil, namun mungkin sedikit lebih besar dibandingkan Axios, sehingga mendapatkan skor 3.

## Conclusion

Berdasarkan evaluasi skoring yang telah dilakukan antara Axios dan Fetch, Axios mendapatkan skor yang lebih tinggi di hampir semua kriteria. Dengan keunggulan dalam pemeliharaan, reputasi, kompatibilitas, dukungan komunitas, dokumentasi, fleksibilitas, dan ukuran, kami dapat menyimpulkan bahwa Axios menawarkan kelebihan yang signifikan dalam pengembangan aplikasi web modern. Oleh karena itu, kami merekomendasikan penggunaan Axios sebagai pilihan utama dalam menangani get HTTP dalam pengembangan aplikasi.