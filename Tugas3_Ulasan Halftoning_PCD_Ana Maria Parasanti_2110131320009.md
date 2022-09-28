**Ana Maria Parasanti - 2110131320009**

---

## Halftone

  Halftone adalah sebuah teknik reprografi yang mensimulasikan citra ton berkelanjutan melalui titik-titik bervariasi, baik dalam ukuran, dalam bentuk 
  ataupun dalam jarak. Halftone juga dapat digunakan untuk merujuk secara khusus gambar akan yang dihasilkan.

  Digital halftoning adalah suatu proses untuk mengkonversi citra yang kontinu ke dalam suatu array berupa titik-titik. Jika dilihat oleh sistem visual 
  manusia, pola tersebut akan  menciptakan  suatu  ilusi  sehingga  citra  tersebut  tampak  bukan  seperti  citra  hitam putih, namun seperti citra 
  abu-abu yang kontinu.

  Metode  yang  paling  sederhana  untuk  mengkonversi  citra  abu-abu  menjadi  citra biner  adalah  dengan  menggunakan  ambang  batas,  yaitu  dengan  dua  tingkat  (satu bit) kuantisasi.  Misalkan  f(i,j)  adalah  sebuah  citra abu-abu,  dan  b(i,j)  adalah  citra  yang dihasilkan dari metode ambang 
  batas yang sederhana. Untuk ambang batas T, citra biner dihitung dengan sebagai berikut:

  <p align="center">
  <img width="134" alt="pcd3 4" src="https://user-images.githubusercontent.com/112605121/192793935-4bcd446e-2cb1-4086-b1f1-1bdb5b404228.PNG"></p>
  
  <p align="center">
  <i>Ambang batas T</i></p>

  Gambar 1 adalah gambar asli, yaitu gambar “lena.jpg” dengan resolusi 256 x 256. Sedangkan, Gambar 2 menggambarkan   hasil   konversi   ke   citra   biner   dengan   ambang   batas menggunakan T = 127.

  <p align="center">
  <img width="143" alt="pcd3 5" src="https://user-images.githubusercontent.com/112605121/192794002-37f7ef90-3d11-4f90-b4d0-5b3f70eee035.PNG"></p>

  <p align="center">
  <i>Gambar 1. Citra asli "lena.jpg" dengan resolusi 256x256</i></p>

  <p align="center">
  <img width="131" alt="pcd3 6" src="https://user-images.githubusercontent.com/112605121/192794078-86b94928-9ff7-4b5d-9997-9fa32ba4df33.PNG"></p>

  <p align="center">
  <i>Gambar 2. Citra biner "Lena.jpg" dihasilkan dari ambang batas tetap yang sederhana</i></p>

  Gambar  1  dan Gambar  2  menunjukkan  bahwa  citra  biner  tidak  “berbayang” dengan benar. Beberapa artefak  di  dalam citra tampak sebagai contouring palsu. Hal ini sering terjadi jika kuantisasi dilakukan pada bit terendah (dalam hal ini adalah satu bit), sehingga terjadi kesalahan kuantisas.

  Dimana citra ton warna berkelanjutan berisi warna tak terbatas atau disebut dengan abu-abu, proses halftone mengurangi reproduksi visual untuk gambar biner yang dicetak dengan hanya satu warna tinta (biner adalah sistem penulisan yang hanya menggunakan dua simbol yaitu (0 dan 1). Reproduksi biner ini tergantung pada ilusi optis dasar bahwa titik-titik kecil halftone ini dicampur kedalam nada halus dengan mata manusia. Pada tingkat mikroskopis, dikembangkan film fotografi hitam-putih yang juga terdiri dari hanya dua warna, dan bukan jangkauan ton yang berlanjut tak terbatas.

  Sama seperti fotografi berwarna  berkembang dengan penambahan filter dan lapisan film, pencetakan ini dimungkinkan dengan mengulangi proses halftone untuk setiap warna subtraktif yang paling umun menggunakan ini ialah dalam metode pencetakan CMYK. Properti semi-optik tinta ini memungkinkan halftone dengan titik-titik warna yang berbeda untuk menciptakan efek citra lain yang penuh warna optik.

  Tiga contoh warna penghalftonan dengan menggunakan sistem CMYK. Dari kiri ke kanan. Pemisahan cyan, pemisahan magenta, pemisahan yellow, dan pemisahan warna hitam. Pola halftone gabungan dan akhirnya bagaimana cara mata manusia melihat pola halftone gabungan dari jarak yang cukup(paling kanan).

  Meskipun titik bulat yang paling sering digunakan, ada jenis titik lain yang tersedia, masing-masing dari mereka memiliki karakteristik yang brebeda. Dan mereka juga dapat digunakan secara bersamaan untuk menghindari efek moire. Umumnya bentuk dot(bulat) paling disukai termasuk didalam dunia sablon atau percetakan, namun tergantuk dari alat cetaknya juga.

  + Ada 3 type titik :

      + Titik putaran : ini yang paling umum, cocok untuk gambar yang memfokuskan gambar-gambar cahaya, terutama untuk warna kulit. Mereka bertemu di nilai nada dari 70%.

      + Titik elipse : ini sesuai untuk gambar dengan banyak objek. Titik elipse bertemu di nilai 40% (berakhir menunjuk) dan 60% (sisi panjang), sehingga ada risiko pola.

      + Titik persegi : terbaik untuk gambar rinci, tidak dianjurkan untuk warna kulit. Sudut ini bertemu di nilai tonal 50%. Transisi antara titik persegi terkadang dapat terlihat dengan mata manusia.

  Halftoning bertujuan  untuk  memberikan  kesan  warna  citra biner tampak seperti citra abu-abu meskipun hanya menggunakan piksel warna hitam dan putih saja. Meskipun teknik ambang batas (thresholding) yang sederhana ini dapat mengkonversi citra abu-abu menjadi  citra  biner, namun kualitas  citra  yang  dihasilkan  masih  kurang  baik.

## Metode Halftone

+ **Patterning**

    Patterning adalah yang paling sederhana dari tiga teknik untuk menghasilkan gambar halftoning digital. Patterning dilakukan dengan mengganti setiap piksel dengan pola yang diambil dari 'font biner'.
    
    Ini menghasilkan gambar yang memiliki resolusi spasial lebih tinggi daripada gambar sumber. Jumlah sel halftone citra keluaran sama dengan jumlah piksel citra sumber. Namun, setiap sel halftone dibagi lagi menjadi kotak 4x4. Setiap nilai piksel input diwakili oleh jumlah kotak terisi yang berbeda dalam sel halftone. Karena kisi 4x4 hanya dapat mewakili 17 tingkat intensitas yang berbeda, gambar sumber harus dikuantisasi. Gambar kedua menunjukkan matriks pola rekursif Rylander, yang akan digunakan dalam daftar pertama, dan contoh operasi Patterning.
    
    
    <p align="center">
    <img width="151" alt="pcd3 6" src="https://user-images.githubusercontent.com/112605121/192797720-4208ed81-5db0-4099-9a8a-966b9176f000.jpg"></p>

    <p align="center"><i>
    Matriks pattern rekursif Rylander</i></p>

    <p align="center">
    <img width="200" alt="pcd3 6" src="https://user-images.githubusercontent.com/112605121/192797779-b1acee21-2a6f-41f2-8a0d-018d54d3fd45.jpg"></p>

    <p align="center"><i>Operasi Patterning</i></p>
    
    Konsep pattering:
    
    - Akan ada ambang batas yang dikenakan pada abu-abu nilai level dari gambar asli.
      
    - Jika ambang batas berada dalam kisaran font pertama maka pola font pertama akan diganti untuk piksel.
      
    - Proses berlanjut untuk semua piksel dalam gambar dan diganti dengan font yang sesuai pola.
      
    - Perhatikan bahwa, karena kita mengganti setiap piksel dengan 3x3 blok piksel, baik lebar maupun tinggi bayangan bertambah tiga kali lipat.
    
    Algoritma untuk halftone gambar menggunakan patterning:
    
    <img width="386" alt="pcd3 13" src="https://user-images.githubusercontent.com/112605121/192812898-ec70b68d-ea9c-4b79-8185-67270c1457c7.PNG">

+ **Dithering**

    Teknik lain untuk halftoning digital adalah dithering. Dithering dapat dilakukan dengan ambang batas gambar terhadap matriks dither. Unsur-unsur matriks gentar adalah ambang batas.
    Proses dithering ini tidak akan merubah ukuran, namun hanya merubah pada detail saja.
    
    Karena  sistem  visual  manusia  cenderung  meratakan  suatu area di  sekitar  piksel, bukan   melihat   setiap   piksel   secara   sendiri-sendiri,   sehingga   memungkinkan   untuk membuat  ilusi  dari  beberapa  tingkat  keabuan  di  dalam  sebuah  citra  biner  yang  dalam kenyataanya  hanya  terdiri  dari  dua  tingkat  abu-abu. Dengan  menggunakan  matriks  2x2 piksel,  lima  nilai  intensitas  “efektif”  yang  berbeda  dapat  terwakili,  seperti   yang diilustrasikan  pada Gambar 3.  Demikian  juga  dengan  matriks  4x4  piksel,  sepuluh  buah tingkat kabuan yang berbeda dapat terwakili. Metode ini disebut dengan dithering, dalam proses dithering blok  asli  pada  citra  kemudian  akan  diganti  dengan  jenis  pola  biner tersebut.

    <p align="center">
    <img width="250" alt="pcd3 7" src="https://user-images.githubusercontent.com/112605121/192798141-1df0a2f4-98d7-402a-8651-2047699f0a00.PNG"></p>

    <p align="center"><i>
    Gambar 3. Lima pola berbeda dari matriks biner 2x2 piksel</i></p>

    Proses dithering:
    
    Ordered dithering dilakukan  dengan  membandingkan  tiap  blok  dari  citra  asli dengan sebuah matriks  pembatas  yang  disebut  dengan matriks dither. Masing-masing elemen  dari  blok  asli  dikuantisasi  sesuai  dengan  nilai  batas  pada  pola dither.  Nilai-nilai pada matriks dither adalah tetap, tetapi bisa bervariasi sesuai dengan jenis citra.

    Matriks dither pertama yang digunakan dalam metode ini adalah:

    <img width="230" alt="pcd3 8" src="https://user-images.githubusercontent.com/112605121/192798182-7def1ae3-8433-457c-bb7f-90c65b3e0f35.PNG">

    Matriks  tersebut  diulang  sampai  mencakup  seluruh  matriks  pada  citra  yang  diolah. Katakanlah  d(i,j)  adalah  matriks  yang  diperoleh  dari  mereplika  A  dan  x(i,j)  adalah  citra abu-abu asli. Piksel untuk citra yang dihasilkan p(i,j) didefenisikan sebagai berikut:

    <img width="364" alt="pcd3 9" src="https://user-images.githubusercontent.com/112605121/192798223-75ec6f77-c1a8-4a91-b1d3-400109389f4e.PNG">

    Hasil  konversi  citra  abu-abu  pada Gambar  1  menggunakan  metode ordered dithering menggunakan matriks dither2 x 2, ditunjukkan pada Gambar 4.

    <p align="center">
    <img width="123" alt="pcd3 10" src="https://user-images.githubusercontent.com/112605121/192798270-02278610-5d62-4b7a-8176-b52ea985270c.PNG"></p>

    <p align="center"><i>
    Gambar 4. Citra menggunakan matriks dithering 2x2</i></p>

    Selain matriks 2x2, teknik ini juga memiliki matriks dithering yang lainnya, yaitu 4x4 sebagai berikut

    <p align="center">
    <img width="260" alt="pcd3 11" src="https://user-images.githubusercontent.com/112605121/192798316-6ddd75de-ca78-4e39-ba75-caed443e1038.PNG"></p>

    <p align="center"><i>
    Gambar 5. menunjukkan citra yang dihasilkan dari penggunaan ordered dithering matriks 4x4.</i></p>

    <p align="center">
    <img width="127" alt="pcd3 12" src="https://user-images.githubusercontent.com/112605121/192798371-852948ba-4198-4dc5-9ef4-f15bf2e47f88.PNG"></p>

    <p align="center"><i>Gambar 6. Citra menggunakan matriks dithering 4x4</i></p>
    
    Algoritma untuk halftone gambar menggunakan matriks dithering:
    
    ![n59QFk5](https://user-images.githubusercontent.com/112605121/192807437-40d8cf65-ebca-48a4-8b84-e69dff6d6fe4.png)
 
---
