# Summary

## Library

### Web

Berdasarkan skoring yang tinggi di berbagai kriteria evaluasi untuk `@nestjs/platform-express`, kami dapat menyimpulkan bahwa library ini menawarkan standar kualitas yang sangat tinggi. Dengan performa yang impresif dalam hal pemeliharaan, reputasi, kompatibilitas, dukungan komunitas, dokumentasi, lisensi, fleksibilitas, dan ukuran, `@nestjs/platform-express` memenuhi banyak kebutuhan yang diharapkan oleh pengembang modern. Oleh karena itu, kami merekomendasikan `@nestjs/platform-express` sebagai solusi yang cocok untuk pengembangan aplikasi backend yang handal, efisien, dan scalable menggunakan framework NestJS.

### Logging

Pino mungkin lebih sesuai untuk aplikasi dengan model layanan tanpa server (serverless) atau aplikasi berbasis event, sementara Winston mungkin lebih cocok untuk aplikasi web tradisional atau aplikasi dengan infrastruktur yang lebih kompleks. Jadi pilihan jatuh kepada Pino.

### Rest Client

Berdasarkan evaluasi skoring yang telah dilakukan antara Axios dan Fetch, Axios mendapatkan skor yang lebih tinggi di hampir semua kriteria. Dengan keunggulan dalam pemeliharaan, reputasi, kompatibilitas, dukungan komunitas, dokumentasi, fleksibilitas, dan ukuran, kami dapat menyimpulkan bahwa Axios menawarkan kelebihan yang signifikan dalam pengembangan aplikasi web modern. Oleh karena itu, kami merekomendasikan penggunaan Axios sebagai pilihan utama dalam menangani get HTTP dalam pengembangan aplikasi.

### Configuration

Mengingat `@nestjs/config` memiliki skor yang lebih tinggi terutama dalam kompatibilitas dan ekstensibilitas dalam ekosistem NestJS, modul ini disimpulkan sebagai pilihan yang lebih baik untuk manajemen konfigurasi dalam aplikasi NestJS, menawarkan integrasi yang mulus dan pengaturan yang lebih efisien.

### Monitoring

Berdasarkan penjeleasan diatas menunjukkan bahwa Zipkin adalah solusi monitoring yang kuat, andal, dan efisien, sangat cocok untuk arsitektur mikroservis. Dengan komunitas yang aktif, dokumentasi yang jelas, dan pemeliharaan yang teratur, Zipkin menjanjikan peningkatan visibilitas performa aplikasi dan efisiensi dalam pemecahan masalah. Kesimpulannya, Zipkin adalah pilihan yang direkomendasikan.

### RDBMS

Dengan skor yang tinggi dalam ekstensibilitas dan kompatibilitas, serta dukungan kuat untuk TypeScript, TypeORM terpilih sebagai ORM paling sesuai untuk pengembangan backend NestJS, menawarkan skalabilitas dan pemeliharaan yang efisien untuk proyek-proyek modern.

### Document Based DB

Dikarenakan Mongoose adalah ODM yang sempurna, Keandalan dan dukungan luas yang diberikan oleh Mongoose membuatnya menjadi solusi ODM yang sangat cocok untuk aplikasi yang memanfaatkan MongoDB sebagai database berbasis dokumen.

### In-memory DB

Berdasarkan skor yang tinggi pada setiap kriteria penilaian, ioredis terpilih sebagai klien Redis utama untuk pengembangan backend menggunakan NestJS. Kemampuannya yang kuat, fitur-fitur lengkap, dan dukungan komunitas yang solid menjadikannya pilihan yang handal untuk proyek-proyek yang memerlukan database in-memory dengan akses yang cepat dan efisien.

### GraphDB

neo4j-driver adalah pilihan yang sangat baik untuk mengembangkan backend NestJS dengan fokus pada data yang sangat terhubung, menjadikannya pilihan utama kami untuk proyek yang memerlukan database graf.

### Storage

