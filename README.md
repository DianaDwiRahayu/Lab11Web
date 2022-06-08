<b> Nama : Diana Dwi Rahayu
<p> NIM : 312010055
<p> Kelas : TI.20.D1
<p> Mata Kuliah : Pemograman Web
<p>Pertanyaan dan Tugas </b>
<p> Lengkapi kode program untuk menu lainnya yang ada pada Controller Page, sehingga semua link pada navigasi header dapat menampilkan tampilan dengan layout yang
sama.
<p> 1. Melakukan konfigurasi pada web server dengan membuka Xampp control panel kemudian pada bagian Apache klik config>PHP.ini
<p> Pada bagian extention hilangkan tanda ; (titik koma pada pada ekstensi yang akan diaktifkan.

![26](https://user-images.githubusercontent.com/101866805/172610099-0c9dcac1-352c-433f-a485-0fb2063d0ca9.png)
![1](https://user-images.githubusercontent.com/101866805/172610696-1013be73-58c4-4eda-b064-f20518d32218.png)
<p> <b> Instalasi Codeigniter </b>
<p> Unduh Codeigniter dari website https://codeigniter.com/download
<p> Extrak file zip Codeigniter ke direktori htdocs/Lab11_ci
<p> Ubah nama direktory framework-4.x.xx menjadi ci4

![27](https://user-images.githubusercontent.com/101866805/172611353-9994309f-3c92-48c1-958b-315fd1c2a68c.png)
<p> Buka browser dengan alamat http://localhost/lab11_ci/ci4/public/

![3](https://user-images.githubusercontent.com/101866805/172611393-624643d9-78e3-4c59-a045-0fe06e08c905.png)
<p> Kemudian saya menggunakan cmd untuk konfigurasinya, arahkan lokasi direktory sesuai dengan direktory project (xampp/htdocs/lab11_ci/ci4/) kemudian jalankan perintah php spark

![4](https://user-images.githubusercontent.com/101866805/172612028-1b18c339-382d-4fb9-9c6c-f2ca0153a535.png)
![5](https://user-images.githubusercontent.com/101866805/172612068-e615b58e-0c44-444e-a3e2-67d651a14e34.png)
<p> <b> Mengaktifkan mode Debugging </b>
<p> Debugging digunakan untuk memudahkan developer untuk mengetahui pesan error apabila terjadi kesalahan dalam membuat kode program. Secara default fitur ini belum aktif. Ketika terjadi error pada aplikasi akan ditampilkan pesan kesalahan seperti berikut.

![6](https://user-images.githubusercontent.com/101866805/172612657-cc906b82-f73c-4d32-b717-ba50652d7bbc.png)
<p> Untuk mengetahui jenis errornya, maka perlu diaktifkan mode debugging dengan mengubah nilai konfigurasi pada environment variable CI_ENVIRINMENT menjadi development, Ubah nama file env menjadi .env

![30](https://user-images.githubusercontent.com/101866805/172618706-69224621-3a26-46ad-89f9-67a7cb059ae9.png)
![8](https://user-images.githubusercontent.com/101866805/172612674-dfb545ba-bb8c-49ff-9a2e-f3d899513c64.png)
<p> Ubah kode pada file app/Controller/Home.php hilangkan titik koma pada akhir kode

![7](https://user-images.githubusercontent.com/101866805/172613147-25eaf01e-b0e1-42ef-b7ff-c6d1dc658af3.png)
<p> <b> Routing dan Controller </b>
<p> Router terletak pada file app/config/Routes.php. Membuat Route Baru. Tambahkan kode berikut di dalam Routes.php

![9](https://user-images.githubusercontent.com/101866805/172613687-d980600f-73bf-4fa1-a627-2e47102e4152.png)
<p> Untuk mengetahui route yang ditambahkan sudah benar, buka CLI dan jalankan perintah php spark routes

![10](https://user-images.githubusercontent.com/101866805/172613961-70368eb1-a57b-4f16-9d7b-db86352ca6a0.png)
<p> Selanjutnya coba akses route yang telah dibuat dengan mengakses alamat url http://localhost:8080/about

![11](https://user-images.githubusercontent.com/101866805/172614086-d1a51b2e-2f76-4f24-84dc-baa4b88c5cf7.png)
<p> Itu artinya file/page tersebut tidak ada. Untuk dapat mengakses halaman tersebut, harus dibuat terlebih dahulu Contoller yang sesuai dengan routing yang dibuat yaitu Contoller Page.
<p> Membuat Controller Selanjutnya adalah membuat Controller Page. Buat file baru dengan nama page.php pada direktori Controller kemudian isi kodenya seperti berikut refresh kembali halaman about

![28](https://user-images.githubusercontent.com/101866805/172614846-149f6eda-298d-4508-9322-2c02d2d010d4.png)
![12](https://user-images.githubusercontent.com/101866805/172615003-c2ad93e9-2a39-4ffe-b19e-c58e85305f4e.png)
<p> <b> Auto Routing </b>
<p> Secara default fitur autoroute pada Codeiginiter sudah aktif. Untuk mengubah status autoroute dapat mengubah nilai variabelnya. Untuk menonaktifkan ubah nilai true menjadi false.

![13](https://user-images.githubusercontent.com/101866805/172615440-40d507a8-f714-408c-ac93-e1a9816af168.png)
<p> Tambahkan method baru pada Contorller page seperti berikut

![29](https://user-images.githubusercontent.com/101866805/172615682-867896c1-a53c-47e9-86d7-819601b22bf9.png)
<p> Method ini belum ada pada routing, sehingga cara mengaksesnya dengan menggunakan alamat: http://localhost:8080/page/tos

![15](https://user-images.githubusercontent.com/101866805/172615861-40b6856b-a4e8-44e5-8525-7136ab9d0c70.png)
<p> <b> Membuat View </b>
<p> Selanjutnya adalam membuat view untuk tampilan web agar lebih menarik. Buat file baru dengan nama about.php pada direktori view (app/view/about.php) kemudian isi
kodenya seperti berikut

![16](https://user-images.githubusercontent.com/101866805/172616425-6ee8b22c-9d4f-4239-8214-24d78e8e0cc3.png)
![17](https://user-images.githubusercontent.com/101866805/172616439-fba47588-9fea-4caa-b8d6-9729f0b591f9.png)
<p> Kemudian refresh pada halaman tersebut

![18](https://user-images.githubusercontent.com/101866805/172616542-2ef5197e-e818-42d2-9f46-e3c6accd5809.png)
<p> Membuat Layout Web dengan css, saya copy file css dari tugas praktikum 4 kemudian simpan pada directory public

![19](https://user-images.githubusercontent.com/101866805/172617114-60c3c261-e752-49c3-965e-7d9d54b807ff.png)
<p> Kemudian buat folder template pada direktori view kemudian buat file header.php dan footer.php seperti berikut

![20](https://user-images.githubusercontent.com/101866805/172617275-05f08839-d29b-4c37-af54-cd0ba514b9d1.png)
![21](https://user-images.githubusercontent.com/101866805/172617298-5f87b553-69d8-4f5f-9787-a25abc715f4c.png)
<p> Ubah file about seperti beikut 

![22](https://user-images.githubusercontent.com/101866805/172617482-eafc63eb-5ad7-4c8d-9f24-807ec09ab23c.png)
<p> Selanjutnya refresh tampilan pada alamat http://localhost:8080/about

![23](https://user-images.githubusercontent.com/101866805/172617570-f2c87190-a9e0-42c9-b104-43bf75fc6a94.png)
<p> Lengkapi kode program Controller page lainnya

![24](https://user-images.githubusercontent.com/101866805/172617752-c927ddbf-76a8-464a-beb1-ab9adea6104a.png)
![25](https://user-images.githubusercontent.com/101866805/172617763-2db79ed6-885b-4ae1-a976-428f57126a12.png)
