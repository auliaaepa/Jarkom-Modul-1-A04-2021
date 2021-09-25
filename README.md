# Jarkom-Modul-1-A04-2021

## Nama Anggota Kelompok 
### Julietta Anastasia Rodiah Boru Panjaitan (05111940000033)
### Aulia Eka Putri Aryani (05111940000044)
### Abdun Nafi’ (05111940000066)



### Soal 1
1.Sebutkan webserver yang digunakan pada "ichimarumaru.tech"! 
#### Penjelasan
Untuk mengetahui webserver apa yang digunakan pada `ichimarumaru.tech`, kami menggunakan display filter berupa `http.host == "ichimarumaru.tech"` pada wireshark, dan muncul tampilan seperti berikut.
<img width="1440" alt="Screen Shot 2021-09-25 at 07 14 15" src="https://user-images.githubusercontent.com/74484044/134751144-00853ef9-7d93-4c99-98b1-0ca8c5efd81c.png">

Setelah muncul tampilan tersebut, maka pilih salah satu dari hasil yang muncul, lalu klik kanan > ```Follow``` > ```TCP Stream``` seperti berikut ini.
<img width="1440" alt="Screen Shot 2021-09-25 at 07 18 41" src="https://user-images.githubusercontent.com/74484044/134751311-74d387d6-8fa7-43c0-8a03-399b0fdcf89c.png">

Lalu akan muncul tampilan berikut.
<img width="1440" alt="Screen Shot 2021-09-25 at 07 17 24" src="https://user-images.githubusercontent.com/74484044/134751275-4f5cfcdd-c9ef-4cfd-bb79-86f9fd0d33a1.png">

Dapat dilihat server yang tertera pada tampilan tersebut yakni, ```Server: nginx/1.18.0 (Ubuntu)```, dan itulah webserver yang digunakan pada `ichimarumaru.tech`.


### Soal 2
2.Temukan paket dari web-web yang menggunakan _basic authentication method_! 
#### Penjelasan
Untuk menemukan paket dari web yang menggunakan _basic authentication method_, kami menggunakan display filter berupa `http.authbasic` pada wireshark, sehingga diperoleh hasil sebagai berikut.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/2a.png)


### Soal 3
3.Ikuti perintah di basic.ichimarumaru.tech! Username dan password bisa didapatkan dari file .pcapng!
#### Penjelasan
Untuk mengetahui username dan password untuk memasuki portal ``` basic.ichimaru.tech ``` maka memasukkan source code berikut ```http.authbasic && http.host == basic.ichimarumaru.tech``` pada filter wireshark sehingga akan di dapatkan tampilan sebagai berikut :
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/3a.png)

Setelah muncul tampilan wireshark filter selanjutnya klik > ```Hypertext Transfer Protocol``` > ```Authorization```. Maka pada credentials akan muncul sebagai berikut :
dengan Username ```kuncimenujulautan``` dan Password ```tQKEJFbgNGC1NCZlWAOjhyCOm6o3xEbPkJhTciZN```. Setalah didapatkan pasword selanjutnya masukan username dan password 
pada portal ```basic.ichimarumaru.tech``` maka akan tampil sebuah pertanyaan sebagai sebagai berikut :
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/3b.png)

Dengan pertanyaaan mengenai Urutan Konfigurasi Pengkabelan T568A : 
Maka urutan dari kabel T568A adalah sebagai berikut :
```
Urutan ke 1 : Putih Hijau TD+ (data kirim+)
Urutan ke 2 : Hijau TD- (data kirim-)
Urutan ke 3 : Putih Orange RD+ (data terima +)
Urutan ke 4 : Biru NC (tidak dipakai)
Urutan ke 5 : Putih Biru NC (tidak dipakai)
Urutan ke 6 : Orange RD- (data terima -)
Urutan ke 7 : Putih Coklat NC (tidak dipakai)
Urutan ke 8 : Coklat NC (tidak dipakai)
```



### Soal 4
4.Temukan paket mysql yang mengandung perintah query select! 
#### Penjelasan
Untuk mencari paket mysql yang berisi perintah query select, kita dapat menggunakan display filter berupa `mysql.command==3 and frame matches "select"` pada wireshark, sehingga dapat diperoleh hasil sebagai berikut.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/4a.png)


### Soal 5
5.Login ke portal.ichimarumaru.tech kemudian ikuti perintahnya! Username dan password bisa didapat dari query insert pada table users dari file .pcap!
#### Penjelasan
Untuk mendapatkan pasword dan username yang didapat dari query insert  pada table users yaitu dengan cara memasukan kode ```mysql.command ==3 and frame matches "select"```
pada filter wireshark sehingga akan muncul tampilan paket sebagai berikut :
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/5a.png)

