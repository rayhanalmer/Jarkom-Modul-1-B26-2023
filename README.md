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

## Soal 6

## Soal 7
Berapa jumlah packet yang menuju IP 184.87.193.88?

### Jawaban
```
6 
```

### Cara Pengerjaan

### Dokumentasi

### Kendala Yang Dialami

## Soal 8
Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)

### Jawaban
```
tcp.dstport == 80 || udp.dstport == 80
```

### Cara Pengerjaan

### Dokumentasi

### Kendala Yang Dialami

## Soal 9
Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!

### Jawaban
```
ip.src == 10.51.40.1 && ip.dst != 10.39.55.34
```
### Cara Pengerjaan

### Dokumentasi

### Kendala Yang Dialami

## Soal 10
