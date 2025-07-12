---
layout: post
title: "Laravel"
---

<h1>Laravel</h1>

Laravel adalah framework PHP modern dan powerful yang digunakan untuk membangun aplikasi web berskala kecil hingga besar. Di bawah ini adalah panduan instalasi Laravel secara lengkap, mulai dari nol hingga siap dijalankan secara lokal, beserta penjelasan kegunaan setiap langkah.

<h2>Prasyarat Sistem</h2>
Sebelum memulai, pastikan perangkatmu sudah memiliki:

<ul>
    <li>PHP versi 8.1 atau lebih baru</li>
    <li>Composer (manajer dependensi PHP)</li>
    <li>Web server (seperti Apache atau Nginx, atau gunakan server bawaan Laravel)</li>
    <li>Database (MySQL, PostgreSQL, SQLite, dsb)</li>
</ul>

<h2>1️. Install Composer</h2>
Perintah:

<pre>
Kunjungi dan ikuti petunjuk instalasi Composer:  
<a href="https://getcomposer.org/download/">https://getcomposer.org/download/</a>
</pre>

<h3>Kegunaan:</h3>
Composer adalah alat untuk mengelola dependensi/library PHP. Laravel membutuhkan Composer untuk mengunduh semua komponen framework dan dependensi proyeknya.

<h2>2️. Install Laravel Installer Secara Global</h2>
Perintah:

<pre>
composer global require laravel/installer
</pre>

<h3>Kegunaan:</h3>
Perintah ini menginstal Laravel Installer secara global di sistemmu. Dengan ini, kamu bisa membuat proyek Laravel baru dengan cepat menggunakan perintah `laravel new nama-proyek` dari terminal, tanpa harus mendownload manual.

<h2>3️. Tambahkan Laravel ke PATH (Jika Perintah Belum Terdeteksi)</h2>

<h3>Linux/macOS:</h3>
<pre>
export PATH="$HOME/.composer/vendor/bin:$PATH"
</pre>

<h3>Windows:</h3>
Tambahkan path berikut ke Environment Variables:

<pre>
C:\Users\NamaUser\AppData\Roaming\Composer\vendor\bin
</pre>

<h3>Kegunaan:</h3>
Menambahkan Laravel Installer ke PATH sistem memungkinkan kamu menjalankan perintah `laravel` dari terminal di direktori mana pun. Tanpa ini, terminal tidak akan mengenali perintah `laravel`.

<h2>4️. Buat Project Laravel Baru</h2>
Perintah (menggunakan installer):

<pre>
laravel new nama-proyek
</pre>

Atau alternatif:

<pre>
composer create-project laravel/laravel nama-proyek
</pre>

<h3>Kegunaan:</h3>
Langkah ini membuat direktori baru berisi struktur standar Laravel, termasuk folder `app`, `routes`, `config`, dan file konfigurasi penting. Laravel siap dikembangkan di folder ini.

<h2>5️. Masuk ke Direktori Project</h2>
Perintah:

<pre>
cd nama-proyek
</pre>

<h3>Kegunaan:</h3>
Perintah ini membawa kamu ke dalam folder proyek Laravel, agar kamu bisa menjalankan perintah seperti `php artisan`, membuka file kode, dan mengelola proyekmu langsung dari terminal.

<h2>6️. Jalankan Server Lokal Laravel</h2>
Perintah:

<pre>
php artisan serve
</pre>

<h3>Kegunaan:</h3>
Perintah ini menjalankan server development bawaan Laravel di <a href="http://localhost:8000" target="_blank">http://localhost:8000</a>. Sangat cocok untuk keperluan pengembangan dan testing tanpa perlu konfigurasi server Apache/Nginx.

<h2>7️. Atur File Konfigurasi Lingkungan (.env)</h2>
File yang diedit: `.env`

Contoh isi file:

<pre>
APP_NAME=Laravel  
APP_ENV=local  
APP_KEY=base64:...  
APP_DEBUG=true  
APP_URL=http://localhost  

DB_CONNECTION=mysql  
DB_HOST=127.0.0.1  
DB_PORT=3306  
DB_DATABASE=laravel_db  
DB_USERNAME=root  
DB_PASSWORD=
</pre>

<h3>Kegunaan:</h3>
File `.env` menyimpan konfigurasi penting proyek seperti koneksi database, mode debug, nama aplikasi, dan kunci enkripsi. Setiap environment (development, staging, production) dapat memiliki `.env` yang berbeda tanpa mengubah file kode utama.

<h2>Selamat laravel berhasil diinstal dan dijalankan!</h2>
Setelah semua langkah di atas selesai, kamu bisa mulai membuat route, controller, model, dan fitur aplikasi web dengan Laravel.

![html link dan lists](/assets/images/L.png)