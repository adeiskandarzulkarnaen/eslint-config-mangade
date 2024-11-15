# Custom JavaScript - Personal Styling Guide

## Introduction


*Repository* ini berisi konfigurasi ESLint yang merupakan *styling guide* pribadi saya, yang digunakan untuk keperluan pekerjaan. Konfigurasi ini dirancang untuk menjaga konsistensi dan kualitas kode dalam proyek-proyek JavaScript dan TypeScript yang saya kerjakan.

*Style guide* ini mencakup berbagai aturan format dan gaya yang membantu memastikan bahwa kode yang saya tulis tetap rapi, mudah dibaca, dan mengikuti praktik terbaik yang disarankan. Termasuk di dalamnya adalah aturan-aturan umum seperti penggunaan indentasi, format kutipan, preferensi untuk `const` daripada `var`, serta pengaturan untuk menjaga jarak antar elemen kode.

Konfigurasi ini telah disesuaikan agar bekerja dengan baik untuk proyek berbasis JavaScript dan TypeScript, sehingga dapat membantu dalam mengelola berbagai jenis proyek dengan standar yang sama.

## ESLint Sharable Config

 ESlint *[sharable config](https://eslint.org/docs/latest/extend/shareable-configs)* bisa digunakan untuk menerapkan style guide yang didefinisikan sebagai berikut.

### Using Sharable Config in ESLint  9 or Latest

Pasang package ESLint dan `eslint-config-mangade` dengan menggunakan perintah di bawah ini.

```shell
npm install --save-dev eslint eslint-config-mangade
```

Buatlah berkas [konfigurasi ESLint](https://eslint.org/docs/latest/use/configure/#extending-configuration-files) (contoh: `eslint.config.mjs`) dan di dalamnya tulis kode di bawah ini.

```javascript
import adStyle from 'eslint-config-mangade';

export default [
  ...adStyle,
  // other config style
];

```

Anda bisa mendeteksi kesalahan penulisan JavaScript melalui perintah di bawah ini.

```shell
npx eslint
```

Jika ada kode yang tidak sesuai dengan aturan, ESLint akan menampilkan informasinya pada STDOUT.
