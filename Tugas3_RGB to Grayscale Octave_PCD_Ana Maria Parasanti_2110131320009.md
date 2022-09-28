**Ana Maria Parasanti - 2110131320009**

---

## Pengaplikasian Rumus RGB ke Grayscale Menggunakan Octave

1. Lightness Method

    Rumus: 

        grayscale = (min(R*G*B)+max(R*G*B))/2

    Sintaks Kode: 

    <img width="433" alt="pcd3 1" src="https://user-images.githubusercontent.com/112605121/192739401-239a919e-76fa-42bc-b3e4-496ceb3fb1cb.PNG">

    Penjelasan:

    + Pada variabel gambar menggunakan fungsi imread, untuk membaca file image yang disimpan yaitu gambarPCD.png.
    + Pada variabel R, akan menyeleksi layer berwarna merah. Pada variabel G, akan menyeleksi layer berwarna hijau. Serta pada variabel B, akan 
      menyeleksi layer berwarna biru.
    + Pada variabel Gray, disimpan rumus untuk mengubah warna gambar yang awalnya berwarna menjadi skala keabu-abuan menggunakan metode *Lightness*.
    + Pada subplot(1,2,1), akan ditampilkan gambar ke dalam satu figure yaitu sebelah kiri. Sedangkan Pada subplot(1,2,2), akan ditampilkan gambar 
      ke dalam satu figure yaitu sebelah kanan.
    + Pada fungsi imshow(Gray), akan ditampilkan objek gambar tersebut. 
    + Pada fungsi imhist(Gray), akan ditampilkan gambar tersebut dengan bentuk histogram.
    + Pada title, digunakan untuk memberikan judul pada figure saat ditampikan.

    Hasil Output:

    ![Screenshot (642)](https://user-images.githubusercontent.com/112605121/192742222-1ef6c9bf-59e3-4f54-a294-809d3dca532c.png)

2. Average Method
    
    Rumus:
    
        grayscale = (R+G+B)/3
    
    atau 
    
        grayscale = (0,33*R)+(0,33*G)+(0,33*B)
    
    Sintaks Kode:
    
    <img width="479" alt="pcd3 2" src="https://user-images.githubusercontent.com/112605121/192744231-250ba127-2e88-40b4-bfa2-00258a55c125.PNG">

    Penjelasan:

    + Pada variabel gambar menggunakan fungsi imread, untuk membaca file image yang disimpan yaitu gambarPCD.png.
    + Pada variabel R, akan menyeleksi layer berwarna merah. Pada variabel G, akan menyeleksi layer berwarna hijau. Serta pada variabel B, akan 
      menyeleksi layer berwarna biru.
    + Pada variabel Gray, disimpan rumus untuk mengubah warna gambar yang awalnya berwarna menjadi skala keabu-abuan menggunakan metode *Average*.
    + Pada subplot(1,2,1), akan ditampilkan gambar ke dalam satu figure yaitu sebelah kiri. Sedangkan Pada subplot(1,2,2), akan ditampilkan gambar 
      ke dalam satu figure yaitu sebelah kanan.
    + Pada fungsi imshow(Gray), akan ditampilkan objek gambar tersebut. 
    + Pada fungsi imhist(Gray), akan ditampilkan gambar tersebut dengan bentuk histogram.
    + Pada title, digunakan untuk memberikan judul pada figure saat ditampikan.

    Hasil Output:
    
    ![Screenshot (688)](https://user-images.githubusercontent.com/112605121/192744586-d55bff33-b0a8-4f8a-aa76-5cdaeb0c36a4.png)

3. Luminosity Method
    
    Rumus:
    
        (0,3*R)+(0,59*G)+(0,11*B)
    
    Sintaks Kode:
    
    <img width="427" alt="pcd3 3" src="https://user-images.githubusercontent.com/112605121/192745937-22080233-82e9-40be-a3ae-c25365dcf961.PNG">
    
    Penjelasan:

    + Pada variabel gambar menggunakan fungsi imread, untuk membaca file image yang disimpan yaitu gambarPCD.png.
    + Pada variabel R, akan menyeleksi layer berwarna merah. Pada variabel G, akan menyeleksi layer berwarna hijau. Serta pada variabel B, akan 
      menyeleksi layer berwarna biru.
    + Pada variabel Gray, disimpan rumus untuk mengubah warna gambar yang awalnya berwarna menjadi skala keabu-abuan menggunakan metode *Luminosity*.
    + Pada subplot(1,2,1), akan ditampilkan gambar ke dalam satu figure yaitu sebelah kiri. Sedangkan Pada subplot(1,2,2), akan ditampilkan gambar 
      ke dalam satu figure yaitu sebelah kanan.
    + Pada fungsi imshow(Gray), akan ditampilkan objek gambar tersebut. 
    + Pada fungsi imhist(Gray), akan ditampilkan gambar tersebut dengan bentuk histogram.
    + Pada title, digunakan untuk memberikan judul pada figure saat ditampikan.
    
    Hasil Output:
    
    ![Screenshot (653)](https://user-images.githubusercontent.com/112605121/192746112-35c74a68-a4df-4942-80e8-d9cf7d5a8f4e.png)

---
