## Definition

library file operation mengacu pada kemampuan untuk mengelola operasi I/O (Input/Output) pada file atau data yang terletak di jaringan, seperti mengambil atau mengirim data melalui protokol jaringan seperti HTTP atau FTP.

## Spring Integration

Spring Integration adalah ekstensi dari model pemrograman Spring yang mendukung Pola Integrasi Perusahaan yang ternama. Ini memungkinkan pesan ringan dalam aplikasi berbasis Spring dan mendukung integrasi dengan sistem eksternal melalui adaptor deklaratif. Adaptor tersebut memberikan tingkat abstraksi yang lebih tinggi atas dukungan Spring untuk remote, pesan, dan penjadwalan.

Spring Integration mengambil konsep ini selangkah lebih maju, di mana POJO (Plain Old Java Object) dihubungkan bersama menggunakan paradigma pesan dan komponen individu mungkin tidak menyadari komponen lain dalam aplikasi. Aplikasi semacam itu dibangun dengan merakit komponen yang dapat digunakan kembali untuk membentuk tingkat fungsionalitas yang lebih tinggi. Dengan desain yang hati-hati, aliran ini dapat dimodularisasi dan juga digunakan kembali pada tingkat yang lebih tinggi.

Selain menghubungkan komponen berskala kecil, Spring Integration menyediakan berbagai pilihan adaptor saluran dan gateway untuk berkomunikasi dengan sistem eksternal. Adaptor Saluran digunakan untuk integrasi satu arah (kirim atau terima); gateway digunakan untuk skenario permintaan/balasan (masuk atau keluar).

Spring Integration juga digunakan sebagai mesin untuk _microservice_ yang didorong oleh pesan dalam proyek Spring Cloud Stream.

Spring Integration dapat digunakan untuk melakukan operasi berkas (file operations) dan mengintegrasikan operasi berkas ke dalam aliran data aplikasi Anda.

## Conclusion

Gunakanlah Spring Integration dalam **File Operation** dikarenakan Spring Integration juga mendukung non-blocking.

