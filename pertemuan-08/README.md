# pertemuan-08

## Menu Navigasi
Telah dilakukan penambahan menu Manajemen Penyewaan pada bilah navigasi sidebar aplikasi dengan rincian pengerjaan sebagai berikut:

1. Navigasi SideBar:
   Menambahkan elemen navigasi baru yang mengarah ke URL modul penyewaan menggunakan fungsi helper
   
2. Keamanan Link :
   Penerapan fungsi pada atribut untuk memastikan URL dirender dengan aman dan mencegah potensi celah keamanan 

3. Pengembangan Antarmuka:
   Penggunaan ikon untuk memberikan identitas visual bagi pengguna dalam mengelola data master penyewaan kendaraan.

### 2. Antarmuka Formulir dan Tampilan Data
1. Membangun halaman Manajemen Penyewa yang konsisten dengan tata letak fitur Manajemen Kendaraan
2. Menyediakan tabel untuk menampilkan seluruh daftar penyewa beserta formulir input/edit data penyewa

### 3. Implementasi Arsitektur MVC & CRUD
1. Menerapkan arsitektur (MVC) secara terpisah untuk pemrosesan data penyewa
2. Memastikan kata sandi (password) disimpan secara aman menggunakan enkripsi hash

### 4. Validasi, Keamanan, dan Pengelolaan Berkas Foto
1. Menerapkan validasi input data dan sanitasi untuk mencegah celah keamanan
2. Menerapkan pola Post-Redirect-Get (PRG) untuk menghindari pengiriman ulang form saat refresh halaman
3. Mengimplementasikan fitur unggah foto KTP dan SIM A dengan pemeriksaan ekstensi/ukuran berkas serta penanganan error saat pengunggahan

### 5. Pengujian Sistem
1. Memastikan seluruh fungsi CRUD (Create, Read, Update, Delete) data penyewa berjalan tanpa hambatan
2. Memastikan validasi password dan pengunggahan berkas berjalan sesuai aturan
3. Memastikan seluruh fitur bawaan aplikasi yang sudah ada sebelumnya tidak mengalami break/error

### 6. Dokumentasi & Repositori
1. Menyusun dokumentasi pengerjaan pada berkas `pertemuan-08\README.md`
2. Mengunggah hasil ekspor basis data terbaru dalam format `.sql` ke repositori
3. Melakukan versi kontrol Git secara berkala menggunakan perintah `git add`, `git commit -m "..."`, dan `git push`