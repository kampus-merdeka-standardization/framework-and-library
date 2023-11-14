# Configuration

## Definition
Dalam pengembangan perangkat lunak, "konfigurasi" merujuk pada parameter dan opsi yang menentukan bagaimana sebuah aplikasi atau sistem akan beroperasi. Ini bisa mencakup segala sesuatu mulai dari pengaturan koneksi database, environment variables, API keys, kata sandi, dan lain-lain. Konfigurasi ini biasanya dikelola sedemikian rupa sehingga bisa dengan mudah diubah tanpa harus mengubah kode program itu sendiri, memungkinkan aplikasi berjalan di berbagai lingkungan (development, testing, production, dll.) dengan sedikit atau tanpa modifikasi kode.

## Dotenv

Dotenv adalah modul yang memungkinkan Anda memuat environment variables dari file .env ke dalam process.env, membantu Anda menjaga konfigurasi aplikasi Anda terpisah dari kode. Hal ini sangat berguna untuk menyembunyikan informasi sensitif seperti kata sandi basis data atau API Key dari publik dan untuk mengatur konfigurasi yang berbeda untuk lingkungan pengembangan, pengujian, dan produksi.

## `@nestjs/config`

`@nestjs/config` adalah solusi konfigurasi untuk aplikasi NestJS yang menggunakan paket dotenv. Modul ini memfasilitasi penggunaan variabel lingkungan di dalam aplikasi NestJS Anda, menyediakan cara yang terstruktur dan terintegrasi untuk mengelola pengaturan aplikasi.

## Scoring sheet

| Kriteria | dotenv | @nestjs/config |
| --- | --- | --- |
| Maintenance | 4 | 4 |
| Reputable | 4 | 4 |
| Compatibility | 3 | 4 |
| Community | 4 | 4 |
| Documentation | 4 | 4 |
| Licensing | 4 | 4 |
| Extensible | 3 | 4 |
| Size | 4 | 4 |
| **Total Score** | **30** | **32** |

## Conclusion

Mengingat `@nestjs/config` memiliki skor yang lebih tinggi terutama dalam kompatibilitas dan ekstensibilitas dalam ekosistem NestJS, modul ini disimpulkan sebagai pilihan yang lebih baik untuk manajemen konfigurasi dalam aplikasi NestJS, menawarkan integrasi yang mulus dan pengaturan yang lebih efisien.

## Referensi

- [How to Use Node Environment Variables with a DotEnv File for Node.js and npm](https://www.freecodecamp.org/news/how-to-use-node-environment-variables-with-a-dotenv-file-for-node-js-and-npm/)
- [dotenv - npm](https://www.npmjs.com/package/dotenv)
- [dotenv - github](https://github.com/motdotla/dotenv)
- [@nestjs/config - npm](https://www.npmjs.com/package/@nestjs/config)
- [@nestjs/config - github](https://github.com/nestjs/config)