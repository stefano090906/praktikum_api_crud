Nama     : Stefano Tessari Abur
kelas    : TRPL 2B
NIM      : 362458302014

1.	Tujuan praktikum
-	Memahami konsep dasar API (Application Programming Interface) dan REST API
-	Menggunakan package http di Flutter untuk melakukan permintaan (request) ke API eksternal
-	Melakukan operasi CRUD (Create, Read, Update, Delete) terhadap data melalui API
-	Mengurai data JSON (parsing) dan mengubahnya menjadi objek Dart (Model)
-	Menampilkan data dari API ke dalam UI Flutter menggunakan widget seperti ListView
-	Mengimplementasikan styling dasar pada komponen UI untuk menyajikan data den gan rapi
-	Mengelola state secara sederhana untuk menangani data yang bersifat asinkron (asynchronous)

2.	Dasar teori
-	API
API (Application Programming Interface) adalah seperangkat definisi, protokol, dan tools untuk membangun perangkat lunak aplikasi. Dalam praktikum ini, API bertin dak sebagai jembatan yang memungkinkan aplikasi Flutter (klien) Anda berkomunikasi dengan server (backend) untuk mengambil atau mengirim data 

-	REST
REST (Representational State Transfer) adalah gaya arsitektur yang paling umum digunakan untuk membuat API berbasis web. REST API menggunakan metode HTTP standar untuk melakukan operasi pada resources

-	JSON
JSON adalah format pertukaran data yang ringan dan mudah dibaca manusia serta di parsing oleh mesin. Hampir semua REST API menggunakan JSON sebagai format data utama

-	http package
Package http adalah library yang direkomendasikan untuk melakukan permintaan HTTP di Dart dan Flutter. Package ini menyediakan fungsi-fungsi mudah digunakan seperti http.get(), http.post(), http.put(), dan http.delete()


3.	langkah – langkah implementasi
-	Pembuatan proyek flutter baru
  <img width="719" height="486" alt="image" src="https://github.com/user-attachments/assets/b905945f-9dfc-48bb-ad5f-1898908f87fb" />

-	Menambahkan http : ^1.2.1 pada pubspec.yaml yang terletak di root proyek dan simpan perubahannya menggunakan flutter pub get
 <img width="727" height="265" alt="image" src="https://github.com/user-attachments/assets/acb556d4-5956-40cc-92e3-7d123c0b7305" />

-	Buat file baru bernama user_model.dart di dalam folder lib/
  <img width="575" height="605" alt="image" src="https://github.com/user-attachments/assets/a06b609b-e21e-4d4d-b920-4ec36358346f" />
  
-	Buat file baru Bernama api_service.dart didalam folder lib/
  <img width="869" height="1382" alt="image" src="https://github.com/user-attachments/assets/73275ae8-0d48-4ed8-aeba-867593b5dfcf" />

-	Buat file baru bernama add_user_page.dart didalam folder lib/
  <img width="480" height="1328" alt="image" src="https://github.com/user-attachments/assets/0ea613c6-c25e-4c58-b336-0de71092bfdf" />

-	edit file : main dart
  <img width="299" height="1367" alt="image" src="https://github.com/user-attachments/assets/0a167a66-5e42-4e60-8044-1405ac1c37ae" />

-	Buat file edit_user_page.dart
  <img width="512" height="1339" alt="image" src="https://github.com/user-attachments/assets/1fd171b8-3ce0-4382-b13b-bfd2f25c8afe" />

-	Buat file : api_config.dart
  <img width="620" height="256" alt="image" src="https://github.com/user-attachments/assets/ba567cb3-a88a-4fd9-8dd6-e55106de60d0" />
  
-	Hasil :
  <img width="399" height="888" alt="image" src="https://github.com/user-attachments/assets/7d911977-bf91-4c1a-9ed8-6e16875d28d5" />
  <img width="399" height="887" alt="image" src="https://github.com/user-attachments/assets/bca4c0b7-ca5e-421a-84a2-f09afc402332" />
  <img width="330" height="734" alt="image" src="https://github.com/user-attachments/assets/719ab09d-19d9-4470-8afc-6050938777d3" />
  <img width="329" height="731" alt="image" src="https://github.com/user-attachments/assets/eec48b10-187d-4b95-9293-52689a12083d" />
  <img width="309" height="686" alt="image" src="https://github.com/user-attachments/assets/eb5322aa-bf0f-472c-9be5-5fb765888d47" />


4.	Analisis code
disini saya ingin menjelaskan tentang file api_config dart :
Kelas ini berfungsi sebagai tempat penyimpanan konfigurasi global untuk API, dengan dua nilai penting:
•	baseUrl untuk alamat utama API
•	apiKey untuk kunci akses 
<img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/5eece2ee-b873-430a-9579-94d4c6d64b05" />

Disini juga saya sedikit menyeting pada jaringan, yang Dimana saya mematikan internet protocol version 6 (TCP/IPv6) fungsinya adalah membuat sistem hanya menggunakan IPv4, yang bisa membantu mengatasi masalah koneksi atau kompatibilitas jaringan. Namun, tindakan ini juga dapat membatasi akses ke layanan yang memerlukan IPv6 dan sebaiknya hanya dilakukan jika benar-benar diperlukan

<img width="442" height="248" alt="image" src="https://github.com/user-attachments/assets/bd6f502c-6a35-466a-8420-f4176cc0f504" />

Setelah itu untuk mengeceknya saya menggunakan terminal bawaan laptop/cmd dengan menggunakan perintah nslookup reqres.in


5.	Kesimpulan dan saran
-	Kesimpulan 
Kesimpulan dari praktikum ini adalah memahami konsep dasar API dan REST API, Menggunakan package http di Flutter untuk melakukan permintaan (request) ke API eksternal, Melakukan operasi CRUD (Create, Read, Update, Delete) terhadap data melalui API, Mengurai data JSON (parsing) dan mengubahnya menjadi objek Dart (Model), Menampilkan data dari API ke dalam UI Flutter menggunakan widget seperti ListView, Mengimplementasikan styling dasar pada komponen UI untuk menyajikan data dengan rapi, dan Mengelola state secara sederhana untuk menangani data yang bersifat asinkron (asynchronous).
-	Saran
Mungkin modul praktikum bisa di lengkapi lagi untuk langkah demi Langkah praktikumnya karena masih banyak mahasiswa yang masih kebingungan pada saat melakukan praktikum







