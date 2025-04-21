+++
title = 'Encoder Dan Decoder'
date = 2025-04-21T19:46:38+08:00
draft = false
+++

# Encoder

Encoder adalah rangkaian digital yang berfungsi untuk mengompresi bit. Jadi informasi dalam bentuk bit akan diproses oleh rangkaian ini
dan akan diubah ke ukuran yang lebih kecil. Hanya ukuran data yang berubah tetapi informasi di dalamnya tetap sama. Encoder banyak digunakan dalam sistem komunikasi dan pengolahan data.

![Encoder](/img/encoder.png)

## Table kebenaran encoder 4 to 2

| Input | A(3) | A(2) | A(1) | A(0) | Output B(1) | Output B(0) |
|-----------|---------|---------|---------|---------|---------------|---------------|
| 0001      | 0       | 0       | 0       | 1       | 0             | 0             |
| 0010      | 0       | 0       | 1       | 0       | 0             | 1             |
| 0100      | 0       | 1       | 0       | 0       | 1             | 0             |
| 1000      | 1       | 0       | 0       | 0       | 1             | 1             |


# Decoder

Jika encoder digunakan untuk memperkecil ukuran data, maka decoder melakukan hal yang sebalinya.
Decoder akan memperluas atau mengembalikan data ke ukuran asalnya.

![Decoder](/img/decoder.png)

## Table kebenaran decoder 2 to 4

| Input | B(1)  | B(0) | Output A(3) | Output A(2) | Output A(1) | Output A(0) |
|-----------|---------------|---------------|---------------|---------------|---------------|---------------|
| 00        | 0             | 0             | 0             | 0             | 0             | 1             |
| 01        | 0             | 1             | 0             | 0             | 1             | 0             |
| 10        | 1             | 0             | 0             | 1             | 0             | 0             |
| 11        | 1             | 1             | 1             | 0             | 0             | 0             |

