+++
title = 'Program Pertama'
date = 2024-09-05T20:29:14+08:00
draft = false
tags = ['pemrograman', 'python']
+++

Pada tutorial sebelumnya Anda telah belajar tentang bagaimana cara menginstall python di berbagai sistem operasi.
Sekarang Anda akan belajar membuat program python sederhana.

Buat baru lalu isi dengan text di bawah

```python
# script.py
print('Hello World')
```

Buka terminal lalu eksekusi file dengan perintah

```fish
python script.py
```

Output:
```
Hello World
```

Selamat Anda telah berhasil membuat program pertama Anda

## Penjelasan Program

Dalam python perintah `print` digunakan untuk menampilkan nilai ke layar. Semua nilai yang berada di dalam tanda kurung `()`
akan ditampilkan ke layar. Sedangkan tanda petik `''` berfungsi untuk membungkus text yang akan Anda tampilkan. Anda juga dapat
menggunakan tanda petik dua `""` untuk menampilkan text ke layar.

```python
print('Hello World')
# sama dengan
print("Hello World")
# keduanya akan menampikan hasil yang sama persis
```

## Komentar (*comment*)

Komentar dalam bahasa pemrograman tidak akan dieksekusi. Meskipun begitu komentar sangat penting untuk memberikan penjelasan
pada baris-baris kode program yang Anda tulis. Dalam python, komentar dibuat dengan menambahkan tanda pagar `#` di awal komentar.
Sebagai contoh

```python
# mencetak angka
print(18) # ini juga komentar
# print("Ilmu Komedi") <- baris ini tidak akan di eksekusi
```

Output:
```fish
18
```

Program di atas hanya akan menampilkan angka 18 dan akan mengabaikan komentarnya. Selain komentar satu baris, di python kita juga dapat
membuat komentar multi baris. Caranya adalah dengan menggunakan tanda petik 3 kali.

```python
'''Ini adalah komentar
yang lebih dari satu baris'''
print('Halo cantikkkk')
"""Ini juga komentar
yang tidak akan dieksekusi"""
```

Output:
```bash
Halo cantikkkk
```

## Alasan menggunakan komentar (*comment*)

Ada beberapa hal yang menjadikan komentar itu penting dalam dunia pemrograman.

1. Menjadikan kode yang kita tulis menjadi lebih mudah untuk dibaca
2. *Debuggin*
3. Mempermudah orang lain saat membaca program yang Anda buat

Pada pembahasan selanjutnya Anda akan belajar tentang konsep dasar dalam pemrograman python.

