---
layout: post
title: "CRUD"
---

<h1>CRUD</h1>

Apa itu CRUD? CRUD adalah crate, read, update, dan delate. setelah kita menghubungkan database kita ke laravel maka sekarang kita ada melakukan CRUP di database di pertemuan yang lalu di database siswa.

<h3>Langkah pertama</h3>
Buat model dan migration untuk siswa, gunanya untuk mendefinisikan kolom/atribut siswa (misal: nis, nama, kelas, alamat, agama, jenis kelamin) yang akan di simpan ke database.

<h3>Langkah kedua</h3>
Setelah membuat migration, langkah selanjutnya adalah menjalankan migrasi agar tabel siswa benar-benar dibuat di dalam database, gunanya menyiapkan tempat menyimpan data siswa.

<h3>Langkah ketiga</h3>
Selanjutnya buat sebuah controller khusus yang bertugas menangani semua permintaan terkait data siswa, seperti menampilkan daftar siswa, menambahkan data, menyimpan data, mengedit, dan menghapus. gunanya sebagai jembatan antara data dan tampilan (view), serta pengatur logika CRUD.

<h3>Langkah keempat</h3>
Agar halaman-halaman siswa bisa diakses lewat URL, kamu harus menambahkan routing. gunanya mengatur URL apa saja yang tersedia (misalnya /siswa, /siswa/tambah, dll), dan menghubungkannya ke fungsi di controller.

<h3>Langkah kelima</h3>
Buat tampilan untuk:
<ul>
<li>Menampilkan daftar siswa dalam bentuk tabel</li>
<li>Formulir untuk menambah siswa baru</li>
<li>Formulir untuk mengedit data siswa</li>
<li>Konfirmasi penghapusan</li>
</ul>
Gunanya agar pengguna dapat berinteraksi secara visual dengan data siswa.

<h3>Langkah keenam</h3>
Tambahkan link di bagian sidebar atau menu utama dashboard agar pengguna bisa langsung menuju halaman manajemen siswa. gunanya memberikan akses cepat dan terstruktur ke fitur siswa dari antarmuka utama aplikasi.

<h3>Langkah ketujuh</h3>
Selanjutnya isi logika di dalam controller seperti menyimpan data baru, memperbarui data yang sudah ada, menghapus, dan menampilkan data. Gunanya agar semua aksi CRUD bisa berjalan dengan benar sesuai permintaan pengguna.

<h3>Langkah kedelapan</h3>
Jika fitur siswa hanya boleh diakses oleh admin atau pengguna yang login, tambahkan perlindungan menggunakan middleware. Gunanya menjaga keamanan agar fitur tidak bisa diakses sembarang orang.

<h3>Contoh hasil setelah melakukan semua langkah langkah</h3>
Setelah langkah telah dikerjakan maka hasil yang akan di dapatkan ialah:
<ul>
<li>Menu sidebar bernama Siswa</li>
<li>Halaman daftar siswa</li>
<li>Formulir tambah siswa</li>
<li>Formulir edit siswa</li>
<li>Tombol hapus siswa</li>
<li>Semua data tersimpan di database dan bisa dimodifikasi sesuai kebutuhan</li>
</ul>
CRUD ini sangat penting dalam aplikasi atau database.

<h3>Contoh hasil</h3>
Disini kalian sudah bisa tambah data, edit maupun hapus data.

![html link dan lists](/assets/images/awal.png)