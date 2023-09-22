# Jarkom-Modul-1-E17-2023

## Soal 1
User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.
### a. Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut?
- Cara Pengerjaan
- Screenshoot 
- Kendala

### b. Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut?
- Cara Pengerjaan
- Screenshoot 
- Kendala

### c. Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
- Cara Pengerjaan
- Screenshoot 
- Kendala

### d. Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
- Cara Pengerjaan
- Screenshoot 
- Kendala


## Soal 2
Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!
- Cara Pengerjaan
- Screenshoot 
- Kendala


## Soal 3
Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
### a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?
- Cara Pengerjaan
    - buka file wireshark yang sudah di download
    - pasang display filter ```(ip.src == 239.255.255.250 or ip.dst == 239.255.255.250) and udp.port == 3702``` untuk memfilter IP source ataupun destination berdasarkan port yang diinginkan.
    - hitung banyaknya paket yang telah difilter
- Screenshoot
  ![Alt text](modul1_image/no3.png)
  ![Alt text](modul1_image/no3_ubuntu.png)
- Kendala
  </br>Bingung cara membuat 2 kondisi filter yaitu mendapatkan IP dan filter port, sehingga waktu itu saya hanya memfilter IP adrresnya dan menghitung manual port dengan melihat pada detail paketnya:)

### b. Protokol layer transport apa yang digunakan?
- Cara Pengerjaan
  - masih berada di paket yang sama dan pada filter yang sama
  - lihat protocol apa yang digunakan pada IP addres 239.255.255.250 port 3702
- Screenshoot
  ![Alt text](modul1_image/no3.png)
  ![Alt text](modul1_image/no3_ubuntu.png)
- Kendala
  </b>tidak ada


## Soal 4
Berapa nilai checksum yang didapat dari header pada paket nomor 130?
- Cara Pengerjaan
  - Buka file wireshark yang sudah di download
  - Cari paket dengan nomor 130
  - Klik 2 kali pada paket, nanti akan muncul detai paketnya
  - Cari nilai  checksumnya pada bagian ```user diagram protocol```
- Screenshoot
  ![Alt text](modul1_image/no4.png)
  ![Alt text](modul1_image/no4_ubuntu.png)
- Kendala
  </br>Agak susah dalam mencari checksumnya pada detail paket


## Soal 5
Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.
### a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?
- Cara Pengerjaan
- Screenshoot 
- Kendala

### b. Port berapakah pada server yang digunakan untuk service SMTP?
- Cara Pengerjaan
- Screenshoot 
- Kendala

### c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?
- Cara Pengerjaan
- Screenshoot 
- Kendala



## Soal 6
Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan **"server SOURCE ADDRESS 7812 is invalid"**. ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.
- Cara Pengerjaan
  - Buka file wireshark yang sudah di download
  - Cari nomor paket yang diinginkan yaitu 7812
  - Copy IP source address paket tersebut
  - Buka website A1Z26 untuk men-decrypt IP address nya
  - Setelah itu akan muncul code resultnya, pilih yang A=1
- Screenshoot
  ![Alt text](modul1_image/no6.png)
  ![Alt text](modul1_image/no6_a1z26.png)
- Kendala
  kurang mengerti apa yang dimaksudkan soal tersebut, sehingga kelompok kami tidak solve no6 waktu praktikum


## Soal 7
Berapa jumlah packet yang menuju IP 184.87.193.88?
- Cara Pengerjaan
  - Buka paket yang telah di download sesuai soal
  - Terapkan display filter ```ip.dst``` untuk menyaring paket yang menuju ke IP 184.87.193.88 
  - Lalu lihat jumlah paket yang telah difilter pada bagian bawah jendela Wireshark.
- Screenshoot
  ![Alt text](modul1_image/no7.png)
  ![Alt text](modul1_image/no7_ubuntu.png)
- Kendala
  </br>tidak ada

## Soal 8
Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)
- Cara Pengerjaan
  - Mencari filter yang sesuai dengan kondisi yang diminta
  - Dengan filter ```tcp.dstport == 80 || udp.dstport == 80``` Wireshark akan menampilkan semua paket yang menuju ke port 80, baik menggunakan protokol TCP atau UDP.
  - Jika ada lebih dari satu port 80 yang muncul dalam paket yang sedang ditangkap, Wireshark akan menampilkan semuanya dan akan mengurutkannya secara alfanumerik (sesuai abjad).
- Screenshoot
  ![Alt text](modul1_image/no8.png)
- Kendala
  </br>Tidak ada


## Soal 9
Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!
- Cara Pengerjaan
- Screenshoot 
- Kendala


## Soal 10
Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet
- Cara Pengerjaan
- Screenshoot 
- Kendala
