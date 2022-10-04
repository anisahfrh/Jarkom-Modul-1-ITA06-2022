# Jarkom-Modul-1-ITA06-2022

## <b> Anggota Kelompok: </b>
1. Anisah Farah Fadhilah - 5027201023
2. Banabil Fawazaim Muhammad - 5027201055
3. Shafira Khaerunnisa - 5027201072
---

## Soal 1
Sebutkan web server yang digunakan pada "monta.if.its.ac.id"! 
### Penyelesaian soal 1
- Dengan menggunakan display filter `http.server` kemudian “Follow" > "TCP Stream” agar bisa mendapatkan response dari request
![soal1_1](https://user-images.githubusercontent.com/76768695/192086722-94db4bc1-edf2-4dc9-b3f5-2d027c5727b2.PNG)

Tampilan sebelum Follow TCP Stream

![soal1_2](https://user-images.githubusercontent.com/76768695/192086869-c130ff38-44db-4f2e-800e-fd3e42885a8e.PNG)
- Bisa dilihat dari hasil diatas, dalam respons header terdapat header dengan value server `nginx/1.10.3`

## Soal 2
Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh ishaq ?

### Penyelesaian soal 2
- Dengan menggunakan display filter `http.request.uri contains "detailTopik"`untuk menampilkan semua paket dengan protokol HTTP yang URL nya mengandung string "detailTopik"

![soal2_1](https://user-images.githubusercontent.com/76768695/193758705-f32821a0-5e6b-46fe-b391-7c7f79b496b6.PNG)

- Kemudian “Follow" > "TCP Stream” agar bisa mendapatkan response dari request

- Selanjutnya `ctrl+f` untuk mencari string "detailTopik" yang terhubung dengan link, maka didapatkan `http://monta.if.its.ac.id/index.php/topik/detailTopik/194`

![soal2_2](https://user-images.githubusercontent.com/76768695/192087738-11f465f8-443a-454b-9217-e3cb034dd885.PNG)

- Kemudian mengarahkan ke link tersebut, maka akan didapatkan detail topik TA dengan judul "Evaluasi unjuk kerja User Space Filesystem (FUSE)"
![soal2_3](https://user-images.githubusercontent.com/76768695/192087675-8073d0af-681c-473a-99e1-078d622ff608.PNG)

## Soal 3
Filter sehingga wireshark hanya menampilkan paket yang menuju port 80!
### Penyelesaian soal 3
- Untuk menampilkan paket menggunakan **Display Filter** pada Wireshark
- Port 80 menggunakan protokol **TCP**
- Sehingga, Display Filternya `tcp.dstport == 80`

![tcp.dstport == 80](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal3/soal3_1.jpg)

### Hasil soal 3

![hasil tcp.dstport == 80](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal3/soal3_2.jpg)

## Soal 4
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 21!

### Penyelesaian soal 4
- Untuk mengambil paket menggunakan **Capture Filter** pada Wireshark
- Port 21 menggunakan protokol **TCP**
- Sehingga, Capture Filternya `tcp src port 21` dan `Adapter for loopback traffic capture` untuk menangkap traffic lokal

![tcp src port 21](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal4/soal4_1.jpg)
- Buka **XAMPP** --> `Start` **FileZilla** --> Pilih **Admin**

![xampp](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal4/soal4_2.jpg)
- Buat user dan shared folder di `Edit`-`Users`, kemudian `OK`

![users](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal4/soal4_3.jpg)
- Buka Command Prompt, jalankan `ftp [ip address]`

![ftp [ip address]](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal4/soal4_4.jpg)
- Masukkan user dan password yang telah dibuat, kemudian lakukan beberapa command

![ftp command](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal4/soal4_5.jpg)

### Hasil soal 4

![hasil tcp src port 21](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal4/soal4_6.jpg)

## Soal 5
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 443!

### Penyelesaian soal 5
- Untuk mengambil paket menggunakan **Capture Filter** pada Wireshark
- Port 443 menggunakan protokol **TCP**
- Sehingga, Capture Filternya `tcp src port 443`

![tcp src port 443](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal5/soal5_1.jpg)

### Hasil soal 5

![hasil tcp src port 443](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal5/soal5_2.jpg)

## Soal 6
Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id !

### Penyelesaian soal 6
- Untuk menampilkan paket menggunakan **Display Filter** pada Wireshark
- Host lipi.go.id menggunakan protokol **HTTP**
- Sehingga, Display Filternya `http.host == lipi.go.id`

![http.host == lipi.go.id](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal6/soal6_1.jpg)

### Hasil soal 6

![hasil http.host == lipi.go.id](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal6/soal6_2.jpg)

## Soal 7
Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

### Penyelesaian soal 7
- Untuk menampilkan paket menggunakan **Capture Filter** pada Wireshark
- Sehingga, Capture Filternya `src host 192.168.131.81`

![src host 192.168.131.81](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal7/soal7_1.jpg)

### Hasil soal 7

![hasil src host 192.168.131.81](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/soal7/soal7_2.jpg)

Di sebuah planet bernama Viltrumite, terdapat Kementerian Komunikasi dan Informatika yang baru saja menetapkan kebijakan baru. Dalam kebijakan baru tersebut, pemerintah dapat mengakses data pribadi masyarakat secara bebas jika memang dibutuhkan, baik dengan maupun tanpa persetujuan pihak yang bersangkutan. Sebagai mahasiswa yang sedang melaksanakan program magang di kementerian tersebut, kalian mendapat tugas berupa penyadapan percakapan mahasiswa yang diduga melakukan tindak kecurangan dalam kegiatan Praktikum Komunikasi Data dan Jaringan Komputer 2022. Selain itu, terdapat sebuah password rahasia (flag) yang diduga merupakan milik sebuah organisasi bawah tanah yang selama ini tidak sejalan dengan pemerintahan Planet Viltrumite. Tunggu apa lagi, segera kerjakan tugas magang tersebut agar kalian bisa mendapatkan pujian serta kenaikan jabatan di kementerian tersebut!

Terdapat laporan adanya pertukaran file yang dilakukan oleh kedua mahasiswa dalam percakapan yang diperoleh, carilah file yang dimaksud! Untuk memudahkan laporan kepada atasan, beri nama file yang ditemukan dengan format [nama_kelompok].des3 dan simpan output file dengan nama “flag.txt”.
Temukan password rahasia (flag) dari organisasi bawah tanah yang disebutkan di atas!
Note: Terkait soal nomor 9 dan 10, file yang didapatkan tidak perlu dikumpulkan, cukup tulis flag yang didapatkan ke dalam laporan kalian 🙏.

## Soal 8

Telusuri aliran paket dalam file .pcap yang diberikan, cari informasi berguna berupa percakapan antara dua mahasiswa terkait tindakan kecurangan pada kegiatan praktikum. Percakapan tersebut dilaporkan menggunakan protokol jaringan dengan tingkat keandalan yang tinggi dalam pertukaran datanya sehingga kalian perlu menerapkan filter dengan protokol yang tersebut.

### Penyelesaian Soal 8

Kita akan menemukan payload berisi salah satu message dari dua mahasiswa tersebut, jika di follow maka kita akan mendapatkan filter nya yaitu `tcp.stream eq 12` dan yang kedua adalah `tcp.stream eq 41`

![hasil tcp.stream eq 12 or tcp.stream eq 41](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/no8-1.PNG)

## Soal 9

Terdapat laporan adanya pertukaran file yang dilakukan oleh kedua mahasiswa dalam percakapan yang diperoleh, carilah file yang dimaksud! Untuk memudahkan laporan kepada atasan, beri nama file yang ditemukan dengan format **[nama_kelompok].des3**  dan simpan *output file* dengan nama **“flag.txt”**.

### Penyelesaian Soal 9

Terjadi pengiriman file di port 9002, ikuti pakai `tcp.port eq 9002`, cari payload yang berisi tulisan salt.

![hasil tcp.stream eq 12 or tcp.stream eq 41](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/no9-1.PNG)

Dari hasil percakapan juga ada kata sandi yang memberikan clue anime kembar lima, langsung sajar saya menebak dengan key nakano

follow tcp nya, setelah itu dijadikan raw untuk disimpan menjadi ITA06.des3

![hasil tcp.stream eq 12 or tcp.stream eq 41](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/no9-2.PNG)

gunakan line berikut di openssl untuk mendecrypt file des3 nya `des3 -d -salt -in ITA06.des3 -o flag.txt -k nakano`

![hasil tcp.stream eq 12 or tcp.stream eq 41](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/no9-3.PNG)

dapatlah flag nya

## Soal 10

Temukan password rahasia (flag) dari organisasi bawah tanah yang disebutkan di atas!

Note: Terkait soal nomor 9 dan 10, file yang didapatkan tidak perlu dikumpulkan, cukup tulis flag yang didapatkan ke dalam laporan kalian 🙏.

### Penyelesaian Soal 10

![hasil tcp.stream eq 12 or tcp.stream eq 41](https://github.com/anisahfrh/Screenshot_Jarkom/raw/main/Modul1/no9-3.PNG)

## Kendala Pengerjaan
- Soal 4 sempat terjadi eror menjalankan FileZilla di XAMPP
