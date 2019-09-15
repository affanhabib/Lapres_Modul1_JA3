# Laporan Resmi Praktikum Modul 1

Praktikum Modul 1 mata kuliah Jaringan Komputer berisi cara *Crimping* dan *Filter* pada *Wireshark*. Saat *Crimping*, diberi waktu 10 menit untuk membuat jenis kabel, yaitu *Straight* dan *Cross*. Untuk *Filter* pada *Wireshark*, menggunakan *Capture Filter* dan *Display Filter*.

## Capture Filter

Untuk *Capture Filter*, menggunakan bagian seperti gambar dibawah ini pada *Wireshark*.
![Capture Filter](images/capture_filter.png)
 Ada 5 soal yang disajikan, yaitu:
 1. Filter sehingga wireshark hanya mengambil paket yang mengandung port 21
 	**Jawab**:
	
	Pada *Capture Filter* ketik `tcp port 21`. Paket akan muncul ketika kita membuka *FIlezila*. Karena sedang tidak membukanya, maka tampilan hanya seperti berikut:
	![Tampilan port 21](images/capture1.png)

 2. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80 (ajk.if.its.ac.id)
	**Jawab**:

	Masukkan `src port 80`. Setelah itu buka [ajk.if.its.ac.id](ajk.if.its.ac.id). Tampilan pada *Wireshark* akan seperti dibawah ini:
	![Tampilan source port 80](images/capture2.png)
 
 3. Filter sehingga wireshark hanya menampilkan paket yang menuju port 443 (google.com)
	**Jawab**:

	Ketik `dst port 443`. Dalam soal, untuk mengetes menggunakan [google.com](google.com). Tetapi saat kami menjalankannya, kami telah membuka [youtube.com](youtube.com) dan [stackedit.io](stackedit.io). *Wireshark* menampilkan seperti ini:
	![Tampilan destination port 443](images/capture3.png)

 4. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian
	**Jawab**:
	
	Pertama mencari IP dengan `ipconfig` pada *command promt*. 
	![Tampilan ipconfig](images/ipconfig.png)
	Diketahui IP kami `192.168.88.108`. Kemudian pada *Wireshark* ketik `ip src 192.168.88.108`. Hasilnya seperti dibawah ini:
	![Tampilan source dari ip sendiri](images/capture4.png)

 5. Filter sehingga wireshark hanya mengambil paket yang tujuannya ke monta.if.its.ac.id
	**Jawab**:

	Ketik `dst host monta.if.its.ac.id`. Kemudian buka [monta.if.its.ac.id](monta.if.its.ac.id). Hasil akan seperti berikut:
	![Tampilan destination monta.if.its.ac.id](images/capture5.png)


## Display Filter

*Display Filter* pada praktikum kali ini telah disediakan file *Wireshark* untuk menjawab 15 soal yang telah diberikan. Pertama buka file `no1-no15.pcapng` di *Wireshark*. Tampilan akan seperti gambar dibawah ini.
![Open file no1-no15.pcapng](images/open_file.png)
Kemudian kita menjawab sesuai perintah soal menggunakan *Display Filter*.
**Soal**
1.  Tampilkan semua paket yang hostnya mengandung "www.ne.its.ac.id"
**Jawab**:

    
2.  Tampilkan paket yang hanya berasal dari IP 10.151.36 81 dan menuju web "mb.its.ac.id"
**Jawab**:

    
3.  Simpan gambar ckedokteran.png
**Jawab**:

    
4.  Cari charset dari halaman "ajk.if.its.ac.id"
**Jawab**:

    
5.  Cari username dan password ketika login di "freeshare.lp.if.its ac.id"
**Jawab**:

    
6.  Sebutkan web server yang digunakan pada "[www.ne.its.ac.id](http://www.ne.its.ac.id)"
**Jawab**:


7.  Sebutkan versi PHP dan yang digunakan pada "riset.ajk.if.its.ac.id"
**Jawab**:


8.  Filter pada wireshark kalian sehingga menampilkan hasil ping
**Jawab**:

    
9.  Dapatkan semua metode GET yang mengakses "monta.if.its.ac.id"
**Jawab**:

    
10.  Tunjukkan username dan password yang dimasukkan ketika login FTP
**Jawab**:

    
11.  Tunjukkan di wireshark, paket mana yang dikirimkan FTP client ketika upload file "qwpeaspojdasjfpasjfpaosuhuy.jpg"
**Jawab**:

    
12.  Tunjukkan di wireshark, paket mana yang dikirimkan FTP client ketika menghapus file "qwpeaspojdasjfpasjfpaos.jpg"
**Jawab**:

    
13.  Tunjukkan di wireshark, paket mana yang dikirimkan FTP client ketika mengganti nama file "sutlin.png"
**Jawab**:

    
14.  Tunjukkan di wireshark, paket mana yang dikirimkan FTP client ketika download file "sutlun.png"
**Jawab**:

    
15.  Cari file .zip di wireshark lalu download dan extract file tersebut
clue: "50 4B 03 04"
**Jawab**:

