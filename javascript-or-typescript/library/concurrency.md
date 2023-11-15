## Definition

Concurrency adalah konsep dalam pemrograman yang mengacu pada kemampuan sebuah program untuk menjalankan beberapa tugas atau potongan kode secara bersamaan, tanpa harus menunggu tugas sebelumnya selesai. Ini dapat diterapkan untuk meningkatkan efisiensi dan kinerja dalam aplikasi, terutama pada sistem dengan banyak prosesor atau pada tugas yang melibatkan I/O.

## Node.js Native Concurrency

Concurrency dalam Node.js dapat dicapai dengan menggunakan berbagai teknik, seperti menggunakan callback, promises, dan async/await.

1. **Callback**: Callback adalah fungsi yang dilewatkan sebagai argumen ke fungsi lain dan kemudian dipanggil kembali setelah operasi tertentu selesai. Ini memungkinkan Node.js untuk melanjutkan dengan operasi lain dan kemudian kembali ke callback ketika siap.

2. **Promises**: Promise adalah objek yang mewakili penyelesaian atau kegagalan operasi asinkron. Promise dapat digunakan untuk menangani operasi asinkron secara berurutan dan menangani kesalahan dengan lebih baik.

3. **Async/Await**: Async/await adalah sintaks khusus yang dibuat untuk bekerja dengan promises dengan cara yang lebih nyaman. Fungsi async memastikan bahwa fungsi mengembalikan promise, dan ekspresi await digunakan untuk menunggu promise diselesaikan.

## Conclusion

Berdasarkan penjelasan diatas, dinyatakan bahwa Node.js Native Concurrency menjadi pilihan kami untuk menghandle Concurrency.

## Referensi

- [A simple guide to JavaScript concurrency in Node.js and a few traps that come with it](https://tsh.io/blog/simple-guide-concurrency-node-js/)
