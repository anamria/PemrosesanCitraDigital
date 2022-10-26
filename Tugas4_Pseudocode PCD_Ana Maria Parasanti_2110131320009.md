**Ana Maria Parasanti - 2110131320009**

---

## Pseudocode Pemrosesan Citra Digital

### Patterning

1. Tentukan banyak pola patterning untuk level tingkat keabuan yang akan digunakan.
2. Hitung persebaran range nilai sebanyak dengan jumlah pola patterning yang telah ditentukan.
3. Bandingkan nilai element matriks gambar asli dengan nilai pada range pola patterning.

### Dithering

1. Bandingkan elemen matriks dari citra gambar asli (A) dengan elemen matriks threshold/ambang batas/ditthering (B)
2. Jika elemen matriks A lebih besar dari pada elemen di matriks threshold B, maka akan diubah menjadi putih atau 255.
3. Jika sebaliknya, maka akan diubah menjadi hitam atau 0.

### Histogram Equalization

1. Temukan jumlah berjalan dari nilai histogram
2. Normalisasikan nilai dari langkah (i) dengan membagi dengan jumlah total piksel
3. Kalikan nilai dari langkah (ii) dengan nilai tingkat keabuan maksimum dan bulat
4. Petakan nilai tingkat keabuan ke hasil dari langkah (iii) menggunakan korespondensi satu-ke-satu

### Bit Plane Slicing 

1. Asumsikan piksel dengan representasi nilai matriks S seperti berikut: [229,12,12,12]
2. Ubah nilai intensitas matriks A ke dalam bentuk biner. Misalnya untuk 299 diubah ke dalam biner menjadi 11100101. Jadi dalam 1 piksel gambar terdiri dari 8 bit biner.
3. Untuk citra bit-plane yang mengandung bit terendah (LSB) dari keseluruhan nilai yang ada di dalam piksel terdapat di bagian ujung tiap nilai.
4. Untuk citra bit-plane yang mengandung bit tertinggi (MSB) dari keseluruhan nilai yang ada di dalam piksel terdapat di bagian depan tiap nilai.

---
