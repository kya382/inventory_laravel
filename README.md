# Sistem Informasi Inventori Barang

## 1. Deskripsi Proyek

Sistem Informasi Inventori Barang adalah aplikasi berbasis web yang dibuat menggunakan Laravel untuk membantu mengelola data barang dan stok. Aplikasi ini memudahkan pengguna dalam menambahkan, melihat, mengubah, dan menghapus data barang serta kategori barang.

## 2. Fitur Aplikasi

- Login dan logout pengguna.
- Dashboard yang menampilkan ringkasan data inventori.
- Mengelola kategori barang.
- Menambah, melihat, mengubah, dan menghapus data barang.
- Mencari barang berdasarkan nama atau SKU.
- Memfilter barang berdasarkan kategori.
- Mengurutkan data barang berdasarkan nama atau harga.
- Menampilkan data barang dengan pagination.
- Menampilkan status stok aman dan stok menipis.

## 3. Teknologi yang Digunakan

- **Bahasa pemrograman:** PHP
- **Framework:** Laravel
- **Database:** MySQL
- **Pengelolaan database:** MySQL melalui XAMPP
- **Tampilan:** Blade, HTML, dan CSS

## 4. Persyaratan

Sebelum menjalankan aplikasi, pastikan perangkat sudah memiliki:

- PHP
- Composer
- MySQL
- XAMPP
- Browser

## 5. Cara Menjalankan Aplikasi

1. Salin atau ekstrak folder proyek ke komputer.
2. Buka terminal di dalam folder proyek.
3. Jalankan perintah berikut untuk memasang paket Laravel:

   ```bash
   composer install
   ```

4. Salin file `.env.example` menjadi `.env`.
5. Sesuaikan pengaturan database pada file `.env`:

   ```env
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=inventory_web5
   DB_USERNAME=root
   DB_PASSWORD=
   ```

6. Buat database bernama `inventory_web5` melalui phpMyAdmin.
7. Buat kunci aplikasi dengan perintah:

   ```bash
   php artisan key:generate
   ```

8. Jalankan migrasi database:

   ```bash
   php artisan migrate
   ```

9. Jalankan aplikasi:

   ```bash
   php artisan serve --port=8001
   ```

10. Buka browser dan akses:

    `http://127.0.0.1:8001`

## 6. Informasi Login

Akun login untuk pengujian lokal:

- **Username:** admin
- **Password:** admin123

Gunakan akun tersebut jika masih sesuai dengan data akun yang tersimpan di database proyek.

## 7. Struktur Folder

- `app/` — menyimpan model dan pengaturan aplikasi.
- `database/` — menyimpan migration, factory, dan seeder.
- `public/` — menyimpan file yang dapat diakses melalui web.
- `resources/views/` — menyimpan tampilan aplikasi.
- `routes/web.php` — menyimpan pengaturan alamat halaman.
- `config/` — menyimpan konfigurasi aplikasi.
- `composer.json` — menyimpan informasi paket PHP yang digunakan.
- `.env.example` — contoh pengaturan lingkungan aplikasi.

## 8. Catatan

File `.env` tidak disertakan dalam repositori karena berisi pengaturan lokal dan informasi sensitif. Folder `vendor` dapat dibuat kembali dengan menjalankan `composer install`.

Aplikasi ini dibuat untuk memenuhi tugas praktikum Web 5 dengan menggunakan framework Laravel.
