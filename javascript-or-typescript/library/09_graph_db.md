# Graph Database

## Definition

Graph Database (GDB) adalah database yang menggunakan struktur graf untuk melakukan query semantik dengan node, edge, dan properti untuk merepresentasikan dan menyimpan data. Konsep kunci dari sistem ini adalah graf (atau edge atau relationship). Graf tersebut menghubungkan item data dalam toko ke kumpulan node dan edge, edge tersebut mewakili hubungan antara node. Hubungan memungkinkan data dalam toko untuk dihubungkan secara langsung dan, dalam banyak kasus, diambil dengan satu operasi.

Graph Database memprioritaskan hubungan antara data. Query hubungan cepat karena mereka selalu disimpan dalam database. Hubungan dapat divisualisasikan secara intuitif menggunakan database graf, membuatnya berguna untuk data yang sangat saling terhubung.

## neo4j-driver

neo4j-driver adalah driver resmi yang dibuat oleh tim Neo4j untuk memungkinkan interaksi aplikasi dengan database Neo4j, yang merupakan graph database. Driver ini memfasilitasi komunikasi antara aplikasi klien (seperti aplikasi berbasis Node.js atau aplikasi lain yang menggunakan backend JavaScript) dengan instance Neo4j. Dengan menggunakan neo4j-driver, pengembang dapat terhubung ke database, menjalankan kueri Cypher, dan memanipulasi data graf dengan efisien.

## Scoring sheet

| Kriteria       | neo4j-driver |
| -------------- | ------------ |
| Maintenance   | 3            |
| Reputable       | 4            |
| Compatibility | 4            |
| Community      | 4            |
| Documentation    | 4            |
| Licensing        | 4            |
| Extensible| 4            |
| Size         | 4            |
| **Total Skor** | **31**       |

- **Maintenance**: neo4j-driver mendapatkan skor 3 karena update terakhir 10 hari yang lalu pada saat dokumen ini dibuat.
- **Reputable**: Sebagai driver resmi Neo4j untuk JavaScript, neo4j-driver mendapatkan skor 4.
- **Compatibility**: neo4j-driver mendukung protokol Bolt, yang merupakan protokol jaringan biner yang dioptimalkan untuk bekerja dengan database graf, sehingga mendapatkan skor 4.
- **Community**: Dengan komunitas pengguna yang besar dan aktif, neo4j-driver mendapatkan skor 4.
- **Documentation**: Memiliki dokumentasi yang lengkap dan terstruktur dengan baik, neo4j-driver mendapatkan skor 4.
- **Licensing**: Sebagai perangkat lunak open source, neo4j-driver mendapatkan skor 4.
- **Extensible**: neo4j-driver mudah diperluas dan mendukung berbagai fitur, sehingga mendapatkan skor 4.
- **Size**: Ukuran library neo4j-driver relatif kecil, sehingga mendapatkan skor 4.

## Conclusion

neo4j-driver adalah pilihan yang sangat baik untuk mengembangkan backend NestJS dengan fokus pada data yang sangat terhubung, menjadikannya pilihan utama kami untuk proyek yang memerlukan database graf.

## Referensi

- [What is Graph Database](https://www.geeksforgeeks.org/what-is-graph-database/)
- [Graph database](https://en.wikipedia.org/wiki/Graph_database)
- [npmjs - neo4j-driver](https://www.npmjs.com/package/neo4j-driver)
- [github - neo4j-driver](https://github.com/neo4j/neo4j-javascript-driver)
