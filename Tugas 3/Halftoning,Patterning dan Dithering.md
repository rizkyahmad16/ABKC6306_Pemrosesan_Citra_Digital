## __Tugas 3__ : mengimplementasikan method grayscale lightness method, average method, dan Luminousity method serta menjelaskan tentang halftoning patterning, dithering, bagaimana menentukan pola patterning, dan menentukan tresholding dithering

Soure code:

![gambar](/Tugas%203/gambar/1.jpeg)

> Mencoba 3 Rumus :
1. Lightness Method

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Lightness Method rumusnya adalah minimal RGB ditambah dengan maximum RGB lalu dibagia dua, dengan hasil gambar output seperti dibawah. Untuk kejelasan gambar hampir beda dengan yang aslinya dikarnakan metode ini menghadirkan kelemahan yang sangat serius karena satu komponen RGB tidak digunakan. Ini jelas merupakan masalah karena jumlah cahaya yang dilihat mata kita bergantung pada ketiga warna dasar.

![gambar](/Tugas%203/gambar/2.jpeg)

2. Avarage Method

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Avarage Method dengan rumus warna R+G+B lalu dibagi tiga, Hasilnya seperti gambar dibawah untuk tingkat keabuanya dapat membuat mata sakit dikarnakankita memperhitungkan semua komponen, metode rata-rata juga bermasalah karena memberikan bobot yang sama untuk setiap komponen. Berdasarkan penelitian tentang penglihatan manusia, kita tahu bahwa mata kita bereaksi terhadap setiap warna dengan cara yang berbeda. Secara khusus, mata kita lebih sensitif terhadap hijau, lalu merah, dan akhirnya biru. Oleh karena itu, bobot dalam persamaan di atas harus berubah.

![gambar](/Tugas%203/gambar/3.jpeg)

3. Luminosity

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Metode ini adalah yang terbaik dari dua diatas. Berdasarkan pengamatan di atas, kita harus mengambil rata-rata tertimbang dari komponen. Kontribusi warna biru pada nilai akhir harus berkurang, dan kontribusi warna hijau harus meningkat. Jadi warna keabuan di metode ini sangat jelas dan tepat serta enak dilihat oleh mata.

![gambar](/Tugas%203/gambar/4.jpeg)