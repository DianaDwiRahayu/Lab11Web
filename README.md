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
<p> <b>Praktikum 12: Framework Lanjutan (CRUD)
<p> Pertanyaan dan Tugas </b>
<p> Selesaikan programnya sesuai Langkah-langkah yang ada. Anda boleh melakukan improvisasi. 
<p> Membuat Database : Studi Kasus Data Artikel
<p> Membuat database dengan nama lab_ci4 kemudian membuat table artikel

![1](https://user-images.githubusercontent.com/101866805/173764756-c2f91e0d-d7bd-4932-b6e2-bbef881883b1.png)
<p> Melalui file .env saya melakukan konfigurasi agar terhubung dengan database server, isi sesuai dengan database yang sudah dibuat sebelumnya

![2](https://user-images.githubusercontent.com/101866805/173765283-59e29d99-06b3-4454-9fc7-0f5defef1a73.png)
<p> Membuat model untuk memproses data Artikel. Buat file baru pada direktori app/Models dengan nama ArtikelModel.php

![3](https://user-images.githubusercontent.com/101866805/173765648-1bb73133-7695-4264-9c4f-59e1d7b6a771.png)
<p> Buat Controller baru dengan nama Artikel.php pada direktori app/Controllers

![4](https://user-images.githubusercontent.com/101866805/173765881-85403f02-437e-4120-bf0a-5f6cbd572187.png)
<p> Buat direktori baru dengan nama artikel pada direktori app/views, kemudian buat file baru dengan nama index.php

![5](https://user-images.githubusercontent.com/101866805/173766042-cac25fc3-737d-440c-93a8-b270acd6022d.png)
<p> Selanjutnya buka browser kembali, dengan mengakses url http://localhost:8080/artikel

![6](https://user-images.githubusercontent.com/101866805/173766823-39d51c84-eb0d-4d96-bf01-f72aa3cc852e.png)
<p> Menambahkan Data pada Database

![7](https://user-images.githubusercontent.com/101866805/173767187-e50ad650-e574-4af9-8460-7ea2a130ffc7.png)
<p> Refresh kembali halaman browser

![8](https://user-images.githubusercontent.com/101866805/173767333-47398c65-28ee-41af-82ea-d05247cac0e1.png)
<p> Membuat tampilan detail artikel dengan nama view() pada Controller Artikel

![9](https://user-images.githubusercontent.com/101866805/173768001-8234ce6a-f9ba-4311-941c-c2b95970e9f6.png)
<p> Membuat View Detail dengan nama app/views/artikel/detail.php

![10](https://user-images.githubusercontent.com/101866805/173768382-4023bd3e-eb3c-4329-8f6b-11f983c868ed.png)
<p> Membuat Routing untuk artikel detail pada Routes.php

![12](https://user-images.githubusercontent.com/101866805/173768882-6ae1f089-0319-4e2f-bfea-5862b46f160b.png)
<p> Selanjutnya buka browser kembali dengan mengakses url http://localhost:8080/artikel/artikel-kedua

![13](https://user-images.githubusercontent.com/101866805/173770732-b1d7be19-0d0a-4bc6-bf44-fe5dc1e58605.png)
<p> Membuat menu Admin untuk proses CRUD data atikel. Buat methode baru pada Controller Artikel dengan nama admin_index()

![14](https://user-images.githubusercontent.com/101866805/173771929-8a3f2003-1796-43ec-a707-8021fad8b128.png)
<p> Buat view dengan nama admin_index

![15](https://user-images.githubusercontent.com/101866805/173772255-62af69bf-3a62-4a81-b4b1-58fbb155016a.png)
<p> Membuat file admin_header dan admin_footer untuk tampilan

![23](https://user-images.githubusercontent.com/101866805/173773480-e75298ee-7225-477d-8d32-29d7920672b0.png)
![24](https://user-images.githubusercontent.com/101866805/173773493-49bc38c5-c4e8-42e5-8850-b2ae2cb5d490.png)
<p> Menambahkan routing untuk menu admin

![16](https://user-images.githubusercontent.com/101866805/173772453-db9867ac-4609-4426-b0ab-a52474a411f7.png)
<p> Selanjutnya ke browser dengan alamat url http://localhost:8080/admin/artikel

![17](https://user-images.githubusercontent.com/101866805/173772685-e6e39476-9a23-4a94-b154-41fba0c2857f.png)
<p> Menambah Data Artikel, tambahkan methode baru pada Controller Artikel dengan nama add()

![25](https://user-images.githubusercontent.com/101866805/173774843-c78ef037-6514-4c15-9150-9f6d7961749a.png)
<p> Buat view untuk form tambah dengan nama form_add.php

![26](https://user-images.githubusercontent.com/101866805/173775071-c5fc1272-e4ea-4550-9e28-b7b3a3be030e.png)
<p> Selanjutnya buka browser dengan url http://localhost:8080/admin/artikel/add

![18](https://user-images.githubusercontent.com/101866805/173775321-6bf07fde-9b68-48f4-991c-fe12d33704eb.png)
<p> Mengubah Data, tambahan methode baru pada Controller Artikel dengan anma edit()

![19](https://user-images.githubusercontent.com/101866805/173775595-5a2ec656-10b0-44bd-91cb-2f3d62010a7c.png)
<p> Kemudian membuat view untuk form tambah dengan nama form_edit.php

![20](https://user-images.githubusercontent.com/101866805/173775799-2b10a065-8308-4f5e-8f00-98e568750153.png)
<p> Selanjutnya buka browser dengan alamat url http://localhost:8080/admin/artikel/edit/1

![21](https://user-images.githubusercontent.com/101866805/173776072-a73b1acd-5a62-4e89-84dc-160d4574d96d.png)
<p> Menghapus Data, tambahkan methode baru pada Cotroller Artikel dengan nama delete()

![22](https://user-images.githubusercontent.com/101866805/173776342-73ee1706-7b13-4cb5-abc0-6b5af9620b56.png)
