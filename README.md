# Jarkom-Modul-1-A04-2021

## Nama Anggota Kelompok 
### Julietta Anastasia Rodiah Boru Panjaitan  05111940000033 
### Aulia Eka Putri Aryani				            05111940000044 
### Abdun Nafi’					                      05111940000066 



### Soal 1
   1.Sebutkan webserver yang digunakan pada "ichimarumaru.tech"! 
### Penjelasan



### Soal 2
   2.Temukan paket dari web-web yang menggunakan basic authentication method! 
#### Penjelasan



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



### Soal 5
5.Login ke portal.ichimarumaru.tech kemudian ikuti perintahnya! Username dan password bisa didapat dari query insert pada table users dari file .pcap!
#### Penjelasan



### Soal 6
6.Cari username dan password ketika melakukan login ke FTP Server!
#### Penjelasan



### Soal 7
7.Ada 500 file zip yang disimpan ke FTP Server dengan nama 0.zip, 1.zip, 2.zip, ..., 499.zip. Simpan dan Buka file pdf tersebut. (Hint = nama pdf-nya "Real.pdf")
#### Penjelasan



### Soal 8
8.Cari paket yang menunjukan pengambilan file dari FTP tersebut!
#### Penjelasan



### Soal 9
9.Dari paket-paket yang menuju FTP terdapat inidkasi penyimpanan beberapa file. Salah satunya adalah sebuah file berisi data rahasia dengan nama "secret.zip". Simpan dan buka file tersebut!
#### Penjelasan



### Soal 10
10.Selain itu terdapat "history.txt" yang kemungkinan berisi history bash server tersebut! Gunakan isi dari "history.txt" untuk menemukan password untuk membuka file rahasia yang ada di "secret.zip"!
#### Penjelasan


### Soal 11
11.Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80! 
#### Penjelasan


### Soal 12
12.Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
#### Penjelasan


### Soal 13
13.Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!
#### Penjelasan


### Soal 14
14.Filter sehingga wireshark hanya mengambil paket yang tujuannya ke kemenag.go.id!
#### Penjelasan


### Soal 15
15.Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
#### Penjelasan










