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

## Conclusion

Berdasarkan evaluasi skoring yang telah dilakukan antara Axios dan Fetch, Axios mendapatkan skor yang lebih tinggi di hampir semua kriteria. Dengan keunggulan dalam pemeliharaan, reputasi, kompatibilitas, dukungan komunitas, dokumentasi, fleksibilitas, dan ukuran, kami dapat menyimpulkan bahwa Axios menawarkan kelebihan yang signifikan dalam pengembangan aplikasi web modern. Oleh karena itu, kami merekomendasikan penggunaan Axios sebagai pilihan utama dalam menangani get HTTP dalam pengembangan aplikasi.
