**Ana Maria Parasanti - 2110131320009**

---

### Pertanyaan

1. Jelaskan ada berapa layer pada gambar berwarna! screenshot hasil ekplorasi layer pada aplikasi octave.

2. Gunakan fungsi (1) imread, (2) imshow (3) dan imhist. jelaskan fungsi2 tersebut disertakan screenshot.

### Jawaban

1. Pada gambar berwarna terdiri dari tiga layer yaitu layer Merah (Red), Hijau (Green), Biru (Blue) atau biasa disebut dengan RGB. 
   Red (Merah), Green (Hijau) dan Blue (Biru) merupakan warna dasar yang dapat diterima oleh mata manusia. Setiap piksel pada citra 
   warna mewakili warna yang merupakan kombinasi dari ketiga warna dasar RGB. Setiap titik pada citra warna membutuhkan data sebesar 
   3 byte. Setiap warna dasar memiliki intensitas tersendiri dengan nilai minimum nol (0) dan nilai maksimum 255 (8 bit). RGB didasarkan 
   pada teori bahwa mata manusia peka terhadap panjang gelombang 630nm (merah), 530 nm (hijau), dan 450 nm (biru).
   
   Pada channel merah, warna merah sempurna direpresentasikan dengan nilai 255 dan hitam sempurna dengan nilai 0. Pada channel hijau, warna 
   hijau sempurna direpresentasikan dengan nilai 255 dan hitam sempurna dengan nilai 0. Begitu juga pada channel biru, warna biru 
   sempurna direpresentasikan dengan nilai 255 dan hitam sempurna dengan nilai 0.

    Berikut eksplorasi pada gambar berwarna dengan ukuran 32x32.

    + Gambar asli
      
      Sintaks kode:
      
      <img width="346" src="https://user-images.githubusercontent.com/112605121/191336530-5cc3b1b7-4403-419a-82f3-fd66f2f525b1.PNG">
      
      Hasil keluaran:
      
      <img width="860" src="https://user-images.githubusercontent.com/112605121/191332998-727607e9-44aa-4777-9930-fa77d885e621.PNG">
    
    + Channel merah

      Sintaks kode:
      
      <img width="316" src="https://user-images.githubusercontent.com/112605121/191336610-a75a3b9f-3103-46aa-a48d-6271019d3282.PNG">
      
      Hasil keluaran:
      
      <img width="863" src="https://user-images.githubusercontent.com/112605121/191333185-c669dbc9-56b3-4f6f-afd8-118a613295c4.PNG">

    + Channel hijau
      
      Sintaks kode:
      
      <img width="328" src="https://user-images.githubusercontent.com/112605121/191336731-c33a305a-f322-4149-8839-f1ba1a823514.PNG">
      
      Hasil keluaran:

      <img width="864" src="https://user-images.githubusercontent.com/112605121/191333229-b4b8d6a6-ae77-4649-aeba-ca72cd7734ae.PNG">

    + Channel Biru

      Sintaks kode:
      
      <img width="319" src="https://user-images.githubusercontent.com/112605121/191336826-7aaf7e89-bd77-4c3c-b569-43d89561ea57.PNG">
      
      Hasil keluaran:

      <img width="960" src="https://user-images.githubusercontent.com/112605121/191338658-f0e650f8-2cc0-40f5-a483-a2ce5406d6ad.PNG">

2. - Fungsi imread

        <img width="500" src="https://user-images.githubusercontent.com/112605121/191334220-9ebbeaee-ecb1-45af-a061-93a91f5e2997.PNG">

        fungsi ini digunakan untuk membaca file image yang disimpan. Pada contoh diatas dituliskan,
        
                    gambar = imread("gambarPCD.png"); 
        
        artinya, octave akan membaca file gambar bernama gambarPCD dengan ekstensi PNG yang disimpan ke dalam variabel gambar.

    - Fungsi imshow
        
        <img width="500" src="https://user-images.githubusercontent.com/112605121/191334273-28c3bf9a-8836-49c9-9e89-d845271d707d.PNG">

        fungsi ini digunakan untuk menampilkan objek gambar. Pada contoh diatas dituliskan,
        
                    imshow(gambar);
        
        artinya, octave akan menampilkan file gambar yang tersimpan pada variabel gambar.

    - Fungsi imhist
        
        <img width="500" src="https://user-images.githubusercontent.com/112605121/191334342-26142cb2-1ca8-41bb-8b63-71e7770ceb1f.PNG">

        Fungsi ini digunakan untuk menampilkan image dengan bentuk histogram. Pada contoh diatas dituliskan,
        
                    imhist(Blue);
        
        artinya, octave akan menampilkan image dengan bentuk histogram pada variabel blue.
---
