# Aplikasi Peminjaman Ruang Kelas
--------------------------------------------------------------------------------------
### Deskripsi Program
> Program Aplikasi Peminjaman Ruang Kelas dibuat dengan tujuan untuk membantu memudahkan pengguna dalam melakukan peminjaman ruang kelas yang tersedia. Selain itu, program ini juga membantu admin untuk mengelola pendaftaran ruang kelas dan melakukan monitoring terhadap peminjaman ruang kelas yang telah dilakukan serta membantu dan memudahkan mahasiswa dalam melakukan peminjaman ruang kelas. Dengan begitu, program ini diharapkan dapat meningkatkan efektivitas dan efisiensi dalam penggunaan ruang kelas yang tersedia.

> Program ini dibuat dengan menggunakan Bahasa pemrograman Python dan mengimplementasikan struktur data Linked List. Aplikasi peminjaman ruang kelas ini juga menggunakan sebuah database, yaitu database MongoDB yang digunakan untuk menyimpan data akun Mahasiswa dan Staff serta data peminjaman ruang kelas.
--------------------------------------

### Struktur Project
> 1. Folder Controller, berisi file-file controller yang akan mengatur alur program serta mengambil data dari model dan menampilkan ke view.                                  > - File Controller Account, sebagai file controller yang berisi logika untuk manajemen akun mahasiswa dan staff, seperti registrasi, login, dan profil user.
       > - File Controller Linked List, sebagai file controller yang berisi logika untuk manajemen data ruang kelas dalam bentuk linked list, dimana data dalam linked list diambil dari database.
        - File Controller User, sebagai file controller yang berisi logika untuk manajemen data mahasiswa dan staff seperti logika menambahkan peminjaman ruang.
> 2. Folder Model, berisi file-file model yang berisi fungsi-fungsi untuk mengakses database dan memproses data.
        - File Database, sebagai file yang berisi class untuk menghubungkan python dan database.
        - File Ruang, sebagai file yang berisi definisi class Ruang yang digunakan untuk merepresentasikan sebuah node pada struktur data Linked List.
> 3. Folder View, berisi file-file view yang berisi tampilan antarmuka aplikasi yang akan dilihat oleh pengguna.
        - File App, sebagai halaman untuk menampilkan informasi dan melakukan peminjaman ruang kelas oleh pengguna yang belum terdaftar sebagai staff atau mahasiswa.
        - File Mahasiswa, sebagai halaman untuk menampilkan informasi dan melakukan peminjaman ruang kelas oleh mahasiswa.
        - File Staff, sebagai halaman untuk menampilkan informasi dan daftar peminjaman ruang kelas oleh staff.
> 4. File main, sebagai file utama yang berfungsi untuk menjalankan program.
--------------------------------------

### Fitur
Pada program ini terdapat library yang digunakan, diantaranya adalah PrettyTable, Datetime, time, PyMongo, os dan random.
>  1. PrettyTable merupakan library atau pustaka dalam python yang digunakan untuk membuat / mengeluarkan data dalam bentuk tabel.
>  2. Datetime adalah sebuah library atau modul yang dipanggil jika anda membutuhkan segala operasi yang berhubungan demi waktu.
>  3. Modul time adalah modul yang menyediakan fungsi-fungsi untuk mengelola waktu dan tanggal. 
>  4. PyMongo berisi alat untuk bekerja dengan MongoDB, dan merupakan cara yang disarankan untuk bekerja dengan MongoDB dari Python.
     Untuk menjalankan PyMongo sendiri, hal yang harus dilakukan adalah mengakses MongoDB ataupun menginstall MongoDB. 
     Selanjutnya user dapat memverifikasi apakah instalasi telah selesai dengan sukses, kita akan terhubung ke server database MongoDB menggunakan alat mongo dan melihat status koneksi melalui MongoDB. 
     Terdapat opsi authorization yang memungkinkan Role-Based Access Control (RBAC) yang mengatur akses pengguna ke sumber daya dan operasi database. 
     Jika opsi ini dinonaktifkan, setiap user akan memiliki akses ke semua database dan melakukan tindakan apa pun.
>  5. Modul os dapat digunakan untuk berinteraksi dengan sistem operasi dan melakukan operasi pada file dan direktori.
>  6. Modul random pada adalah modul yang menyediakan fungsi-fungsi untuk menghasilkan bilangan acak. 

Beberapa fitur yang terdapat pada program ini, yaitu :
- User 
> 1. Pemilihan ruangan : User dapat melihat daftar kelas yang dapat dilakukan peminjaman.
> 2. Membuat peminjaman : User dapat membuat peminjaman kelas yang akan digunakan.
> 3. Mencari ruangan : User dapat mencari kelas untuk mengecek apakah kelas tersebut digunakan atau tidak, apabila digunakan maka akan memunculkan informasi daftar kelas yang digunakan.
> 4. Melihat profil : User dapat melihat profil diri yang berisi NIM, Nama, Program Studi dan Jenis Kelamin.
- Staff
> 1. Membuat dan mengupdate peminjaman : Staff dapat menambahkan daftar kelas dan mengupdate status kelas yang digunakan
> 2. Konfirmasi Peminjaman : Staff dapat melakukan konfirmasi peminjaman yang telah dilakukan oleh mahasiswa. 
> 3. Mencetak bukti peminjaman : Setelah Staff menambahkan daftar kelas yang akan digunakan maka dapat mencetak bukti peminjaman sebagai bukti tanda kelas digunakan sudah terkonfirmasi oleh staff.
> 4. Mencari NIM : Staff juga dapat mencari NIM Mahasiswa yang mengkonfirmasi peminjaman ruang kelas
> 5. Menghapus daftar peminjaman : Staff dapat menghapus daftar kelas yang digunakan
> 6. Melihat profil : Staff dapat  melihat profil yang berisi NIP, Nama, Jenis Kelamin, dan Jabatan
--------------------------------------

### Fungsionalitas
>  1. Registrasi Mahasiswa. Mahasiswa dapat melakukan pendaftaran untuk dapat masuk ke dalam sistem peminjaman ruang kelas dengan mengisi formulir pendaftaran. Mahsiswa harus memberikan informasi pribadi seperti nim, nama, program studi, dan jenis kelamin.
>  2. Login dan Logout (Exit). User dapat melakukan login ke dalam sistem dengan menggunakan nim/nip dan password mereka. User juga dapat keluar dari program dengan melalui pilihan Exit.
>  3. Peminjaman Ruang Kelas. User dapat meminjam ruang kelas dengan mengisi formulir peminjaman. User harus memberikan informasi seperti tanggal dan waktu peminjaman, mata kuliah, dan keperluan peminjaman.
     
--------------------------------------

