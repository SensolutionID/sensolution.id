+++
title = "Aplikasi Boris Untuk Pengamatan Proses Oral"
date = "2018-09-19T11:27:13+07:00"
tags = ["proses oral", "boris"]
categories = ["tips", "metode"]
banner = "img/banners/eat.jpeg"
+++

Proses oral (*oral processing*) merupakan salahsatu komponen penting yang diamati dalam bidang ilmu sensoris. Proses oral dapat diartikan sebagai rangkaian utuh sejak makanan dimasukan dalam mulut hingga akhirnya ditelan.

Proses oral terdiri atas beberapa paramater, diantaranya adalah gigitan pertama, ukuran gigitan, kekuatan gigitan, banyaknya kunyahan, frekuensi kunyahan, durasi, serta titik telan.

Terdapat bererapa metode untuk mengamati proses oral saat makan, misalnya melalui pengamatan video, *Electromyography* (EMG), *videofluorography*, sensor tekanan, *Magnetic Resonance Imaging* (MRI), dan lain-lain . Masing-masing metode memiliki fungsi, tujuan pemakaian, seta kelebihan dan kelemahan tersendiri.

Dalam tulisan ini saya akan membahas mengenai metode pengamatan proses oral berdasarkan pengamatan video. Metode ini sendiri dapat dikelompokan menjadi dua, yaitu berdasarkan pengamatan oleh pangamat (*observer*) dan berdasarkan analisis pergerakan titik (*dot movement tracking*). Secara khusus saya akan membahas mengenai metode berdasarkan pengamatan oleh pengamat.

