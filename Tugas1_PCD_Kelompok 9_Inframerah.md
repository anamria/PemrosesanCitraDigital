![Logo ulm](https://user-images.githubusercontent.com/112606990/188874672-07dbff81-fc9c-4a90-b5d0-a051f3e22671.png)

# Kelompok 9 - InfraMerah
### Anggota:
### - Fatimah Azzahra Maulida (2110131220020)
### - Ana Maria Parasanti (2110131320009)

---
## **Inframerah (Infrared)**

![inframerah](https://user-images.githubusercontent.com/112605121/188873991-bbf5c8cb-7f81-4bfe-a066-b7873cca4f4b.jpg)

## Pengertian

Inframerah adalah radiasi elektromagnetik dari panjang gelombang lebih panjang dari cahaya tampak, tetapi lebih pendek dari radiasi gelombang radio. Namanya berarti "bawah merah" (dari bahasa Latin infra, "bawah"), merah merupakan warna dari cahaya tampak dengan gelombang terpanjang. Radiasi inframerah memiliki jangkauan tiga "order" dan memiliki panjang gelombang antara 700 nm dan 1 mm. Inframerah ditemukan secara tidak sengaja oleh Sir William Herschell, astronom kerajaan Inggris ketika ia sedang mengadakan penelitian mencari bahan penyaring optis yang akan digunakan untuk mengurangi kecerahan gambar matahari pada teleskop tata surya.

## Karakteristik
1. Sumbernya bisa didapatkan dari radiasi panas
2. Memiliki panjang gelombang yang berbalik dengan suhu, yaitu ketika suhu naik maka panjang gelombang infra merah akan turun dan sebaliknya
3. Berpotensi diinterfensi oleh sinar matahari
4. Sinarnya tidak tertangkap mata manusia
5. Tidak bisa menembus objek yang tidak transparan

## Tipe Infra Merah Berdasarkan Jaraknya
1. Infra Merah Jarak Jauh

    Infra merah ini memiliki panjang gelombang 10 µm sampai 100 µm  sehingga cenderung jauh. Contohnya terdapat pada beberapa alat kesehatan misalnya gelang kesehatan.
2. Infra Merah Jarak Menengah

    Infrared ini memiliki panjang gelombang 1.5 µm sampai 10 µm sehingga tidak terlalu dekat maupun jauh. Contohnya terdapat pada sensor alarm.
3. Infra Merah Jarak Dekat

    Infrared jarak dekat memiliki panjang gelombang 0.75 µm sampai 1.5 µm saja. Contohnya terdapat pada alat untuk meningkatan penglihatan manusia pada kondisi cahaya yang sangat rendah seperti Nightscoop.

## Kelebihan dan Kekurangan Infra Merah

**Kelebihan**

- Tidak Terikat Waktu

    Transfer data atau file tidak terikat waktu (bisa dilakukan kapan saja) karena infra merah tidak membutuhkan sinyal dalam pengoperasiannya.
- Mudah Digunakan

    Pengiriman file mudah dilakukan siapa saja karena termasuk alat yang sederhana dan mudah digunakan.
- Bebas Biaya

    Transfer data dari satu perangkat ke perangkat lainnya tidak menggunakan biaya (gratis).
    
**Kekurangan**

- Tidak Praktis

    Saat melakukan pengiriman file dengan infrared, lubang infrared pada perangkat harus berhadapan satu sama lain sehingga cukup merepotkan. Pengiriman data pun terasa lebih sulit karena berpotensi data tidak terkirim.
- Cenderung Berbahaya

    Karena merupakan sinar elektromagnetik, infrared sangat berbahaya bagi penglihatan. Oleh karena itu, jangan sampai sorotan infra merah mengenai mata karena bisa menyebabkan berbagai penyakit berbahaya.
- Relatif Lamban

    Dibandingkan dengan media transfer data lain seperti bluetooth, kecepatan infrared mengirim data relatif lambat.

## Contoh Kasus
    Kasus: Mengukur kadar asam pada buah jeruk nipis dengan pengolahan citra digital yang menggunakan modul inframerah obstacle.

> Alat yang digunakan

Pembuatan   alat   terbagi   menjadi   pembuatan perangkat   keras   dan   pembuatan   perangkat lunak.    Modul/kompomen    elektronika    yang digunakan pada alat untuk melakukan pengukuran  kadar  asam  askorbat  antara  lain Kamera yang digunakan untuk mengambil citra larutan  yang  dititrasi,  Arduino  Nano,  Modul Inframerah obstacle,    motor    servo,    Motor pengaduk,   lampu   dan   perangkat komputer untuk  mengolah  citra digital  yang  ditangkap oleh kamera.

<img width="263" src="https://user-images.githubusercontent.com/112605121/188874094-1d97abe4-b93d-49ac-8a13-f8276aa731ef.PNG">

<img width="285" src="https://user-images.githubusercontent.com/112605121/188874210-12bb621d-37df-4b9d-8512-c6ca2536527f.PNG">

Modul   Inframerah obstacle adalah    sebuah modul    yang    berfungsi    sebagai    pendeteksi halangan  atau  objek  di  depannya.  Komponen utama  dari  modul  inframerah obstacle terdiri dari Infrared(IR) emitter dan Infrared(IR) receiver/phototransistor. Pada modul inframerah obstacleterdapat  Op-Amp  LM  365 yang  berfungsi  sebagai  komparator  tegangan dari   rangkaian   IR receiver dan   rangkaian pembagi    tegangan    dari trimpot    pengatur sensitivitas.    Keluaran    dari    Op-Amp (pin “OUT”) dihubungkan ke Arduino Nano.

Cara kerja dari modul inframerah obstacle yaitu ketika  diberikan  sumber  tegangan,  IR emitter memancarkan   cahaya   inframerah.   Kemudian jika ada objek di depan IR emitter, maka cahaya inframerah   tersebut   akan   dipantulkan   oleh objek yang berada di depan IR emitter tersebut. Cahaya   inframerah  yang   terpantul   kemudian diterima  oleh  IR receiver,  sehingga  resistansi IR receiver menjadi  kecil  sehingga  keluaran dari Op-Amp menjadi logika  high. Desain  rancangan  perangkat  keras  alat  untuk pengukuran  kadar  asam  askorbat  ditunjukkan oleh gambar 4 sebagai berikut.

<img width="347" src="https://user-images.githubusercontent.com/112605121/188874306-6096e4b6-493f-45db-9b36-dbcdbc736c72.PNG">

Dari    gambar    perancangan    perangkat    yang ditunjukkan   oleh   gambar   4,   posisi   kamera diletakkan  di  atas  wadah  larutan  yang  dititrasi dan mengarah pada larutan tersebut. Sedangkan modul  sensor  infra  merah  diletakkan  di  bawah ujung  buret.  Sensor  tersebut  digunakan  untuk mendeteksi  tetesan  I2.  Motor  servo  digunakan untuk   proses   buka   tutup   katub   pada   buret. Sedangkan  motor  pengaduk  digunakan  untuk mengerakkan  pengaduk  larutan  yang  dititrasi agar  I2 yang  menetes  ke  larutan  tersebut  cepat merata.    Lampu    yang    sinarnya    didifusikan diletakkan dibawah wadah larutan yang dititrasi untuk  memberikan  pencahayaan  pada  larutan yang dititrasi.

Dalam    pembuatanperangkat    lunak    sistem pengukur kadar asam askorbat dengan menerapkan   pengolah   citra   digital,   bahasa pemrograman  yang  digunakan  untuk  membuat perangkat   lunak   pengolah   citra   digital   pada perangkat komputer    menggunakan    bahasa pemrograman   Python   versi   2.7   dan libraryOpenCV  versi  3.2.  Sedangkan  pemrograman pada    Arduino    Nano    untuk mengendalikan motor  servo  dan  motor  DC  maupun  mengolah jumlah    tetesan    I2 menggunakan aplikasi Arduino IDE.

-Rancangan Perangkat Keras

Cara    kerja    pada    perangkat    lunak    untuk pengukuran  kadar  asam askorbat  terbagi  dalam tiga proses, dimana diagram alir program secara umum ditunjukkan gambar 5 sebagai berikut.

<img width="168" src="https://user-images.githubusercontent.com/112605121/188874478-a206c3a9-22a3-452b-9f41-0a7e32a54e83.PNG">

-Proses Titrasi

Titrasi  iodimetri merupakan  titrasi  redoks  yang menggunakan  larutan  standar  I2 sebagai  titran dalam  suasana  netral  atau  sedikit  asam. Persamaan  untuk  menghitung  kadar asam askorbat adalah

<img width="284" src="https://user-images.githubusercontent.com/112605121/188874519-df98ae72-3b04-4ad5-b109-3f2f08cca714.PNG">

Dimana V adalah  volume  I2 yang  diteteskan kedalam larutan yang dititrasi hingga titik akhir titrasi terbentuk. Saat  motor  servo  membuka  katub  buret  dan modul  sensor  infra  merah mendeteksi  adanya tetesan   I2maka   modul   sinyal   infra   merah mengirimkan   logika high(rising   edge)   ke Arduino  Nano  dan  kemudian  motor  pengaduk bekerja  untuk  mengaduk  larutan  dalam  waktu sesaat.  Logika  high  yang  dikirim  dari  modul sensor  infra  merah  ke  Arduino  Nano  disimpan menjadi   data   jumlah   tetasan.   Data   jumlah tetesan   tersebut   selanjutnya   akan   digunakan sebagai  perhitungan  untuk  menentukan  kadar asam askorbat    jika    proses    titrasi    sudah mencapai titik akhir titrasi.

-Proses Pengolahan Citra

<img width="197" src="https://user-images.githubusercontent.com/112605121/188874575-9e9065fb-21f6-48b9-823d-7217af918407.PNG">

Setelah    proses    Titrasi    dilanjutkan    proses pengolahan  citra.  Langkah  awal  dalam  proses pengolahan  citra  adalah  mengambil  citra  RGB melalui  kamera. Tahap selanjutnya pada proses pengolahan citra adalah mereduksi noise pada    citra    RGB    dengan menggunakan algoritma gaussian blur. Selanjutnya   citra   RGB   hasil gaussian   blur dilakukan segmentasi warna untuk memisahkan antara citra objek dengan citra latar berdasarkan ciri  dari  pemodelan  warna  tertentu  pada  suatu citra  objek  tersebut. Setelah itu, dilakukan seleksi warna  berdasarkan  parameter  maksimum  dan minimum  dari  setiap  komponen  pokok ruang warna yang telah   ditentukan. Proses seleksi  tersebut  bertujuan  untuk  menampilkan citra  obyek  yang  diinginkan  saja  pada  proses thresholding warna sehingga hanya menghasilkan  citra grayscale pada  citra  obyek saja    sebagai    citra    masukkan    pada    proses pengenalan obyek. Setelah  terdeteksi  warna  larutan  yang  dititrasi berdasarkan    parameter    warna    yang    telah ditentukan,  selanjutnya  dilakukan  pengenalan objek mengunakan Transformasi Hough. Proses   yang   dilakukan   pada HoughCircle Transform adalah  mencari  titik-titik  pada  citra yang  dianggap  sebagai  bagian  tepi  dari  suatu lingkaran. Hal tersebut bertujuan untuk menemukan titik  pusat  yang  sesungguhnya  dari  lingkaran yang   mengandung   titik-titik   tersebut.   Titik pusat  yang  sesungguhnya  baru  akan  diambil jika terdapat perpotongan antara lingkaran yang dibuat   oleh Hough   Circle   Transform.   Jika terdeteksi  banyak  pola  lingkaran  pada  suatu citra, maka akan ada kemungkinan timbul suatu titik   pusat   yang   tidak   sesuai.   Maka   dapat dilakukan  perbandingan  dengan  citra  aslinya.

-Proses Penghitungan Kadar Asam Askorbat

Setelah terdeteksi warna biru tua pekat dan pola lingkaran  yang  ditandai  dengan  adanya  garis lingkaran  pada  frame  citra  RGB  maka  proses titrasi dihentikan. Selanjutnya dilakukan penghitungan  kadar  asam  askorbat  oleh  alat pengukur  kadar  asam  askorbat  diperoleh  dari data   jumlah   tetesan   I2yang disimpan   oleh Arduino Nano.

Dalam   melakukan   perhitungan kadar   asam askorbat   berdasarkan   jumlah   tetesan   I2oleh sistem, maka persamaan yang digunakan untuk menghitung kadar asam askorbat adalah

<img width="210" src="https://user-images.githubusercontent.com/112605121/188874629-7bd4da21-5835-43d6-b09a-9f9cc653314d.PNG">

Dari persamaan diatas, persentase kadar asam askorbat yang di tampilkan pada layar monitor dihitung menggunakan persamaan sebagai berikut

<img width="206" src="https://user-images.githubusercontent.com/112605121/188874685-504c7f79-9164-4c4c-9add-979cea27d02d.PNG">

-Hasil Pengujian

Dari   hasil   pengujian,   data   yang diperoleh meliputi  data  citra  RGB,  citra  HSV,citra  hasil filter   pada   ruang   warna   HSV,   citra   hasil konversi ke   citra grayscalepada   beberapa jumlah  tetesan  I2. Citra  RGB  dan  Citra  HSV yang diperoleh dari  konversi RGB pada larutan yang  ditetesi  I2ditunjukkan  oleh  tabel  2  adalah citra yang didapatkan dari pengujian pertama. 

<img width="439" src="https://user-images.githubusercontent.com/112605121/188874725-adb26f4e-f90f-4d9d-8e87-f59d54e38fad.PNG">
<img width="426" src="https://user-images.githubusercontent.com/112605121/188874803-90a58ef6-6c1a-44d4-8874-6c8fe4f1f41a.PNG">

Dari  hasil  konversi  citra  RGB  ke  dalam  ruang warna  HSV   yang  ditunjukkan  oleh  tabel   2, Nampak  bahwa  penambahan  tetesan  I2yang menyebabkan  larutan  berubah  warna  menjadi biru  tua  pada  citra  RGB.  Perubahan  warna  biru tua  pada   citra  RGB  juga  menyebabkan  ada perubahan    warna    pada    citra    HSV    yang ditunjukkan     adanya     warna     hijau     muda.

Sedangkan  citra  hasil  filter  warna  pada  ruang warna  HSV  dan  citra  hasil  konversi  ke  citra grayscalepada   pengujian   pertama   disajikan oleh tabel 3 sebagai berikut.

<img width="465" src="https://user-images.githubusercontent.com/112605121/188874836-dd0ffe14-6598-40e7-8610-f5cbcd09cd48.PNG">
<img width="385" src="https://user-images.githubusercontent.com/112605121/188874870-92298802-ccd4-4256-913e-b485f406c6e9.PNG">
