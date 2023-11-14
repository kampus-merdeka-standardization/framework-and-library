# Pub / Sub

## Definition

Pub/Sub, atau Publish/Subscribe, adalah pola desain arsitektur yang digunakan dalam sistem terdistribusi untuk komunikasi asinkron antara berbagai komponen atau layanan. Dalam model Pub/Sub, memiliki dua jenis aktor utama:

1. **Publisher**: Ini adalah sumber pesan. Mereka membuat dan mengirim pesan ke sistem.
2. **Subscriber**: Ini adalah penerima pesan. Mereka menerima dan memproses pesan dari sistem.

## @nestjs/microservices Pub/Sub

Pub/Sub dalam @nestjs/microservices merujuk ke pola desain di mana pesan dikirim dari satu bagian (publisher) ke bagian lain (subscriber) melalui sistem. Dalam NestJS, Anda dapat menggunakan pola Pub/Sub untuk mengirim dan menerima pesan antara komponen independen secara asynchronous.

## Conclusion

Dikarenakan @nestjs/microservices adalah native NestJS dan memiliki berbagai fitur yang ditawarkan, @nestjs/microservices pub/sub adalah pilihan terbaik untuk implementasi pola Pub/Sub dalam pengembangan backend dengan NestJS.
