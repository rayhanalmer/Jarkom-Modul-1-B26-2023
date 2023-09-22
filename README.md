# Jarkom-Modul-1-B26-2023

Anggota Kelompok 

|   Nama                             | NRP      |
| ------                             | ------   |
|  Nur Azizah                        |5025211252|
|  Rayhan Almer Kusumah              |5025211115|
|  Faiz Haq Noviandra Ciptadi Putra  |5025211132|

## Soal 1
User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.
### Jawaban 
Pertama-tama kita memfilter data pada file dengan memunculkan data dengan protokol FTP saja, kemudian kita pilih 2 yang mengandung request & response dari GrabtheFisher.zip
![no1a](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/no1-a.jpg)
Kemudian kita lihat pada list TCP request untuk menemukan jumlah sequence number (raw) dan acknowledge number nya
![no1b](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/no1-b.jpg)
Lalu untuk sequence number response dan acknowledge number response-nya bisa kita lihat pada list TCP response dibawah ini
![no1c](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/no1-c.jpg)
Untuk dokumentasi terminal dalam menemukan flagnya seperti dibawah ini
![no1terminal](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/no-1terminal.jpg)

## Soal 2
Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!
### Jawaban
Pertama-tama kita akan membuka file pcapng yang ditujukan untuk no 2, lali pada display filter kita akan mencari paket yang memiliki source yang sama dengan IP Address web AJK yaitu 10.21.78.111 dengan command “ip.addr == 10.21.78.111”
![no2a](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/no2-a.jpg)
Kemudian kita bisa melihat server apa yang dipakai oleh paket tersebut dengan melihat menu HTP nya
![no2b](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/no2-b.jpg)
Dokumentasi terminal flag nya seperti dibawah ini
![no2terminal](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/no2-terminal.jpg)

## Soal 3
Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
### Jawaban
kita bisa dengan mudah cukup menuliskan filter expression yang diperlukan pada display filter seperti dibawah ini, lalu tampaklah jumlah paket yang tercapture serta protokol yang digunakan
![no3a](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/no3-a.jpg)
Dokumentasi pada terminalnya seperti dibawah ini
![no3terminal](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/no3-terminal.jpg)

## Soal 4
Berapa nilai checksum yang didapat dari header pada paket nomor 130?
### Jawaban
Pertama-tama kita akan mencari paket no 130 terlebih dahulu
![no4a](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/no4-a.jpg)
Lalu pada menu UDP nya kita bisa melihat nilai checksum yang diinginkan
![no4b](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/no4-b.jpg)

## Soal 5
Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.  
a. Berapa banyak packet yang berhasil di capture dari file pcap tersebut?  
b. Port berapakah pada server yang digunakan untuk service SMTP?  
c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?  

### Jawaban
```
a. 60
b. 25
c. 74.53.140.153
```

### Cara Pengerjaan
Untuk mendapatkan jawaban kami membuka package ke 14 yang terdapat informasi pass.  
Lalu buka package dengan klik kanan > follow > TCP Stream.  
Lalu akan ditemukan password seperti gambar dibawah yang harus di decode terlebih dahulu dalam Base64.
![5d_jawaban](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/5d_jawaban.png)  
Setelah didecode password yang didapatkan kita gunakan untuk membuka file zip.  
Isi file zip menampilkan nc/ncat seperti gambar berikut yang digunakan untuk menjawab soal.  
![5a_jawaban](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/5a_jawaban.png)  
Untuk point a bisa kita lihat di pojok kanan bawah terdapat informasi banyak package yang berhasil dicapture yaitu sebanyak 60 package.
![5b_jawaban](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/5b_jawaban.png)  
Untuk menjawab point b dan c, bisa ditemukan di informasi package seperti gambar dibawah.  
Ditemukan port sever yang digunakan untuk service SMTP adalah 25 dan IP yang merupakan IP public adalah 74.53.140.153  
![5c_jawaban](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/5c_jawaban.png)  

### Dokumentasi
![5_terminal](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/5_terminal.png)

