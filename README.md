# Tutorial Penggunaan Git

* Git adalah salah satu sitem pengontrol versi (Version Control System) pada proyek perangkat lunak yang diciptakan oleh Linus TOrvaids.

## Instalasi Git

* Download Git, buka website resminya Git (git-scm.com).
* Kemudian unduh Git sesuai arsitektur komputer kita (32bit atau 64bit).
* Setelah terinstal di Windows, untuk mencobanya silakan buka CMD atau PowerShell, kemudian ketik perintah `git --version`

![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/cmd.PNG)

## Menambahkan Global Config

* Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi *user.name* dan *user.email*
* Konfigurasi ini bisa dilakukan untuk global repository atau individual repository.
* Apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah **git commit**

* Config Global Repository

`$ git config --global user.name "nama_user"`
`$ git config --global user.email "nama_user"`

## Perintah Dasar Git

* **git init**, perintah untuk membuat repository local.
* **git add**, perintah untuk menambah file baru, atau perubahan pada file pada staging sebelum commit.
* **git commit**, perintah untuk menyimpan perubahan kedalam database git.
* **git push -u origin master**, perintah untuk mengirim perubahan pada repository local menuju server repository.
* **git clone [url]**, perintah untuk membuat working directory yang diambil dari repository server.
* **git remote add origin [url]**, perintah untuk menambahkan remote server/repository server pada local repository (working directory).

## Membuat Repository Local

* Buka direktory aktif, misal: `E:\Data Kuliah\Semester 2\Bahasa Pemrograman 1\labspy` (buka menggunakan Windows Explorer)
* Klik kanan pada pada direktory aktif tersebut, dan pilih menu Git Bash sehingga muncul git bash command
* Buat direktory project praktikum dengan nama **Latihan1**

`$ mkdir latihan1`
`$ cd latihan1`

* Sehingga terbentuk satu direktory baru dibawahnya, selanjutnya masuk kedalam direktory tersebut dengan perintah **cd** (change directory)
* Directory aktif menjadi: `E:\Data Kuliah\Semester 2\Bahasa Pemrograman 1\labspy\latihan1`

![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/mkdir.PNG)

* Jalankan perintah `git init`, untuk membuat repository local
* Repository baru berhasil dibuat, dengan terbentuknya folder baru di direktory hidden dengan nama **.git**
* Pada direktory tersebut, semua perubahan pada *working directory* akan disimpan.

![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/gitinit.PNG)

## Menambah File baru pada Repository

* Untuk membaut file dapat menggunakan text editor, lalu disimpan pada direktory(repository)
* Disini kita akan membuat file **README.md**(text file)
* Ketika perintah:
`echo "#latihan1" >> README.md`
* File **README.md** berhasil dibuat.

![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/readme.PNG)

* Tambahkanambahkan file README.md kedalam berkas repo dengan perintah **git add**.
`git add readme.md`
* Cek status repository, masukan perintah
`git status`
 
![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/gitadd.PNG)

## Commit (Menyimpan perubahan ke database)

 * Untuk menyimpan perubahan ke database repository lokal, gunakan perintah:
  `git commit -m "komentar commit"`
  
![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/gitcommit.PNG) 
  
## Membuat Repository Server pada Web Github

* Server Repository yang akan digunakan adalah http://github.com
* Anda harus mempunyai akun terlebih dahulu, kemudian pada laman **github**, silahkan login menggunakan akun tersebut.
* Pada laman github pojok kanan atas, klik **icon +** kemudian klik **New repository**

![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/new.PNG)

* Isikan nama repository, lalu klik tombol **Create repository**

![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/create.PNG)


## Menambahkan Remote Repository

* Untuk menambah remote repository server tadi, masukan perintah : 
`git remote add origin [url]`

![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/remoteadd.PNG)

## Push (mengirim perubahan keserver)

* Untuk mengirim perubahan pada local repository ke server, masukan perintah:
`git push -u origin master`
* Perintah ini akan meminta memasukan username dan passowrd akun github.
* Silahkan masukan username dan password akun **github** untuk login

![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/login.PNG)
![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/push.PNG)

## Melihat hasil repository pada server 

* Buka halaman github.com, hasilnya dapat dilihat di repository **github** yang telah kita buat tadi.
![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/hasil.PNG)

## Clone repository

* Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repository.
* Untuk mengcloning sebuah repository, silahkan masukan perintah
`git clone [url]
![GitHub Logo](https://github.com/Jajang1293/Latihan1/blob/master/clone.PNG)

# Selesai



