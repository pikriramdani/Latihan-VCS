# Latihan-VCS
Repository ini dibuat untuk memenuhi tugas Pertemuan 4-Bahasa Pemrograman

Nama    : Pikri Ramdani

NIM     : 312010162

KELAS   : TI.20.A.1

## Langkah-Langkah Penggunaan Git

* Langkah pertama Download Git,buka website resminya git [click here](https://git-scm.com)

![download git-scm](coding-git/git-scm.PNG) 

* kemudian unduh git sesuai dengan arsitektur komputer kita. kalau menggunakan 64bit, unduh yang 64bit. begitu juga kalo menggunakan 32bit.

![download git-bit](coding-git/git-bit.PNG)

* selamat, Git sudah terinstal di windows. untuk mencobanya, silahkan buka CMD atau PowerShell, kemudian ketik perintah git-version.

![download git-version](coding-git/git-version.PNG)

 ## Menambahkan Global Config

 * pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email

 * konfigurasi ini bisa dilakukan untuk global repository atau individual repository

 * apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit

 * config global repository $ git config --global user.name "masukan nama anda"

![download git-username](coding-git/git-username.PNG)

 * $ git config --global user.email "masukan email anda"

 ![download git-user.email](coding-git/git-useremail.PNG)

 ## Perintah Dasar Git

 * Git init, perintah untuk membuat repository local

 * Git add, perintah untuk menambahkan file baru, atau perubahan file pada staging sebelum proses commit

 * Git commit, perintah untuk menyimpan perubahan kedalam database git

 * Git push -u original master, perintah untuk mengirim perubahan pada repository local menuju server revository 

 * Git clone [url], perintah untuk membuat working directory yang diambil dari repository server

 * Git remote add origin [url], perintah untuk menambahkan remote server/repository server pada local repository (working directory) 

 * Git pull, perintah untuk mengambil/mendownload perubahan terbaru dari server repository ke local repository

 ## Membuat Repository Local 

 * Buka directory aktif, misal: d:/labs_pemrograman1 (buka menggunakan Windows Explorer)

 * klik kanan pada directory aktif tersebut, dan pilih menu Git Bash, sehinga muncul Git Bash, sehingga muncul Git Bash commad

 * Buat directory project praktikum pertama dengan nama latihanVCS

 * Sehingga terbentuk satu directory baru dibawahnya, selanjutnya masuk kedalam directory tersebut dengan perintah cd (change directory)

* Directory aktif menjadi: d:/labs_pemrograman1/latihanVCS $ mkdir latihanVCS $ cd latihanVCS

## Membuat Repository Local

* Jalankan perintah git init, untuk membuat repository local.

* Repository baru berhasil di inisialisasi, dengan terbentuknya satu directory hidden dengan nama.git

* Pada directory tersebut, semua perubahan pada working directory akan disimpan. $ git init

## Menambahkan File Baru Pada Repository 

* Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktor aktif (repository) 

* Disini kita akan coba buat satu file bernama README.md(text file)

* File README.md berhasil dibuat. $ echo "#latihanVCS">>README.md

![download git-latihanvcs](coding-git/git-latihanvcs.PNG)

* Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.

* File README.md berhasil ditambahkan. $ git add README.md

## Commit (Menyimpan Perubahan Ke Database)

* Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m "Komentar Commit"

* Perubahan berhasil disimpan. $ git commit -m "update README.md"

![download git-commit](coding-git/git-commit.PNG)

## Membuat Repository Server

* Server repository yang akan kita gunakan adalah [click here](http://github.com)

* Anda harus membuat akun terlebih dahulu 

Pada laman github, klik tombol star a project, atau dari menu (icon+) klik New Repository

![download github-createnew](coding-git/github-createnew.PNG)

## Membuat Repository Server

* Isi nama repositorynya, misal:Latihan-VCS

* Lalu klik tombol create repository

![download github-newrepo](coding-git/github-newrepo.PNG)

## Menambahkan Remote Repositorynya

* Remote Repositorynya merupakan server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

* Untuk menambahkan remote repository server, gunakan perintah git remote add original [url] $ git remote add origin
[click here](https://github.com/pikriramdani/Latihan-VCS)

## Push (Mengirim Perubahan Ke Server)

* Untuk mengirim perubahan pada local repository ke server gunakan perintah git push

* perintah ini akan meminta memasukan username dan password pada akun github.com $ git push -u origin master

![download github-push](coding-git/github-push.PNG)

![download git-push](coding-git/git-push.PNG)

## Melihat Hasilnya Pada Server Repository

* Buka laman github.com, arahkan pada repositorynya

* Maka perubahan akan terlihat pada laman tersebut

![download github-view1](coding-git/github-view1.PNG)

## Clone Repository

* Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu directory sesuai dengan nama repositorynya (working directory)

* untuk melakukan cloning, gunakan perintah git clone [url]

![download git-clone](coding-git/git-clone.PNG)

## Kegunaan file README.md

* Apabila kita menggunakan github, untuk memberikan penjelasan awal pada project yang kita buat, maka dapat menggunakan sebuah file yang bernama README.md

* pada file tersebut kita dapat membuat dokumentasi dari setiap project yang kita buat untuk memberikan penjelasan atau sekedar cara penggunaan dari aplikasi yang kita kembangkan

* Penulisan file README.md berbasis teks, dan untuk pemformatannya menggunakan Markdown format

* Untuk lebih jelasnya, dapat anda pelajari cara penggunaan markdown pada [url] berikut:

[click here](https://markdownguide.org/basic-syntax)