## Soal 6
Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.

### Jawaban
```
JDRNJA
```

### Cara Pengerjaan
Untuk menemukan jawaban tersebut kita harus fokus pada clue yang ada di pertanyaan. kemuadian buka apk Wireshark dan filter dengan tulisan Frame.number == "code yang di pertanyaan". kemudian bakal muncul angka yang disitu ialah terdapat kode seperti a=1, b=2 dan seterusnya maka kita tinggan baca saja angka dan kalkulasikan.
![6  wireshark](https://github.com/faiznoviandra/6.wireshark/assets/116566988/460d10d5-c333-4688-86a5-5c2e10e94d5d)

### Dokumentasi Terminal
![6  Terminal](https://github.com/faiznoviandra/6.wireshark/assets/116566988/bf203ffa-68ea-47ca-808b-56304be05d56)

### Kendala Yang Dialami
Pada soal ini kendala yang saya temukann ialah saya tidak mengetahui bahwa ada code disoal



## Soal 7
Berapa jumlah packet yang menuju IP 184.87.193.88?

### Jawaban
```
6 
```

### Cara Pengerjaan
Untuk menemukan jawaban kami melakukan query filter sesuai permintaan soal dengan query `ip.dst == 184.87.193.88`.
Bisa dilihat pada gambar dibawah hasil package yang terdisplay yaitu sebanyak 6 package.
![7_jawaban](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/7_jawaban.png)

### Dokumentasi
![7_terminal](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/7_terminal.png)

### Kendala Yang Dialami

## Soal 8
Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)

### Jawaban
```
tcp.dstport == 80 || udp.dstport == 80
```

### Cara Pengerjaan
Query `tcp.dstport == 80` digunakan untuk menampilkan semua paket dengan protokol TCP dengan destination port 80.  
Query `udp.dstport == 80` digunakan untuk memfilter paket UDP dengan destination port 80.  
Kedua filter expression tersebut digabungkan menggunakan logical operator `||` (or).

### Dokumentasi
![8_terminal](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/8_terminal.png)

## Soal 9
Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!

### Jawaban
```
ip.src == 10.51.40.1 && ip.dst != 10.39.55.34
```
### Cara Pengerjaan
Query `ip.src == 10.51.40.1` digunakan untuk menampilkan semua paket yang memiliki source alamat ip 10.51.40.1.  
Query `ip.dst != 10.39.55.34` digunakan untuk memfilter paket sehingga tidak ada paket yang memiliki destination dengan alamat 10.39.55.34.    
Kedua filter expression tersebut digabungkan mengguanakan logical operator `&&` sehingga memenuhi permintaan soal.  

### Dokumentasi
![9_terminal](https://github.com/rayhanalmer/Jarkom-Modul-1-B26-2023/blob/main/images/9_terminal.png)

## Soal 10
Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet!

### Jawaban
```
dhafin:kesayangank0k0
```

### Cara Pengerjaan
Pertama-tama kita akan memfilter paket pada soal no 10 dengan memunculkan paket dengan protokol telnet saja. Lalu kita ambil 1 paket dengan nomor 236 untuk di follow dan kita cek TCP stream-nya yang terlihat seperti dibawah ini. 

![10  telnet](https://github.com/faiznoviandra/6.wireshark/assets/116566988/06a899da-8bf7-4111-bedc-1dede0c48a31)
![10  Jawaban](https://github.com/faiznoviandra/6.wireshark/assets/116566988/642c52d3-1cf4-4520-b58c-fe7ee933abae)

Bisa dilihat username dan password yang kita perlukan yaitu ‘dhafin’ dan ‘kesayangannyak0k0’, lalu kita masukkan jawabannya di terminal dan muncul seperti dibawah ini.

### Dokumentasi
![10  Terminal](https://github.com/faiznoviandra/6.wireshark/assets/116566988/7049abc9-dde4-4420-9040-733996cd945f)

### Kendala Yang Dialami
Tidak ada kendala yang dialami



