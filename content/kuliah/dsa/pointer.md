+++
title = 'Pointer'
date = 2025-07-03T06:15:58+08:00
draft = false
+++

Dalam dunia programming kita mengenal yang namanya pointer. Pointer adalah variabel yang menyimpan alamat memori dari variable lain sebagai nilainya. Pointer memiliki dua jenis operator. Yaitu deference operator dan reference operator.

Contoh Program 1:

Deference operator digunakan untuk mendapatkan alamat memori dari suatu variabel. Deference operator dibuat dengan menambahkan simbol (&) di depan nama variabel. Silahkan lihat contoh program di bawah.

![Program 1](/img/dsa/pointer-contoh-program-1.png)
Output Program 1:
![Ouput Program 1](/img/dsa/pointer-output-program-1.png)

Pada baris ke-10, terdapat tanda reference operator (&) didepan variabel angka dan outputnya akan menjadi alamat memori (bilangan hexadesimal). Berbeda halnya ketika mencetak variabel angka pada baris ke-11, maka yang akan ditampilkan adalah isi dari variabel angka itu sendir yaitu 20.

Contoh Program 2
![Program 2](/img/dsa/pointer-contoh-program-2.png)

Reference operator (*) dalam Bahasa Pemrograman c++ memiliki dua fungsi yaitu. Pertama adalah menyatakan suatu variabel sebagai variabel pointer. Kedua untuk mengakses nilai dari alamat memori yang disimpan pada variabel pointer. Perhatikan contoh program dibawah.

Ouput Program 2
![Output Program 2](/img/dsa/pointer-output-program-2.png)

Pada baris ke-12 dan ke-13 akan mencetak masing-masing nilai dan alamat memori dari variabel a. Output baris ke-14 dan ke-15 adalah nilai dan alamat memori dari variabel b. Perhatikan alamat variabel a sama dengan nilai dari variabel b. Itu berarti variabel b menyimpan alamat memori  variabel a. Namun variabel a dan b terletak pada alamat yang berbeda. Perhatiakan ilustrasi di bawah.

![Ilustrasi 1](/img/dsa/pointer-ilustrasi-1.png)
Lalu pada baris ke-16, program akan mengakses nilai dari alamat memori yang tersimpan pada variabel b. Alamat memori tersebut adalah alamat dari variabel a, jadi nilai yang diakses adalah nilai dari variabel a , yaitu 5.

Contoh Program 3
Sebuat variabel pointer didefinisikan dengan format sebagai berikut.

tipe_data *nama_var;

Ketika mengubah nilai pada suatu variabel, seluruh variabel yang memiliki pointer ke variabel tersebut nilai referencenya juga akan ikut berubah. Hal tersebut karena sebenarnya reference operator akan selalu mengambil nilai berdasarkan alamat memori. Perhatikan contoh dibawah.

![Program 3](/img/dsa/pointer-contoh-program-3.png)

Output:

![Output Program 3](/img/dsa/pointer-output-program-3.png)

Pada contoh program di atas, variabel x berisi angka 10 lalu nilai variabel x dicopy ke variabel y. Lalu selanjutnya variabel px akan diisi dengan alamat memori x. Meskipun nilai x dan y sama, namun kedua nilai tersebut disimpan di alamat memory yang berbeda. Perhatikan ilustrasi yang saya buat dibawah.

![Ilustrasi 2](/img/dsa/pointer-ilustrasi-2.png)

Lanjutan contoh program 3
![Program 4](/img/dsa/pointer-contoh-program-4.png)

Output:
![Output Program 4](/img/dsa/pointer-output-program-4.png)

Pada kode ini, x diisi kembali dengan angka 20. Hasilnya terlihat bahwa hanya variabel x yang nilainya berubah, sedangkan y tetap bernilai 10. Itu karena sebelumnya x dan y adalah dua variabel yang berbeda dan y bukanlah pointer ke variabel x. Jadi meskipun x diubah, y tetap menyimpan nilai 10. Perhatikan yang saya buat.
![Ilustrasi 3](/img/dsa/pointer-ilustrasi-3.png)


Lanjutan Program 3
![Program 5](/img/dsa/pointer-contoh-program-5.png)
Output:
![Output Program 5](/img/dsa/pointer-output-program-5.png)

Di sini, nilai dari alamat memori yang tersimpan pada pointer *px diubah menjadi 30. Terlihat bahwa nilai variabel x juga menjadi 30. Itu karena px menyimpan alamat memori dari variabel x jadi otomatis nilai variabel x yang sebenarnyar terubah.

Untuk lebih memahami alur dari contoh program 3, lihat ilustrasi yang telah saya siapkan.
![Ilustrasi 4](/img/dsa/pointer-ilustrasi-4.png)
![Ilustrasi 5](/img/dsa/pointer-ilustrasi-5.png)


Contoh Program 4
Selain menunjuk alamat suatu variabel, pointer dapat juga digunakan untuk menuntuk alamat dari pointer lain atau pointer di dalam pointer. Untuk membuat pointer di dalam pointer, cukup tambahkan lagi reference operator (*) di depan variabel pointer seperti contoh di bawah.
![Program 6](/img/dsa/pointer-contoh-program-6.png)
Output:
![Output Program 6](/img/dsa/pointer-output-program-6.png)
Terlihat bahwa nilai px adalah alamat dari x dan nilai ppx adalah alamat dari px. Perhatikan contoh di bawah, untuk mengetahui cara mengakses nilai x dari masing-masing ponter px dan ppx.
![Program 7](/img/dsa/pointer-contoh-program-7.png)
![Output Program 7](/img/dsa/pointer-output-program-7.png)

Pada baris satu, program langsung menampikan nilai x. Di baris ke-2, program akan menampilkan nilai dari alamat memori yang tersimpan di variabel px. Lalu pada baris ke-3, reference dilakukan sebanya 2 kali. Pertama reference ke alamat memori yang tersimpan di variabel ppx, lalu dreference lagi untuk mendapatkan nilai dari alamat memori yang tersimpan di px, ditampikanlah angka 5 yang merupakan nilai yang tersimpan di alamat memori x.

Silahkan lihat ilustrasi di bawah untuk memudahkan pemahaman.

![Ilustrasi 6](/img/dsa/pointer-ilustrasi-6.png)
