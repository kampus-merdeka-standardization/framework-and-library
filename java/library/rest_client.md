## Definition

Library rest client adalah perangkat lunak atau modul yang memungkinkan pengembang untuk berinteraksi dengan layanan RESTful API (Application Programming Interface) menggunakan bahasa pemrograman tertentu dengan mudah. Ini menyediakan fungsi dan abstraksi yang memungkinkan pengiriman permintaan HTTP seperti GET, POST, PUT, dan DELETE ke endpoint API, serta pengolahan respons yang diterima. Library rest client membantu mengotomatiskan sebagian besar tugas yang terkait dengan komunikasi dengan API, termasuk manajemen autentikasi, pengelolaan sesi, pemrosesan format data seperti JSON atau XML, serta penanganan kesalahan.

## Rest Template

`RestTemplate` adalah klien REST yang disediakan oleh Spring Framework. Ini digunakan untuk mengonsumsi API REST dan dapat melakukan berbagai operasi HTTP.

Berikut adalah beberapa metode yang disediakan oleh RestTemplate:

- GET: `getForEntity()`, `getForObject()`
- POST: `postForEntity()`, `postForLocation()`, `postForObject()`
- PUT: `put()`
- DELETE: `delete()`
- HEAD: `headForHeaders()`
- OPTIONS: `optionsForAllow()`
- PATCH: `patchForObject()`
- ANY: `exchange()`, `execute()`

Namun, perlu diperhatikan bahwa mulai dari Spring Framework 5, `RestTemplate` akan ditinggalkan dan digantikan oleh `WebClient` yang merupakan klien HTTP modern dan alternatif untuk RestTemplate. `WebClient` tidak hanya menyediakan API sinkronis tradisional, tetapi juga mendukung pendekatan nonblocking dan asinkron yang efisien

## Web Client

`WebClient` adalah antarmuka yang mewakili titik masuk utama untuk melakukan permintaan web. Ini dibuat sebagai bagian dari modul Spring Web Reactive dan akan menggantikan `RestTemplate` klasik dalam skenario ini. Selain itu, klien baru ini adalah solusi reaktif, non-blocking yang bekerja melalui protokol HTTP/1.1.

Berikut adalah beberapa cara untuk membuat instance `WebClient`:

- Membuat objek `WebClient` dengan pengaturan default: 
    ```java
    WebClient client = WebClient.create();
    ```

- Menginisiasi instance `WebClient` dengan URI dasar yang diberikan: 
    ```java
    WebClient client = WebClient.create("http://localhost:8080");
    ```

- Membangun klien dengan menggunakan kelas `DefaultWebClientBuilder`, yang memungkinkan penyesuaian penuh: 
    ```java
    WebClient client = WebClient.builder()
        .baseUrl("http://localhost:8080")
        .defaultCookie("cookieKey", "cookieValue")
        .defaultHeader(HttpHeaders.CONTENT_TYPE, MediaType.APPLICATION_JSON_VALUE)
        .defaultUriVariables(Collections.singletonMap("url", "http://localhost:8080"))
        .build();
    ```

Meskipun `WebClient` adalah klien non-blocking dan termasuk dalam pustaka `spring-webflux`, solusi ini menawarkan dukungan untuk operasi sinkronis dan asinkronis, menjadikannya cocok juga untuk aplikasi yang berjalan pada Servlet Stack. Ini dapat dicapai dengan memblokir operasi untuk mendapatkan hasil. Tentu saja, praktik ini tidak disarankan jika kita bekerja pada Reactive Stack.

## Conclusion
Dikarenakan `WebClient` akan menggantikan `RestTemplate`, maka direkomendasikan menggunakan `WebClient` sebagai library _Rest Client_ pada Java.

## References
- [Spring - RestTemplate - GeeksforGeeks](https://www.geeksforgeeks.org/spring-resttemplate/)
- [A Guide to the RestTemplate | Baeldung](https://www.baeldung.com/rest-template)
- [Spring 5 WebClient | Baeldung](https://www.baeldung.com/spring-5-webclient)
- [WebClient :: Spring Framework](https://docs.spring.io/spring-framework/reference/web/webflux-webclient.html)