# Latihan 1
**CARA PENGGUNAAN GIT**

**1. Download Aplikasi GIT**

Untuk menginstall Git, Anda perlu mengunduh filenya terlebih dahulu di situs resminya https://git-scm.com/, Kemudian pilih git sesuai perangkat yang anda gunakan. Download sesuai tipe sistem operasi pada komputer Anda. Apabila tipe sistem operasi komputer Anda 64bit,  pilih Git yang mendukung Windows 64bit. Tujuannya adalah agar tidak terjadi error saat proses instalasi Git.
![1](https://user-images.githubusercontent.com/73032342/96348623-66476c00-10d4-11eb-9659-abf94099aaec.PNG)

**2. Instalasi GIT**

- Install GIT pada perangkat komputer anda.

- Jika sudah berhasil terinstal, untuk mencobanya, silahkan buka CMD atau PowerShell, kemudian ketik perintah 

`git --version`

![2](https://user-images.githubusercontent.com/73032342/96348844-e9b58d00-10d5-11eb-8f74-084799bc63fb.PNG)

**3. Melakukan Konfigurasi Awal**

- Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email.

- Apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah _git commit_

Silahkan lakukan konfigurasi dengan perintah berikut ini: `$ git config --global user.name "username anda"` `$ git config --global user.email "email anda"`

![3](https://user-images.githubusercontent.com/73032342/96349027-18803300-10d7-11eb-9e8c-df793c869267.PNG)

**4. Membuat Repository Local**

- Buat folder aktif, misalnya Labs_pemrograman1, kemudian klik kanan pada folder tersebut, lalu klik _Git Bash Here_

![4](https://user-images.githubusercontent.com/73032342/96349072-5e3cfb80-10d7-11eb-89b2-7ca024d62528.PNG)

- Kemudian buat folder projek praktikum dengan nama Latihan1 dengan cara memasukan perintah berikut:

`$ mkdir Latihan1` `$cd Latihan1`
 
![4 1](https://user-images.githubusercontent.com/73032342/96349180-fdfa8980-10d7-11eb-8937-ccd0d80629b2.PNG)

- Jalankan perintah _git init_ untuk membuat repository lokal

`$git ini`

![4 2](https://user-images.githubusercontent.com/73032342/96349203-2edabe80-10d8-11eb-82ca-c4f3ceb8e55e.PNG)

**5. Menambahkan File Baru Pada Repository**

- Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository). Disini kita akan coba buat satu file bernama README.md (text file) dengan menggunakan perintah :

`$ echo "#Latihan 1" >> README.md`

![5 1](https://user-images.githubusercontent.com/73032342/96349238-86792a00-10d8-11eb-9a37-c78732737596.PNG)

- Untuk menambah file yang baru saja dibuat tersebut gunakan perintah git add

`$ git add README.md`

![5 2](https://user-images.githubusercontent.com/73032342/96349250-9729a000-10d8-11eb-8edb-1c31f2c0bffa.PNG)

**6. _Commit_ (Menyimpan Perubahan Ke Database)**

Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah berikut: 

`$ git commit --m "komentar commit"`

![6 1](https://user-images.githubusercontent.com/73032342/96349337-2c2c9900-10d9-11eb-8981-ef932511db9e.PNG)

**7. Membuat Repository Server**

- Server reopsitory yang digunakan adalah http://github.com

- Buatlah akun github, kemudian klik new repository dari menu icon (+)

![5](https://user-images.githubusercontent.com/73032342/96349378-71e96180-10d9-11eb-8f44-8367a92134d8.PNG)

- Isi nama repositorynya, misalnya: LatihanVCS, kemudian klik tombol _create repository_.

![6](https://user-images.githubusercontent.com/73032342/96349398-8ded0300-10d9-11eb-98e4-ed2eaf596082.PNG)

**8. Menambahkan Remote Repository**

Untuk menambahkan remote repository server, gunakan perintah: 

`$ git remote origin [url]`

![7](https://user-images.githubusercontent.com/73032342/96349422-b248df80-10d9-11eb-9836-4428f98ac6e1.PNG)

**9. PUSH (Mengirim Perubahan ke Server)**

- Untuk mengirim perubahan pada local repository ke server gunakan perintah berikut:

`$git push -u origin master`

![9](https://user-images.githubusercontent.com/73032342/96349442-e3c1ab00-10d9-11eb-99dc-bb35c382483b.PNG)

**10. Melihat Hasil Pada Server Repository**

Buka laman [https://github.com/], arahkan pada repositorinya. Maka halaman tersebut akan berubah sesuai dengan repository yang telah anda buat sebelumnya.

![11](https://user-images.githubusercontent.com/73032342/96349705-89c1e500-10db-11eb-9b7d-c9e3a9c3ff25.PNG)

**11. Clone Repository**

Clone repository, pada dasarnya adalah mengcopy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory). untuk melakukan cloning, gunakan perintah berikut: `$ git clone [url]`

![10](https://user-images.githubusercontent.com/73032342/96349687-6303ae80-10db-11eb-8df8-6067693df225.PNG)
