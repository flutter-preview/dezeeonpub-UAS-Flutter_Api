# UAS-Flutter_Api


Nama : Muhammad AzizuL Dzikri 
Nim : 312110178

/***
SOURCE CODE NYA PADA MAIN DART

Program di atas adalah sebuah contoh penggunaan API dalam aplikasi Flutter menggunakan bahasa pemrograman Dart. Tujuan program ini adalah untuk menampilkan daftar stasiun kereta api dengan mengambil data dari API yang disediakan oleh KAI (Kereta Api Indonesia).

Berikut adalah penjelasan rinci tentang program ini:

1. Pada baris 1-2, dilakukan import beberapa package yang diperlukan, yaitu 'dart:convert' untuk mengkonversi data JSON, 'package:flutter/material.dart' untuk menggunakan widget dari Flutter, dan 'package:http/http.dart' sebagai package HTTP client untuk melakukan HTTP request ke API.

2. Pada baris 4-7, fungsi `main()` dijalankan ketika aplikasi dijalankan. Fungsi ini menjalankan aplikasi Flutter dengan memanggil `runApp()` dengan menggunakan `MyApp()` sebagai root widget.

3. `MyApp` merupakan stateless widget yang menjadi root widget dari aplikasi. Pada `build()` method, `MaterialApp` digunakan untuk menentukan judul aplikasi dan tema yang digunakan. `MyHomePage()` dijadikan sebagai halaman utama.

4. `MyHomePage` merupakan stateful widget yang digunakan sebagai halaman utama. Pada `build()` method, `Scaffold` digunakan sebagai struktur dasar dari halaman dengan judul yang ditentukan di app bar dan menggunakan `ListView.builder` untuk menampilkan daftar stasiun kereta api.

5. Pada `MyHomePage` juga terdapat method `fetchData()` yang digunakan untuk mengambil data stasiun dari API menggunakan HTTP request. Pada method ini, URL endpoint API diinisialisasi menggunakan `Uri.parse()`, kemudian dilakukan HTTP GET request menggunakan `http.get()`. Jika response berhasil (kode status 200), data JSON yang diterima di-decode menggunakan `jsonDecode()` dan disimpan di dalam list `stations` menggunakan `setState()` untuk memperbarui tampilan.

6. Pada method `initState()`, `fetchData()` dipanggil saat widget diinisialisasi untuk mengambil data stasiun dari API.

7. Pada `ListView.builder`, `itemCount` diatur dengan panjang list `stations`, dan untuk setiap item dalam list, widget `ListTile` digunakan untuk menampilkan informasi stasiun. Data seperti kode stasiun, nama kereta, kota, dan nama kota ditampilkan menggunakan `Text()` widget.

Dengan demikian, program ini akan menampilkan daftar stasiun kereta api yang diambil dari API KAI pada aplikasi Flutter.

HASIL OUTPUT
/**
 ![Gambar 2](https://github.com/dezeeonpub/UAS-Flutter_Api/blob/master/web.PNG)
 ![Gambar 2](https://github.com/dezeeonpub/UAS-Flutter_Api/blob/master/Tampilan-mobile.PNG)
