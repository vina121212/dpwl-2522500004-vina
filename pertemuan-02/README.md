# pertemuan-02
1. Apa perbedaan front controller, Base Controller, dan Controller aplikasi? Jelaskan peran index.php,
system/core/Controller.php, dan application/controllers/Home.php. Mengapa index.php disebut front
controller?
= 1. Perbedaan Front Controller, Base Controller, dan Controller Aplikasi
Front Controller (index.php): Pintu masuk utama (single point of entry) bagi semua permintaan (request) HTTP. Berperan menginisialisasi environment, memuat konfigurasi utama, dan mengarahkan request ke controller yang tepat (routing).

Base Controller (system/core/Controller.php): Kelas induk (parent class) inti yang disediakan oleh framework. Menyiapkan super-object CodeIgniter, menginisialisasi pustaka bawaan, serta menyediakan fondasi agar pustaka (library), model, dan tampilan (view) dapat dipanggil di seluruh aplikasi.

Controller Aplikasi (application/controllers/Home.php): Kelas turunan (child class) yang dibuat oleh pengembang aplikasi. Berisi logika bisnis spesifik untuk fitur atau halaman tertentu (misalnya halaman utama/Home).

Mengapa index.php Disebut Front Controller?
index.php disebut Front Controller karena menerapkan pola desain Front Controller Pattern.

Berdasarkan pola ini, aplikasi tidak membiarkan pengguna mengakses file script individual secara langsung (seperti about.php atau contact.php). Sebaliknya, semua lalu lintas HTTP dialirkan melalui satu file gerbang depan (index.php).

2. Apa perbedaan tanggung jawab routes.php dan Router.php?
=Dalam arsitektur web framework seperti CodeIgniter, routes.php bertindak sebagai file konfigurasi (deklarasi aturan), sedangkan Router.php bertindak sebagai mesin pemroses (eksekutor logika routing).

3. Jelaskan bagaimana URL index.php/info/routing berubah menjadi pemanggilan Home::info("routing").
=Proses transformasi dari request URL index.php/info/routing hingga mengeksekusi metode Home::info("routing") melibatkan kerja sama beberapa komponen inti CodeIgniter (URI, Router, dan Bootstrap Engine).

4. Mengapa URL sebaiknya dibentuk menggunakan base_url()/site_url() daripada ditulis hard-coded
berulang?
=Menggunakan helper base_url() atau site_url() alih-alih menuliskan URL secara hard-coded (misal: http://localhost/myproject/about) adalah praktik terbaik (best practice) dalam pengembangan web.

5. Mengapa folder models belum dibuat pada P2?
=folder models biasanya belum digunakan atau belum dibuat karena
Fokus pada Fondasi Alur Dasar MVC (Routing, Controller, & View):
Pada P2, materi berfokus pada pemahaman bagaimana request diterima oleh index.php, diproses oleh Controller, lalu menampilkan hasilnya ke View. Pengenalan alur dasar ini sengaja dibuat tanpa melibatkan database agar mahasiswa/pembelajar tidak bingung dengan kompleksitas olah data terlebih dahulu.

6. Apa perbedaan fungsi workspace dpwl-nim dan repositori dpwl-nim-nama?
=kita bisa mengerjakan kode program dan melakukan pengujian di Workspace lokal (dpwl-nim).
Setelah selesai, Anda melakukan commit dan menolak (push) perubahan tersebut ke Repositori remote (dpwl-nim-nama) agar tersimpan secara aman dan siap dinilai/direview.

7. Sebutkan komponen P2 yang mempunyai konsep serupa ketika nanti menggunakan CI3.
=Konsep utama yang dipelajari pada Praktikum 2 (P2) dalam mata kuliah Desain & Pemrograman Web Lanjut (DPWL)—seperti struktur arsitektur Web/PHP modular, pengelolaan routing, hingga pemisahan tampilan (view) dan logika—memiliki padanan langsung dalam CodeIgniter 3 (CI3) yang menerapkan pola MVC (Model-View-Controller).