Setelah di dapatkan 4 paket maka pilih paket paling atas lalu ```klik kiri``` -> ```Follow``` -> ```TCP Stream```. Maka akan muncul berupa query sql select dengan username dan 
password sebagai berikut :
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/5b.png)

Didapatkan : 
```
Username : akakanomi
Password : pemisah4lautan
```
Setelah didapatkan pasword selanjutnya masukan Username dan Password pada portal ```portal.ichimarumaru.tech``` maka akan muncul sebuah pertanyaan mengenai Urutan Konfigurasi Pengkabelan T568B sebagai berikut :
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/5c.png)


Maka urutan dari kabel T568B adalah sebagai berikut :
```
Urutan ke 1 : Putih Orange RD+ (data terima+)
Urutan ke 2 : Orange RD- (data terima-)
Urutan ke 3 : Putih Hijau TD+ (data kirim +)
Urutan ke 4 : Biru NC (tidak dipakai)
Urutan ke 5 : Putih Biru NC (tidak dipakai)
Urutan ke 6 : Hijau TD- (data kirim -)
Urutan ke 7 : Putih Coklat NC (tidak dipakai)
Urutan ke 8 : Coklat NC (tidak dipakai)
```




### Soal 6
6.Cari username dan password ketika melakukan login ke FTP Server!
#### Penjelasan
Untuk mengetahui Username dan Password ketika melakukan login ke FTP Server maka masukan Command ```ftp.request.command == USER || ftp.request.command == PASS```
pada filter wireshark maka akan di dadapatkan hasil sebagai berikut :
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/6a.png)


### Soal 7
7.Ada 500 file zip yang disimpan ke FTP Server dengan nama 0.zip, 1.zip, 2.zip, ..., 499.zip. Simpan dan Buka file pdf tersebut. (Hint = nama pdf-nya "Real.pdf")
#### Penjelasan
Langkah awal yang kita lakukan yakni dengan memasukkan code `ftp-data contains Real.pdf` pada display filter wireshark, dan akan muncul tampilan seperti berikut.
<img width="1440" alt="Screen Shot 2021-09-25 at 08 49 33" src="https://user-images.githubusercontent.com/74484044/134753878-3f216a66-46b7-4028-b31f-f0f5dcffcaa1.png">

Setelah itu pilih salah satu hasil, dan klik kanan > `Follow` > `TCP Stream` seperti berikut ini.
<img width="1440" alt="Screen Shot 2021-09-25 at 08 52 17" src="https://user-images.githubusercontent.com/74484044/134753967-5a53dcbb-eb18-465e-8743-c247defa977f.png">

Kemudian akan muncul tampilan seperti dibawah ini.
<img width="1440" alt="Screen Shot 2021-09-25 at 08 59 00" src="https://user-images.githubusercontent.com/74484044/134754142-6fbe8c73-7f3e-4ad6-b2c5-2e6a7376d743.png">

Lalu ubah tampilan dengan memilih raw pada `Show data as : Raw`. Dan tampilan akan berubah.
<img width="1440" alt="Screen Shot 2021-09-25 at 09 01 45" src="https://user-images.githubusercontent.com/74484044/134754219-6e95a3c8-0dff-47fe-9287-364452985230.png">

Setelah itu klik `Save as` dan beri nama file dengan `Real.pdf`, lalu klik `Save`.
<img width="1440" alt="Screen Shot 2021-09-25 at 09 03 31" src="https://user-images.githubusercontent.com/74484044/134754249-5a3feec0-c8ab-460d-88ae-483ac6d7036f.png">

Dan berikut isi dari file `Real.pdf` yang telah disimpan tadi.

<img width="459" alt="Screen Shot 2021-09-25 at 09 07 14" src="https://user-images.githubusercontent.com/74484044/134754327-f4c3fcca-b930-4995-883e-de7ed6467fc5.png">


### Soal 8
8.Cari paket yang menunjukan pengunggahan file ke FTP tersebut!
#### Penjelasan
Untuk mencari paket yang menunjukan pengunggahan file ke FTP, maka kita dapat menuliskan `ftp.request.command==STOR` pada display filter wireshark, sehingga dapat diperoleh hasil sebagai berikut.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/8.png)


