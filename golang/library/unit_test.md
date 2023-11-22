## Definition

Unit testing adalah proses pengujian pada tingkat komponen atau unit individu dalam backend. Unit yang dimaksud bisa berupa kode, fungsi, metode, prosedur, modul, atau objek tersendiri. Tujuan dari pengujian ini adalah untuk memvalidasi bahwa setiap unit kode software sudah bisa bekerja sesuai harapan.

## Testify

Package testify di Go adalah sebuah package unit test eksternal yang populer dan kuat yang menyediakan berbagai fungsi dan utilitas untuk membantu dalam menulis unit test yang lebih bersih dan mudah dipahami. Package ini dapat diintegrasikan dengan kerangka pengujian standar Go (testing) dan memberikan beberapa fitur tambahan yang mempermudah pengujian.

## Conclusion

Menggunakan package testify daripada standard library Golang (testing) memberikan keuntungan tambahan dalam menulis dan menjalankan uji unit. Secara keseluruhan, penggunaan testify meningkatkan kualitas dan keterbacaan kode pengujian dalam proyek Golang, serta menyediakan alat tambahan yang mendukung praktik unit test yang lebih kuat.

## Unit Test Rules

Dalam mengembangkan unit test, terdapat beberapa praktik terbaik yang membentuk aturan-aturan umum untuk memastikan efektivitas dan keterpeliharaan tes tersebut.

Unit test bersifat independen dan terisolasi, artinya setiap tes berdiri sendiri dan tidak bergantung pada hasil tes lainnya. Disarankan menggunakan mock untuk mengisolasi dependensi eksternal. Kemudian setiap unit test harus berfokus pada satu fitur atau kasus penggunaan spesifik, dengan nama tes yang jelas dan deskriptif untuk memudahkan pemahaman.

Penting juga untuk memperhatikan cakupan (*coverage*) dari unit test yang dibuat. Cakupan mengacu pada sejauh mana kode sumber aplikasi yang diuji oleh unit test. Praktik terbaik adalah *coverage* mencapai 85% atau lebih.

## How To Install

Untuk library unit testing Golang yang digunakan adalah [testify](https://github.com/stretchr/testify). Secara keseluruhan, penggunaan testify meningkatkan kualitas dan keterbacaan kode pengujian dalam proyek Golang, serta menyediakan alat tambahan yang mendukung praktik unit test yang lebih kuat.

Untuk install Testify, gunakan `go get`:
```sh
go get github.com/stretchr/testify
```

*Packages* berikut akan tersedia di project:
```sh
github.com/stretchr/testify/assert
github.com/stretchr/testify/require
github.com/stretchr/testify/mock
github.com/stretchr/testify/suite
github.com/stretchr/testify/http (deprecated)
```

## How To Use

File untuk keperluan testing dipisah dengan file utama, namanya harus berakhiran `_test.go`, dan package-nya harus sama. Unit test di Go dituliskan dalam bentuk fungsi, yang memiliki parameter yang bertipe `*testing.T`, dengan nama fungsi harus diawali kata **Test**. 

Untuk menggunakan _library_ testify *Import* `testify/assert` *package* ke dalam code:

```go
package name

import (
    "testing"
    "github.com/stretchr/testify/assert"
)
```

Gunakan perintah `go test` di terminal untuk menjalankan test:

```sh
go test
```

### true/false

```go
package mypackage

import (
	"testing"
	"github.com/stretchr/testify/assert"
)

func TestMyFunction(t *testing.T) {

	result := someFunction()

	// Assert bahwa hasil adalah true
	assert.True(t, result)

	// Atau assert bahwa hasil adalah false
	assert.False(t, result)
}
```

### same/diff

```go
func TestValuesAreEqual(t *testing.T) {
    value1 := 42
    value2 := 42

    assert.Equal(t, value1, value2, "Values should be equal")
}

func TestValuesAreNotEqual(t *testing.T) {
    value1 := 42
    value2 := 24

    assert.NotEqual(t, value1, value2, "Values should not be equal")
}
```

### error/not-error

```go
// Test untuk error
func TestErrorOccurred(t *testing.T) {
    err := someFunction()

    // Gunakan assert.Error untuk check terjadi error
    assert.Error(t, err, "Expected an error but got none")
}

// Test untuk no error
func TestNoErrorOccurred(t *testing.T) {
    err := anotherFunction()

    // Gunakan assert.NoError untuk check tidak ada error
    assert.NoError(t, err, "Expected no error but got one")
}
```

### nil/not nil

```go
// Test untuk nil
func TestValueIsNil(t *testing.T) {
    value := getValue()

    // Gunakan assert.Nil untuk check value adalah nil
    assert.Nil(t, value, "Value should be nil")
}

// Test untuk non-nil
func TestValueIsNotNil(t *testing.T) {
    value := getNonNullValue()

    // Gunakan assert.NotNil untuk check value tidak nil
    assert.NotNil(t, value, "Value should not be nil")
}
```

## Referensi

- [testify](https://github.com/stretchr/testify)
