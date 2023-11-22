# Summary

## Library

### Web

Berdasarkan hasil scoring, [Fiber](https://github.com/gofiber/fiber) memiliki angka yang paling besar. Fiber memiliki hasil yang paling baik dalam benchmark. Fiber juga sudah digunakan di banyak project di **T**. Jadi Fiber adalah pilihan yang baik untuk library Web.

### Logging

Dari ketiga library logging ini, [Zap](https://github.com/uber-go/zap) adalah pilihan terbaik. Zap masih terus dan sering dilakukan update. Zap juga dibuat dan didukung oleh perusahaan besar, yaitu Uber. Zap juga sudah digunakan di banyak project milik **T**.

### Rest Client

Berdasarkan score yang didapat, [Heimdall](https://github.com/gojek/heimdall) memiliki angka yang paling besar. Selain itu, Heimdall dibuat oleh perusahaan besar yaitu Gojek. Jadi pilihan yang tepat untuk library Rest Client adalah Heimdall.

### Configuration

Berdasarkan score yang didapat, library [Viper](https://github.com/spf13/viper) memiliki angka yang paling besar. Selain itu, Viper juga compatible dengan Consul dan Vault. Jadi pilihan yang tepat untuk library logging adalah Viper.

### Monitoring

Berdasarkan score yang didapat, library [Fiberprometheus](https://github.com/ansrivas/fiberprometheus) memiliki angka yang paling besar. Selain itu, fiberprometheus juga compatible dengan project-project yang ada di **T** karena kebanyakan sudah memakai framework Fiber. Jadi pilihan yang tepat untuk library monitoring adalah Fiber.

### RDBMS

Berdasarkan score yang didapat, library [SQLx](https://github.com/jmoiron/sqlx) memiliki angka yang paling besar. Library SQLx dirancang untuk mendukung berbagai sistem database yang kompatibel dengan Golang. Jadi pilihan yang tepat untuk library RDMS adalah SQLx.

### Document Based DB

Gunakan official library yang sudah disediakan oleh Golang atau yang dibuat oleh penyedia document database tersebut.

### In-memory DB

Untuk library in-memory DB dapat menggunakan Go Redis. Library ini dirancang untuk mendukung database Redis. Selain itu, library Go Redis sudah digunakan di semua project yang ada di **T**. Jadi pilihan yang tepat untuk library in-memory DB adalah Go Redis.

### GraphDB

Gunakan official library yang sudah disediakan oleh Golang atau yang dibuat oleh penyedia graph database tersebut.

### Storage

Gunakan official library yang sudah disediakan oleh Golang atau yang dibuat oleh penyedia storage tersebut.

### File Operation

Berdasarkan score yang didapat, Go Standard Library memiliki angka yang paling besar. Go CSV adalah library yang hanya diperuntukkan untuk file CSV saja. Jadi pilihan yang tepat untuk library file-operation adalah Go Standard Library ("os" dan "io/ioutil").

### Concurrency

Berdasarkan score yang didapat, Go Standard Library memiliki angka yang paling besar. Concurrency di Golang sendiri sudah sangat baik sehingga tidak perlu menggunakan library tambahan. Jadi pilihan yang tepat untuk library concurrency adalah Go Standard Library.

### Routing

Berdasarkan score yang didapat, Go Standard Library memiliki angka yang paling besar. Routing di Golang sendiri sudah sangat baik sehingga tidak perlu menggunakan library tambahan. Tetapi jika ingin menggunakan routing pada framework, maka disarankan menggunakan Fiber. Jadi pilihan yang tepat untuk library routing adalah Go Standard Library.

### Queueing

Karena library queue biasanya disediakan oleh penyedia service tersebut, maka gunakan library yang dibuat oleh penyedia messaging queue tersebut.

### PubSub

Karena library pubsub biasanya disediakan oleh penyedia service tersebut, maka gunakan library yang dibuat oleh penyedia messaging pubsub tersebut.

### Scheduler

Dari kedua library scheduler ini, [Gocron](https://github.com/go-co-op/gocron) adalah pilihan terbaik. Gocron masih terus dan sering dilakukan update. Gocron memiliki jumlah star yang cukup banyak, yaitu 4.2k di repository github. Gocron juga sudah digunakan di banyak project milik **T**.

### CLI

Berdasarkan score yang didapat, library [Cobra](https://github.com/spf13/cobra) memiliki angka yang paling besar. Dibandingkan library yang lain, Cobra lebih populer untuk library CLI. Jadi pilihan yang tepat untuk library CLI adalah Cobra.

### XML Processing

Gunakan standard library yang sudah disediakan oleh Golang karena sudah cukup bagus tanpa perlu menggunakan library xml lain lagi.

### JSON Processing

Berdasarkan score yang didapat, library go-json memiliki angka yang paling besar. Jika dibandingkan, go-json lebih cepat daripada json-iterator. Jadi pilihan yang tepat untuk library json processing adalah go-json.

### Packaging Tools

Untuk Packaging Tools gunakan Go Modules. Go modules meruapakan manajemen dependensi resmi untuk Go.

### SDK

Berdasarkan [web resmi golang](https://go.dev/dl/), versi yang sudah stable adalah go.1.21 dan go 1.20. Jadi gunakan versi Golang 1.20 keatas.

### Unit Test

Menggunakan package [testify](https://github.com/stretchr/testify) daripada standard library Golang (testing) memberikan keuntungan tambahan dalam menulis dan menjalankan uji unit. Secara keseluruhan, penggunaan testify meningkatkan kualitas dan keterbacaan kode pengujian dalam proyek Golang, serta menyediakan alat tambahan yang mendukung praktik unit test yang lebih kuat.

## Web Framework

Saat ini web framework yang sedang ramai dibicarakan adalan Gin dan Fiber. Jika ingin memprioritaskan kinerja tinggi dan memiliki pengalaman dengan Go, Gin mungkin merupakan pilihan yang lebih baik untuk aplikasi yang kompleks dan *high traffic*. Di sisi lain, jika menginginkan kesederhanaan, *asynchronus handling*, dan minimalis, Fiber bisa menjadi pilihan yang tepat, terutama untuk proyek berukuran kecil hingga menengah. Berdasarkan score yang didapat, Fiber memiliki angka yang lebih besar. Fiber juga sudah digunakan di hampir semua project milik **T**. Jadi untuk web framework gunakan [Fiber](https://github.com/gofiber/fiber).
