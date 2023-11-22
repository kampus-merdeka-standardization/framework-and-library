## Definition

Unit testing adalah proses pengujian pada tingkat komponen atau unit individu dalam backend. Unit yang dimaksud bisa berupa kode, fungsi, metode, prosedur, modul, atau objek tersendiri. Tujuan dari pengujian ini adalah untuk memvalidasi bahwa setiap unit kode software sudah bisa bekerja sesuai harapan.

## Jest

Jest adalah sebuah framework pengujian yang dikembangkan oleh Facebook. Framework ini khusus dikembangkan untuk melakukan unit testing pada javascript. Pada backend, khususnya Node.js, Jest juga dapat digunakan untuk melakukan unit testing.

## Mocha

Mocha adalah sebuah framework pengujian JavaScript yang kaya fitur dan berjalan di Node.js dan di browser. Mocha mengenkapsulasi tes dalam suite tes (blok `describe`) dan kasus tes (blok `it`).

## Scoring sheet
| Kriteria      | Jest    | Mocha |
|---------------|---------|---------|
| Maintenance   | 3       | 1       |
| Reputable     | 4       | 4       |
| Compatibility | 4       | 4       |
| Community     | 4       | 4       |
| Documentation | 4       | 4       |
| Licensing     | 4       | 4       |
| Extensible    | 4       | 3       |
| Size          | 4       | 4       |
| **Total Score**   | **31**    | **29**    |

## Conclusion

Berdasarkan skor tinggi yang diperoleh oleh Jest dan beragam fitur yang ditawarkannya, kami menyimpulkan bahwa Jest adalah pilihan utama untuk pengembangan proyek backend menggunakan NestJS. Kombinasi antara keandalan, kompatibilitas, dan komunitas yang kuat membuat Jest menjadi alat yang sangat efektif untuk unit testing dalam lingkungan Node.js, khususnya dengan NestJS.


## How to Install


1. **Instalasi Jest**:

   Menggunakan npm:

   ```sh
   npm install --save-dev jest
   ```

   Atau menggunakan Yarn:

   ```sh
   yarn add --dev jest
   ```

2. **Instalasi tipe Jest untuk TypeScript**:

   ```sh
   npm install --save-dev @types/jest
   ```

3. **Instalasi ts-jest**:

   `ts-jest` adalah preprocessor TypeScript untuk Jest yang akan menangani kompilasi file TypeScript dalam tes Jest Anda.

   ```sh
   npm install --save-dev ts-jest
   ```

4. **Buat atau perbarui konfigurasi Jest Anda**:
   Ini bisa dilakukan dalam `package.json` atau dalam file terpisah `jest.config.js`. Berikut contoh tampilan `jest.config.js` Anda:
   ```javascript
   module.exports = {
     preset: 'ts-jest',
     testEnvironment: 'node',
   };
   ```

5. **Tambahkan skrip tes ke `package.json` Anda**:
   ```json
   "scripts": {
     "test": "jest"
   }
   ```

## How to Use

### Import Modul yang Diperlukan

Pertama-tama, import modul yang akan Anda uji dan modul `expect` dari Jest.

```typescript
import { functionToTest } from './moduleToTest';

// Kode pengujian di sini
```

### Contoh Pengujian

Berikut adalah beberapa contoh pengujian dasar menggunakan Jest dengan TypeScript:

#### Mengujikan nilai true dan false

```typescript
test('true to be true', () => {
  expect(true).toBe(true);
});

test('false to be false', () => {
  expect(false).toBe(false);
});
```

#### Mengujikan kesamaan dan perbedaan

```typescript
test('object assignment', () => {
  const data = { one: 1 };
  data['two'] = 2;
  expect(data).toEqual({ one: 1, two: 2 });
});

test('adding positive numbers is not zero', () => {
  for (let a = 1; a < 10; a++) {
    for (let b = 1; b < 10; b++) {
      expect(a + b).not.toBe(0);
    }
  }
});
```

#### Mengujikan error dan tidak error

```typescript
test('throwing an error', () => {
  expect(() => {
    throw new Error('An error occurred');
  }).toThrow('An error occurred');
});

test('not throwing an error', () => {
  expect(() => {
    // No error thrown here
  }).not.toThrow();
});
```

#### Mengujikan null dan keberadaan nilai

```typescript
test('null', () => {
  const n = null;
  expect(n).toBeNull();
  expect(n).toBeDefined();
  expect(n).not.toBeUndefined();
  expect(n).not.toBeTruthy();
  expect(n).toBeFalsy();
});

test('zero', () => {
  const z = 0;
  expect(z).not.toBeNull();
  expect(z).toBeDefined();
  expect(z).not.toBeUndefined();
  expect(z).not.toBeTruthy();
  expect(z).toBeFalsy();
});
```


Setelah Anda mengatur konfigurasi dan menulis kode pengujian, Anda dapat menjalankan pengujian dengan perintah berikut:

```bash
npm run jest
```

Atau jika Anda ingin menjalankannya secara langsung:

```bash
npx jest
```
Jest kemudian akan menjalankan semua file pengujian yang berakhiran dengan `.test.ts` atau `.spec.ts`.

## Referensi

- [jest - npm](https://www.npmjs.com/package/jest)
- [mocha - npm](https://www.npmjs.com/package/mocha)
- [Unit Testing adalah?](https://glints.com/id/lowongan/unit-testing-adalah/)