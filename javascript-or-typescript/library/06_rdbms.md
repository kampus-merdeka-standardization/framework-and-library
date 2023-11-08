# RDBMS

## Definition

Dalam pengembangan aplikasi berbasis Node.js, memilih sebuah ORM yang tepat adalah salah satu keputusan penting yang akan mempengaruhi bagaimana kita berinteraksi dengan basis data dan menentukan struktur dari kode basis data kita. Sequelize, TypeORM, dan Prisma adalah tiga ORM yang populer dalam ekosistem Node.js, masing-masing menawarkan pendekatan yang berbeda dalam menangani interaksi basis data. 

## Sequilize

Sequelize adalah ORM yang multi SQL dialect yang mendukung PostgreSQL, MySQL, MariaDB, SQLite, dan MSSQL dan memiliki fitur OOP yang solid, seperti Class dan Instance, yang memungkinkan kita untuk menulis kode yang modular dan reusable. 

## TypeORM

TypeORM adalah ORM yang sangat fleksibel dan modular, menawarkan dukungan luas untuk berbagai database SQL dan NoSQL dan fokus pada dukungan TypeScript, memungkinkan pengembangan aplikasi dengan fitur ES6 modern dan pengecekan tipe statis.

## Prisma

Prisma, di sisi lain, adalah pendatang baru yang menawarkan pendekatan yang berbeda dari ORM tradisional, di mana ia bertindak sebagai layer query builder yang menghasilkan akses data yang aman dan efisien, dengan dukungan kuat untuk TypeScript dan flow-typing.


## Scoring sheet


| Kriteria      | Sequelize | TypeORM | Prisma |
|---------------|-----------|---------|--------|
| Maintenance   | 4         | 4       | 4      |
| Reputable     | 4         | 4       | 4      |
| Compatibility | 4         | 4       | 4      |
| Community     | 4         | 4       | 4      |
| Documentation | 4         | 4       | 4      |
| Licensing     | 4         | 4       | 4      |
| Extensible    | 3         | 4       | 3      |
| Size          | 3         | 3       | 3      |
| **Total Score**   | **30**      | **31**    | **30**    |

- **Maintenance**: Sequelize, TypeORM, dan Prisma semuanya mendapatkan skor 4 karena pemeliharaannya yang rutin dan teratur.
- **Reputable**: Ketiga library ini dikembangkan oleh tim pengembang yang dikenal dan memiliki reputasi baik di komunitas Node.js, sehingga semuanya mendapatkan skor 4.
- **Compatibility**: Sequelize, TypeORM, dan Prisma semuanya sangat kompatibel dengan berbagai lingkungan dan dapat digunakan bersamaan dengan berbagai library lainnya, sehingga semuanya mendapatkan skor 4.
- **Community**: Ketiga library ini memiliki komunitas pengguna yang besar dan aktif, baik di tingkat lokal maupun global, sehingga semuanya mendapatkan skor 4.
- **Documentation**: Sequelize, TypeORM, dan Prisma semuanya memiliki dokumentasi yang lengkap dan terstruktur dengan baik, sehingga semuanya mendapatkan skor 4.
- **Licensing**: Sequelize, TypeORM, dan Prisma semuanya adalah perangkat lunak open source, sehingga semuanya mendapatkan skor 4.
- **Extensible**: Sequelize dan Prisma mendapatkan skor 3 karena meskipun dapat diperluas, mungkin memerlukan upaya lebih untuk melakukan hal tersebut. Di sisi lain, TypeORM mendapatkan skor 4 karena lebih mudah diperluas.
- **Size**: Ukuran Sequelize, TypeORM, dan Prisma relatif kecil, yang membuatnya ideal untuk penggunaan di cloud, sehingga semuanya mendapatkan skor 3.

## Conclusion

Dengan skor yang tinggi dalam ekstensibilitas dan kompatibilitas, serta dukungan kuat untuk TypeScript, TypeORM terpilih sebagai ORM paling sesuai untuk pengembangan backend NestJS, menawarkan skalabilitas dan pemeliharaan yang efisien untuk proyek-proyek modern.

## Referensi

- [Sequelize Documentation](https://sequelize.org/master/)
- [TypeORM Documentation](https://typeorm.io/#/)
- [Prisma Documentation](https://www.prisma.io/docs/)
- [Prisma vs. TypeORM – Which is Right For You?](https://spin.atomicobject.com/2023/08/22/prisma-vs-typeorm/)
- [Battle of the Node.js ORMs: Sequelize vs TypeORM](https://dev.to/victor1890/battle-of-the-nodejs-orms-sequelize-vs-typeorm-35ng)
- [Npm Trends: Prisma vs Sequelize vs Typeorm usage](https://npmtrends.com/prisma-vs-sequelize-vs-typeorm)