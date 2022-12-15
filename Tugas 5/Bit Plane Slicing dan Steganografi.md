## __Tugas 5 :__ Memasukkan nama dan nim / gambar 1 dan gambar 2 kedalam LSB Gambar atau lapisan layar yang paling tidak menyerupai (Stegonography)

## __Bit Plane Slicing dan Steganografi__

### __Bit Plane Slicing__

Bit-Plane Slicing merupakan metode yang digunakan untuk melihat kontribusi atau pengaruh dati tiap bit penyusun citra. Untuk citra 8 bit, pada dasarnya tiap intensitas yang nilainya dalam format desimal, bisa dipecah menjadi bit-bit dalam format biner.

Misalnya, sebuah piksel dengan intesnsitas 245(desimal) bila dijadikan biner adalah 11110101. Dengan nilai LSB (Least Significant Bit) berada paling bawah kanan, dan sebaliknya untuk MSB (Most Sigificant Bit). Perhatikan gambar dibawah yang merupakan ilustrasi dari bit-plane sicing pada piksel citra.

![gambar](/Tugas%205/gambar/1.png)

Untuk memahami metode ini, perhatikan contoh berikut !

Misalkan diberikan citra grayscale berukuran 3x3 dengan nilai matriks sebagai berikut :

![gambar](/Tugas%205/gambar/2.%20matriks.png)

Ubah nilai pada tiap elemen matriks di atas menjadi bilangan biner 8 digit

![gambar](/Tugas%205/gambar/3.%20mbiner.png)

Nah yang akan kita lakukan sekarang adalah secara berurutan mengambil bit-bit untuktuap-tiap intensitas dan dimasukkan kedalam matriks baru. Sehingga dapat ditebak bahwa kita akan mendapatkan 8 buah matriks baru yang berisi bit-bit dari urutan yang sama.

![gambar](/Tugas%205/gambar/4.%20bit-plane.png)

1. Mengubah Gambar ukuran 512 x 512 ke grayscale dan buat bit-plane slicing

![gambar](/Tugas%205/gambar/5.%20house.jpg)

Gambar Asli

![gambar](/Tugas%205/gambar/6.%20code_bit-plane2.png)

Code Bit Plane Slicing

![gambar](/Tugas%205/gambar/7.%20bit-plane2.png)

Bit Plane Slicing

Dapat dilihat pada output gambar, semakin tinggi layer bit-plane slicing maka akan semakin tinggi pula kualitas tampilan gambarnya, dapat dilihat setiap berbedaannya pada gambar di atas. Pada gambar di atas bit-plane slicing pada layer 8 mempunyai tampilan gambar kualitas lebih tinggi dari pada layer di bawahnya.

2. Gabung Dua Gambar Ubah ke Grayscale dan Buat Bit-Plane Slicing, Bandingkan Dengan Bit-Plane 1

![gambar](/Tugas%205/gambar/8.%20show_gambar.png)

![gambar](/Tugas%205/gambar/9.%20show_gambar3.png)

Hasil Penggabungan Gambar 1 dengan gambar 2

![gambar](/Tugas%205/gambar/10.%20code_bit-plane3.png)

Code Bit Plane Slicing

![gambar](/Tugas%205/gambar/11.%20bit_plane_gabung.png)

Hasil Penggabungan Gambar 1 dan gambar 2

Dapat dilihat bahwa penggabungan 2 gambar kan mengasilkan gambar yang lebih terang (warna dominan ke putih). Untuk proses bit-plane slicing dari penggabungan 2 gambar ini sama saja dengan soal 1, namun yang berbeda disini adalah tampilan bit-plane slicing yang lebih menonjol pada warna putih sehingga pada bit plane layer 8 gambar hampir tidak terlihat. Dapat disimpulkan semakin tinggi bit plane maka semakin tinggi juga tingkat kecerahan atau kualitas gambar.

### __Steganografi__

Steganografi adalah sebuah metode dalam pemrosesan citra digital untuk menyembunyikan suatu data rahasia ke dalam sebuah citra.

Data yang disembunyikan dapat berupa:

![gambar](/Tugas%205/gambar/12.%20cover_stego.png)
 - Gambar

 - Teks

 - Suara

 - Dll


 Langkah- Langkah Steganografi Adapun langkah-langkah yang dilakukan dalam menerapkan metode steganografi adalah:

 - Ubah citra warna ke dalam citra grayscale.

 - Ubah pesan yang akan disisipkan ke dalam bentuk biner.

 - Cek untuk setiap piksel yang ada pada citra, dan lakukan:

 - Ambil nilai LSB pada citra.

 - Ambil nilai bit pesan yang akan disisipkan.

 - Jika nilai sama, tambahkan 0 ke dalam citra output, jika tidak tambahkan 1.

 - Simpan gambar.

 Membuat Steganografi yang Berisikan Pesan Rahasia Berupa Nama dan Nim

 ![gambar](/Tugas%205/gambar/Gambar%20Stegonografi%201.png)

 ![gambar](/Tugas%205/gambar/Gambar%20Stegonografi%202.png)

 output

 ![gambar](/Tugas%205/gambar/show_stego%20hasil.png)

 Dapat dilihat bahwa pada gambar 1 dan gambar 2 tidak terdapat perbedaan, padahal pada gambar 2 memuat pesan rahasia berupa text di dalam gambar tersebut.