MinIO terbukti sebagai solusi penyimpanan objek yang ideal untuk proyek backend yang menggunakan NestJS. Kinerja, kompatibilitas tinggi dengan Amazon S3, dokumentasi yang komprehensif, dan dukungan komunitas yang kuat menjadikannya pilihan yang tepat bagi pengembang yang membutuhkan penyimpanan objek berkinerja tinggi dan dapat diandalkan.

### File Operation

Dikarenakan Multer satu-satunya sebagai pembanding dan tidak ada komparasi lain, Multer menjadi pilihan utama untuk operasi file pada proyek backend yang menggunakan NestJS.

### Concurrency

Berdasarkan hasil, dinyatakan bahwa Node.js Native Concurrency menjadi pilihan kami untuk menghandle Concurrency.

### Routing

Dikarenakan @nestjs/microservices adalah native NestJS dan memiliki berbagai fitur yang ditawarkan, kami menyimpulkan bahwa @nestjs/common Routing adalah pilihan utama untuk mengembangkan backend dengan menggunakan NestJS karena kompatibilitas, keandalan, dan dukungan komunitas yang luas. Lisensi open-source MIT, dokumentasi yang komprehensif, serta kemudahan ekstensi dan pemeliharaan yang teratur menjadikan @nestjs/common Routing solusi yang sangat efektif dan ramah pengembang dalam membangun arsitektur aplikasi yang kuat dan skalabel.

### Queueing

Dikarenakan @nestjs/microservices adalah native NestJS dan memiliki berbagai fitur yang ditawarkan, kami menyimpulkan bahwa @nestjs/microservices queue adalah pilihan utama untuk pengembangan proyek backend menggunakan NestJS.

### PubSub

Dikarenakan @nestjs/microservices adalah native NestJS dan memiliki berbagai fitur yang ditawarkan, @nestjs/microservices pub/sub adalah pilihan terbaik untuk implementasi pola Pub/Sub dalam pengembangan backend dengan NestJS.

### Scheduler

Dikarenakan @nestjs/schedule adalah native NestJS dan memiliki berbagai fitur yang ditawarkan, paket ini merupakan pilihan yang sangat baik untuk kebutuhan scheduling dalam pengembangan backend menggunakan NestJS.

### CLI

Mengingat @nestjs/cli adalah native dan pilihan satu-satunya, kami merekomendasikan penggunaan @nestjs/cli sebagai alat bantu pengembangan utama untuk proyek backend NestJS.

### XML Processing

Dikarenakan NestJS memiliki XML parser bawaaan, jadi pilihan utama tetap menggunakan XML yang berada pada native NestJS.

### JSON Processing

Karena Native Json Parser sudah baik dan teruji, jadi kami memilih Native Json Parser sebagai Library Json Parser/Builder.

### Packaging Tools

Dikarenakan skoring npm lebih tinggi dan memiliki banyak fitur, jadi kami memilih npm sebagai Packaging Tools utama.

### SDK

Untuk Node JS version, kami memilih versi 20.9.0 LTS sebagai acuan untuk digunakan pada proyek-proyek kedepannya.

### Unit Test

Berdasarkan skor tinggi yang diperoleh oleh Jest dan beragam fitur yang ditawarkannya, kami menyimpulkan bahwa Jest adalah pilihan utama untuk pengembangan proyek backend menggunakan NestJS. Kombinasi antara keandalan, kompatibilitas, dan komunitas yang kuat membuat **Jest** menjadi alat yang sangat efektif untuk unit testing dalam lingkungan Node.js, khususnya dengan NestJS.

## Framework

NestJS dan Express.js masing-masing memiliki kekuatan yang membuat mereka cocok untuk skenario pengembangan yang berbeda. Jika proyek Anda adalah aplikasi skala besar yang memerlukan struktur yang ketat, keselarasan dengan TypeScript, atau memanfaatkan arsitektur microservices dan integrasi dengan teknologi seperti GraphQL atau WebSockets, NestJS adalah pilihan yang tepat.

Di sisi lain, untuk aplikasi yang lebih ringan, yang memerlukan pengembangan cepat dan prototipe, atau ketika Anda membutuhkan fleksibilitas tinggi dalam kustomisasi dan pemilihan library, Express.js menawarkan pendekatan yang lebih sederhana dan kontrol yang lebih besar.
