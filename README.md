# Jarkom-Modul-1-ITA06-2022

## <b> Anggota Kelompok: </b>
1. Anisah Farah Fadhilah - 5027201023
2. Banabil Fawazaim Muhammad - 5027201055
3. Shafira Khaerunnisa - 5027201072
---

## Soal 1
Sebutkan web server yang digunakan pada "monta.if.its.ac.id"! 
### Penyelesaian soal 1

## Soal 2

### Penyelesaian soal 2


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

## Soal 8

### Penyelesaian soal 8

## Kendala Pengerjaan
- Soal 4 sempat terjadi eror menjalankan FileZilla di XAMPP