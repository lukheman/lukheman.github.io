+++
title = 'Pengenalan Variabel'
date = 2024-09-19T09:08:55+08:00
draft = false
+++


Pada bagian ini kita akan belajar tentang variabel dalam bahasa pemrograman python.

Dalam bahasa pemrograman, variabel dikenal sebagai tempat untuk menyimpan data, baik data yang
berbentuk text, angka, *list*, *dictionary*, ataupun *boolean*. Lebih lanjut tentang data akan kita pelajari pada materi
tentang tipe data.

## Membuat Variabel

Di python variabel dapat dibuat dengan menuliskan nama variabel dan memberikan nilai dengan menggunakan tanda sama dengan (`=`).

```python
nama = 'sofhia' # variabel nama menyimpan nilai string 'sofhia'
umur = 18       # variabel umur menyimpan nilai int 18
tinggi = 160.5  # variabel tinggi menyimpan nilai float 160.5
```

## Aturan penamaan variabel

Penamaan variabel dalam bahasa pemrograman tidak dapat dilakukan denga asal-asalan. Ada aturan-aturan tertentu yang harus dipenuhi
agar variabel menjadi valid.

1. Nama variabel harus dimulai dari huruf (A-Z atau a-z) ataupun *underscore* (`_`)
2. Nama variabel tidak boleh dimulai dari angka
3. Nama variabel bersifat *case sensitive* artinya `umur` dan `Umur` adalah 2 variabel yang berbeda
4. Nama variabel tidak menggunakan kata kunci *keywords* python seperti `if`, `def`, `for`, dll

Contoh penamaan variabel yang benar

```python
_nama = 'lukhe'
angka10 = 10
usia_sekarang = 18
```

Contoh penamaan variabel yang salah

```python
1nama = 'lukhe'     # -> variabel tidak boleh dimulai dengan angka
if = 10             # -> variabel tidak boleh menggunakan keywords python
@usia_sekarang = 18 # -> variabel tidak boleh menggunakan karakter spesial
```

## Merubah isi variabel

Di python, variabel yang telah dideklarasikan dapat dirubah nilainya kapan saja. Hal ini dapat dilakukan dengan teknik *overriding*.

```python
nama = 'akmal'
nama = 'sofhia' # -> nilai variabel nama akan berubah dari 'akmal' menjadi 'sofhia'
```

## Mencetak nilai variabel

Kita dapat mencetak nilai variabel dengan menggunakan fungsi `print`

```python
nama = 'sofhia' # variabel nama menyimpan nilai string 'sofhia'
umur = 18       # variabel umur menyimpan nilai int 18
tinggi = 160.5  # variabel tinggi menyimpan nilai float 160.5

print(nama)     # mencetak variabel nama
print(umur)     # mencetak variabel umur
print(tinggi)   # mencetak variabel tinggi

# output:
# sofhia
# 18
# 160.5
```

Kita telah tentang variabel, pada bagian selanjutnya kita akan belajar tentang tipe data. Tipe data secara singkat bisa kita artikan
sebagai nilai yang diproses dalam program yang kita buat. Untuk lebih jelasnya silahkan lanjut ke bagian selanjutnya.