### Soal 9
9.Dari paket-paket yang menuju FTP terdapat inidkasi penyimpanan beberapa file. Salah satunya adalah sebuah file berisi data rahasia dengan nama "secret.zip". Simpan dan buka file tersebut!
#### Penjelasan
Untuk dapat menyimpan file yang berasal dari paket ftp, kita dapat menggunakan display filter `ftp-data.command contains "secret.zip"` pada wireshark, sehingga dapat diperoleh hasil sebagai berikut.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/9a.png)
Kemudian, `klik kanan` pada paket teratas, pilih `Follow`, pilih `TCP Stream`, ubah data menjadi `Raw`, dan `save as secret.zip`.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/9b.png)
Berikut adalah tampilan dari secret.zip yang berhasil disimpan.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/9c.png)


### Soal 10
10.Selain itu terdapat "history.txt" yang kemungkinan berisi history bash server tersebut! Gunakan isi dari "history.txt" untuk menemukan password untuk membuka file rahasia yang ada di "secret.zip"!
#### Penjelasan
Untuk membuka file history.txt, kita dapat menuliskan `ftp-data.command contains "history.txt"` pada display filter wireshark, sehingga diperoleh hasil sebagai berikut.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/10a.png)
Kemudian, `klik kanan` pada paket teratas, pilih `Follow` dan pilih `TCP Stream`, sehingga diperoleh tampilan sebagai berikut.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/10b.png)
Berdasarkan gambar tersebut, password dari file rahasia di secret.zip berada pada file `bukanapaapa.txt`. Oleh karena itu, kita harus membuka file bukanapaapa.txt terlebih dahulu untuk menemukan password nya. 
Untuk membuka file bukanapaapa.txt, kita dapat melakukan cara yang sama seperti file history.txt, yaitu dengan menuliskan `ftp-data.command contains "bukanapaapa.txt"` pada display filter wireshark, sehingga diperoleh hasil sebagai berikut.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/10c.png)
Kemudian, `klik kanan` pada paket teratas, pilih `Follow` dan pilih `TCP Stream`, sehingga diperoleh tampilan sebagai berikut.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/10d.png)
Berdasarkan gambar tersebut, password dari file rahasia di secret.zip adalah `d1b1langbukanapaapajugagapercaya`. Masukan password tersebut pada file rahasia yang ada di file secret.zip.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/10e.png)
Berikut adalah tampilan dari file rahasia yang berhasil terbuka.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/10f.png)


### Soal 11
11.Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80! 
#### Penjelasan
Untuk mengambil paket yang berasal dari port 80 maka masukan Command ```tcp.srcport==80```
pada filter wireshark maka akan di dadapatkan hasil sebagai berikut :
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/11a.png)


### Soal 12
12.Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
#### Penjelasan
Untuk mengambil paket yang mengandung port 21, maka kita bisa menuliskan code `tcp.port==21`, dan akan muncul hasil seperti berikut.
<img width="1440" alt="Screen Shot 2021-09-25 at 09 29 12" src="https://user-images.githubusercontent.com/74484044/134754881-455d375b-c6cd-4c72-97d2-f89c9a06a48a.png">


### Soal 13
13.Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!
#### Penjelasan
Untuk memfilter sehingga wireshark hanya menampilkan paket yang menuju port 443, maka kita bisa menuliskan code `tcp.dstport==443`, lalu akan muncul hasil seperti berikut ini.
<img width="1440" alt="Screen Shot 2021-09-25 at 09 30 43" src="https://user-images.githubusercontent.com/74484044/134754915-337a8c21-6daf-4f4b-bf44-31b20042db32.png">


### Soal 14
14.Filter sehingga wireshark hanya mengambil paket yang tujuannya ke kemenag.go.id!
#### Penjelasan
Untuk dapat melihat paket yang memiliki tujuan kemenag.go.id, pertama kita harus mencari `IP` dari kemenag.go.id terlebih dahulu. Untuk mencari IP, kita dapat menuliskan `ping kemenag.go.id` pada cmd.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/14a.png)
Berdasarkan hasil ping, IP dari kemenag.go.id adalah `103.7.13.247`. Setelah memperoleh IP, kita dapat menggunakannya pada display filter wireshark dengan menuliskan `ip.dst==103.7.13.247`, sehingga diperoleh hasil sebagai berikut.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/14b.png)

### Soal 15
15.Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
#### Penjelasan
Untuk dapat melihat paket yang berasal dari IP kita, pertama kita harus mencari `IP` kita terlebih dahulu, dengan cara menuliskan `ipconfig` pada cmd.
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/15a.png)
Berdasarkan hasil ipconfig, IP nya adalah `192.168.43.57`. Setelah mengetahui IP kita, kita dapat langsung menuliskan `ip.src==192.168.43.57` pada display filter wireshark , sehingga diperoleh hasil sebagai berikut. 
![image](https://github.com/auliaaepa/Jarkom-Modul-1-A04-2021/blob/master/img/15b.png)
