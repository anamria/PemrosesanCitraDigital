**Ana Maria Parasanti - 2110131320009**

---

## Cara menentukan pola pada patterning

Jumlah intensitas yang dapat ditampilkan tergantung dari

  + Jumlah pixel yang menyusun tiap grid.

  + Jumlah level intensitas yang didukung oleh perangkat.

Rumus jumlah intensitas:

        N^2+1

Contoh 2x2 pixel dengan 5 level intensitas:

<img width="230" src="https://user-images.githubusercontent.com/112605121/194598373-56118632-0b44-4cd5-971b-26e0c7c88ed1.PNG">

Contoh 3x3 pixel dengan 10 level intensitas:

<img width="229" src="https://user-images.githubusercontent.com/112605121/194598402-36b2ac1f-961b-4834-8aa3-61a049a8eea6.PNG">

Untuk menentukan polanya, terdapat beberapa poin penting, yaitu

  + Meminimalisir efek konturing (level k + 1) dengan sebisa mungkin memulai pattern dari posisi tengah.

  + Meminimalisir efek visual lain yang tidak ada di citra asli dengan menghindari pola simetris. Pola simetris akan menyulitkan dalam menghasilkan gradasi warna.

    Contoh:

    <img width="230" src="https://user-images.githubusercontent.com/112605121/194598437-fc9dbf7f-1d54-4dd3-93f3-47c7ab4317db.PNG">

## Cara menentukan matriks threshold pada dithering

Thresholding digunakan untuk mengatur jumlah derajat keabuan yang ada pada citra. Dengan   menggunakan thresholding maka derajat keabuan bisa diubah sesuai keinginan, misalkan diinginkan menggunakan derajat keabuan 16, maka tinggal membagi nilai derajat keabuan dengan 16. Proses thresholding ini pada dasarnya adalah proses pengubahan kuantisasi pada citra, sehingga untuk melakukan thresholding dengan derajat keabuan dapat digunakan rumus:

<img width="150" src="https://user-images.githubusercontent.com/112605121/194598216-5c752c3a-089a-49ce-a5b1-b5262b5a18ad.PNG">

dimana :

  + w adalah nilai derajat keabuan sebelum thresholding 
    
  + b adalah jumlah derajat keabuan yang diinginkan 
    
  + x adalah nilai derajat keabuan setelah thresholding

## Mengapa hasil dithering pada matriks dither yang lebih sedikit tidak sebagus dengan yang menggunakan matriks dither yang lebih besar?

Karena hasil dithering yang menggunakan matriks dither dengan ordo lebih besar dapat memuat lebih banyak pola halftone, sehingga hasil output dari pemrosesan tersebut lebih bagus ketimbang menggunakan matriks dither dengan ordo sedikit.

Berikut contoh perbedaan antara hasil dithering dengan matriks dither 2x2 dan 4x4:

  + Hasil dithering dengan matriks dither 2x2

  <img width="230" src="https://user-images.githubusercontent.com/112605121/194598604-00780e5e-ab69-4891-a6dc-8fe417419317.PNG">

  + Hasil dithering dengan matriks dither 4x4
  
  <img width="230" src="https://user-images.githubusercontent.com/112605121/194598631-3e395319-d890-4a41-81a2-1d71df3e50b4.PNG">

Jika kita lihat, terdapat perbedaan dari hasil dithering pada gambar diatas. Hal ini disebabkan oleh sensitifitas nilai piksel gambar asli. Citra yang dihasilkan oleh matriks dither 2x2 memiliki pola halftone yang kurang dibandingkan dengan citra yang menggunakan matriks dither 4x4. Sehingga hasil dari citra digital dengan menggunakan matriks dither 2x2 memiliki banyak daerah dengan pola halftone yang sama, seperti pada daerah latar belakang, rambut, dan hidung, walaupun pada daerah tersebut mengandung lebih banyak nilai piksel.
