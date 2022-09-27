# Membuat Layanan Microservice Sederhana

# About
Menggunakan Maven Spring
<br>Menggunakan Spiring Boot versi 2.6.11
<br>Memakai apache NetBeans IDE 13
<br>Memakai Bahasa Java
<br>Menggunakan JDK 17
<br>Memakai Microsoft Edge

## Donwload Project Maven
**Langkah 1 :** Buat Project Maven menggunakan spring Inirializr https://start.spring.io/
<br>**Langkah 2 :** pilih Maven project pada pilihan project, pilih bahasa java
<br>**Langkah 3 :** pilih springBoot versi 2.6.11 M6 atau versi yang lebih tinggi. Jangan memilih versi snapshot
<br>**Langkah 4 :** Berikan nama group pada project maven yang telah dibuat yaitu com.nadya
<br>**Langkah 5 :** Berikan id Artefak pada project yaitu latihan2-service dan secara otomatis akan mengisi bagian name
<br>**Langkah 6 :** Tambahkan description untuk project yang akan kita buat
<br>**Langkah 7 :** Pilih java atau jdk 17,pastikan sesuai dengan jdk yang tealah kita instals
<br>**Langkah 8 :** Tambahkan dependensi yaitu hanya spring web saja
<br>**Langkah 9 :** Lalu kita generate the project, file zip akan diunduh, setelah itu ekstrak file copekan file ke D,saya menyimpan file di D.
<br>**Langkah 10 :** Jalankan netbeans lalu import project yang telah kita ekstract tadi.Butuh beberapa waktu untuk mengunduh file yang diperlukan
<br>**Langkah 11 :** Lalu build and dependecies pada project yang sudah kita import
<br>**Langkah 12 :** Jalankan LimitServiceAplication, memulai tomcat pada port (s) 8010 (http)

# Project Spring Boot Baru
# Langkah 1 :Mulai Proyek Spiring Boot
<br>Menggunakan start.spring.io untuk membuat proyek "web". Dalam dialog "Dependencies" cari dan tambahkan ketergantungan "web" seperti yang ditunjukkan pada tangkapan layar. Tekan tombol "Generate", unduh zip,dan buka kemasannya ke dalam folder di komputer Anda.![image](https://user-images.githubusercontent.com/113502682/192451900-73ac9127-d298-4135-9b63-8b5c00c8854e.png)
# Langkah 2 :Tambahkan kode anda diNetbeans
<br>Buka proyek di IDE Anda dan cari file LatihanServiceApplication.java di Source Packages pada folder com.nadya.latiha2-nservice. Sekarang ubah isi file dengan menambahkan metode tambahan dan anotasi yang ditunjukkan pada kode di bawah ini. Anda dapat menyalin dan menempelkan kode atau cukup mengetiknya.![image](https://user-images.githubusercontent.com/113502682/192453499-c7f6780c-6b9d-4d7b-9c87-2609bb1af848.png)  
Metode hello() yang di tambahkan dirancang untuk mengambil parameter String yang disebut name, dan kemudian menggabungkan parameter ini dengan kata "Hello"dalam kode. Ini berarti bahwa jika Anda menyetel name dengan “Latihan 2” dalam permintaan, responsnya adalah “Hello Latihan 2”Anotasi @RestController memberi tahu Spring bahwa kode ini menjelaskan titik akhir yang harus tersedia melalui web. @GetMapping(“/hello”) memberi tahu Spring untuk menggunakan method hello() untuk menjawab permintaan yang dikirim ke alamat http://localhost:8080/hello.
# Langkah 3 :Cara Menukar Port
<br>Pada projek yang tadi, pergi ke Other Sources >> src/main/resources >> default package >> application.properties. Lalu buat server.port= *nomorPort* pada application.packages agar tidak terjadi bentrok antar port.![image](https://user-images.githubusercontent.com/113502682/192455075-51dfb755-2fbb-464a-bd87-55c265791152.png)
# Langkah 4 :Jalankan Program
<br> Untuk menjalankan program kita klik kanan >> run file. ![image](https://user-images.githubusercontent.com/113502682/192456255-b35d6cf6-95dc-4b4b-9f74-91e2132c1d3c.png)Server Apache Tomcat tertanam pada Spring Boot bertindak sebagai server web dan mendengarkan permintaan pada localhost port 8010. Buka browser Anda dan di bilah alamat di bagian atas enter http://localhost:8010/halo. Anda harus mendapatkan respons ramah yang bagus seperti ini:![image](https://user-images.githubusercontent.com/113502682/192456794-ac5e267c-42fc-4b7b-9696-ea1b76586d71.png)