Aplikasi yang dapat digunakan untuk tujuan ini misalnya adalah [Observer XT](http://www.noldus.com/human-behavior-research/products/the-observer-xt) dan [BORIS](http://www.boris.unito.it/). Observer XT merupakan aplikasi berbayar dan sumber tertutup yang umum dipakai di bidang sensoris. Aplikasi ini dikembangkan oleh *Noldus Information Technology* yang kebetulan memiliki kantor utama di kota tempat saya studi saat ini yaitu Wageningen. Sedangkan BORIS (*Behavioral Observation Research Interactive Software*) merupakan perangkat lunak bebas dan sumber terbuka yang dikembangkan oleh Olivier Friard and Marco Gamba. Kedua aplikasi tersebut memiliki fitur yang kurang lebih sama untuk digunakan dalam mengamati proses oral saat makan. Luaran yang akan didapatkan adalah parameter banyaknya kunyahan, titik telan, dan durasi makan,

# Mengunduh aplikasi BORIS
Dalam tulisan ini saya secara khusus akan membahas mengenai penggunaan aplikasi BORIS. BORIS merupakan aplikasi *multiplatform* sehingga dapat digunakan di sistem operasi Linux, Windows, maupun Mac. Anda dapat mengunduh aplikasi BORIS secara gratis melalui tautan [ini](http://www.boris.unito.it/pages/download.html).

![](/img/blog/boris-lp.jpg)

# Menggunakan aplikasi BORIS
![](/img/blog/boris-ip.jpg)

Alur kerja pemakaian BORIS untuk mengamati proses oral terdiri atas beberapa tahapan. Skenario pada contoh kasus ini adalah lima orang diminta untuk mengkonsumsi buah duku, makan kerupuk, dan meminum bandrek secara *ad libitum* (bebas jumlah dan durasi). Subyek direkam dari arah depan saat mengkonsumsi makanan dan minuman tersebut. Penyajian jenis makanan atau minuman dilakukan secara acak antar subyek. Parameter yang akan diamati adalah jumlah kunyahan, titik telan, dan durasi.

## Membuat Proyek
Proyek baru dapat dibuat  dengan cara klik '*File - New project*'. Silakan isi nama proyek pada *Project name*, tanggal pada *Date*, deskripsi proyek (disarankan untuk diisi) pada *Description*, dan pilih *Time format* sesuai kebutuhan.

![](/img/blog/boris-proyek-baru.jpg)

## Membuat atau mengubah *Ethogram*
*Ethogram* merupakan daftar perilaku atau parameter yang akan diamati melalui video. Masih pada jendela *new project*, pilih menu *Ethogram* kemudian tambahkan parameter dengan cara klik '*Add behaviour*'. Terdapat dua jenis perilaku yang dapat diatur di '*Behaviour type*', yaitu *Point even* dan *State even*. *Point even* merupakan perilaku yang terjadi sangat cepat, sedangkan *State even* merupakan kondisi yang memiliki durasi tertentu. Pada kasus ini, 'kunyahan' dan 'telan' merupakan *Point even* sedangkan durasi makan termasuk dalam *State even*. Hal terpenting adalah memberikan kunci tombol dan kode pada masing-masing perilaku yang akan digunakan saat mengamati video. Masing-masing diatur pada bagian '*Key*' dan '*Code*' seperti tangkapan layar berikut:

![](/img/blog/boris-ethogram.jpg)

## Menentukan obyek yang akan diamati
Obyek yang akan diamati dalam kasus ini adalah buah duku, kerupuk, dan bandrek. Pengaturan ini dilakukan masih dalam jendela '*new project*' pada menu '*Subject*'. Silakan menambahkan obyek dengan cara klik '*Add subject*' kemudian atur tombol kunci, nama, serta deskripsi masing-masing pada menu '*Key*', '*Subject name*', dan '*Description*' seperti berikut:

![](/img/blog/boris-subyek.jpg)

Setelah semua diatur maka silakan klik '*OK*'. Anda dapat melakukan perubahan terhadap proyek yang telah dibuat dengan cara klik '*File - Edit Project*'.

## Memulai pengamatan
Pengamatan dilakukan satu per satu setiap partisipan. Klik '*Observations - New Observation*'. Masukan '*Observation id*', deskripsi, dan tambahkan dokumen rekaman video dengan cara klik '*Add media*'. Jika terdapat lebih dari satu dokumen rekaman video, Anda dapat menambahkannya pada tab '*Player 2*'. Anda dapat mengatur selisih waktu rekaman dengan cara mengubah nilai '*Time offset*' jika diperlukan.

![](/img/blog/boris-tambah-observasi.jpg)

## Melakukan pengamatan
Pengamatan dapat dilakukan setelah Anda klik '*Start*' pada jendela '*New observation'*. Di bawah menu bar terdapat beberapa fitur kontrol video untuk memutar video, mengatur kecepatan video, dan opsi media video. Saat video sedang berjalan, parameter perilaku dapat diamati dan dicatat dengan cara menekan tombol kunci tiap perilaku (*ethogram* disajikan pada bagian kiri atas layar). Daftar parameter perilaku yang diamati beserta catatan waktu direkam dan disajikan pada bagian kanan layar. Pada kasus ini, Partisipan_001 sedang mengkonsumsi kerupuk sehingga kita harus mengatur fokus (*Focal subject*) dengan cara menekan tombol kunci kerupuk yaitu tombol huruf B (daftar obyek dan tombol kunci dapat dilihat pada bagian kiri bawah layar). Saat obyek telah berganti, misalnya obyek berikutnya adalah buah duku, maka pengamat dapat mengganti fokus dengan cara menekan tombol kunci untuk buah duku (tombol huruf 'A'). 

![](/img/blog/boris-pengamatan.jpg)

Setelah pengamatan untuk Partisipan_001 selesai, klik '*Observation - Close observation*. Selanjutnya pengamatan untuk Partisipan_002 atau selanjutnya dapat dilakukan dengan mengulangi tahapan '*Observations - New Observation*'.

## Mengekspor Hasil Pengamatan
Hasil pengamatan untuk seluruh partisipan dapat dilakukan dengan cara klik '*Observations - Export aggregated events*' kemudian pilih '*Select all*' dan klik '*OK*'. Selanjutnya centang semua *Subject* dan *Behaviour* dan klik '*OK*'. 

![](/img/blog/boris-ekspor.jpg)

Simpan dokumen ekspor dengan esktensi *.csv untuk mempermudah pengolahan data dengan aplikasi lainnya.

Demikian merupakan cara menggunakan aplikasi BORIS untuk melakukan pengamatan proses oral saat makan. Sebagai catatan, terlepas dari aplikasi yang digunakan, pengamatan melalui video memerlukan setidaknya dua orang pengamat independen untuk meminimalisasi subyektifitas. Oleh karena itu, dalam tulisan yang akan datang saya akan membahas mengenai cara pengamatan proses oral menggunakan video dengan metode *dot movement tracking*. Metode ini dapat dibilang lebih obyektif, bekerja secara otomatis dan relatif lebih cepat dibandingkan metode pengamatan oleh pengamat. Selamat mencoba!

[Tulisan ini dibagikan ulang dari aswansyahputra.com](https://aswansyahputra.com/post/aplikasi-boris-untuk-pengamatan-proses-oral/)

