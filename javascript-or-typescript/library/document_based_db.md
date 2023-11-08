# Document Based Database

## Definition

Database berbasis dokumen atau Document-based database adalah jenis database NoSQL yang dirancang untuk menyimpan, mengambil, dan mengelola data berorientasi dokumen. Dokumen ini biasanya disimpan dalam format yang mirip dengan JSON (JavaScript Object Notation).

Database berbasis dokumen lebih efisien dan fleksibel dibandingkan dengan database relasional tradisional. Mereka memungkinkan Anda untuk menyimpan data dalam struktur yang lebih dekat dengan data dalam kode Anda, yang berarti Anda tidak perlu melakukan banyak pemetaan kompleks atau join ketika Anda mengambil atau memperbarui data.


## Mongoose

Mongoose adalah sebuah Object Document Mapper (ODM) yang biasanya digunakan dalam aplikasi Node.js dengan database MongoDB. MongoDB adalah contoh dari database berbasis dokumen. 

Dalam database berbasis dokumen seperti MongoDB, data disimpan dalam format yang mirip dengan JSON. Mongoose memungkinkan Anda untuk mendefinisikan objek dengan skema yang benar-benar diketik yang dipetakan ke sebuah dokumen MongoDB. 

Jadi, hubungan antara Mongoose dan database berbasis dokumen adalah bahwa Mongoose bertindak sebagai perantara antara aplikasi Node.js dan database berbasis dokumen (dalam hal ini, MongoDB), memungkinkan aplikasi untuk berinteraksi dengan database dengan cara yang lebih mudah dan terstruktur.

## Scoring sheet

| Kriteria       | Mongoose |
| -------------- | -------- |
| Maintenance   | 4   |
| Reputable       | 4   |
| Compatibility | 4   |
| Community      | 4   |
| Documentation    | 4   |
| Licensing        | 4  |
| Extensible| 4   |
| Size         | 4   |
| **Total Skor** | **32**   |

- **Maintenance**: Mongoose mendapatkan skor 4 karena pemeliharaannya yang rutin dan teratur. Versi terbaru, Mongoose 8.0.0, dirilis pada 31 Oktober 2023.
- **Reputable**: Sebagai library yang banyak digunakan oleh pengembang di seluruh dunia, Mongoose mendapatkan skor 4.
- **Compatibility**: Mongoose mendukung Node.js dan Deno (alpha), sehingga mendapatkan skor 4.
- **Community**: Dengan komunitas pengguna yang besar dan aktif, Mongoose mendapatkan skor 4.
- **Documentation**: Memiliki dokumentasi yang lengkap dan terstruktur dengan baik, Mongoose mendapatkan skor 4.
- **Licensing**: Mongoose adalah open source jadi mendapatkan skor 4
- **Extensible**: Mongoose mudah untuk diperluas, sehingga mendapatkan skor 4.
- **Size**: Size library Mongoose cukup kecil, sehingga mendapatkan skor 4.

## Conclusion

Dengan pertimbangan total skor yang tinggi, khususnya dalam hal pemeliharaan, reputasi, dan komunitas, Mongoose terpilih sebagai pilihan utama untuk mengembangkan proyek backend menggunakan Node.js. Keandalan dan dukungan luas yang diberikan oleh Mongoose membuatnya menjadi solusi ODM yang sangat cocok untuk aplikasi yang memanfaatkan MongoDB sebagai database berbasis dokumen.

## Referensi

- [Mongoose - npm](https://www.npmjs.com/package/mongoose)
- [Mongoose - github](https://github.com/Automattic/mongoose)
- [Mongoose, MongoDB object modeling buat NodeJS](https://medium.com/@ekaprasasti/mongoose-mongodb-object-modeling-buat-nodejs-83627f521e26)
- [Mongoose official website](https://mongoosejs.com/)