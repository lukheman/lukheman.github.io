+++
title = 'Operator'
date = 2024-10-10T10:00:06+08:00
draft = true
+++

Operator dalam bahasa pemrograman adalah simbol khusus yang digunakan untuk melakukan operasi pada nilai atau variabel.
Python memiliki sangat banyak operator yang dapat digunakan. Operator-operator tersebut dapat kita kualifikasikan berdasarkan
fungsinya.

## Operator Aritmatika (*Arithmetic operators*)
Operator aritmatika digunakan untuk melakukan operasi aritmatika seperti penjumlahan, pengurangan, pembagian, perkalian, dll.

```python
a = 5
b = 2

# penjumlahan
c = a + b
print(f'{a} + {b} = {c}')

# pengurangan
c = a - b
print(f'{a} - {b} = {c}')

# perkalian
c = a * b
print(f'{a} * {b} = {c}')

# pembagian
c = a / b
print(f'{a} / {b} = {c}')

# pembagian yang hasilnya dibulatkan
c = a // b
print(f'{a} // {b} = {c}')

# sisa bagi
c = a % b
print(f'{a} % {b} = {c}')

# pangkat
c = a ** b
print(f'{a} ** {b} = {c}')

# output
# 5 + 2  = 7
# 5 - 2  = 3
# 5 * 2  = 10
# 5 / 2  = 2.5
# 5 // 2 = 2
# 5 % 2  = 1
# 5 ** 2 = 25
```

Pada contoh di atas kita melakukan operasi aritmatika pada angka 5 dan 2 yang disimpan di variabel `a` dan `b` dan hasilnya
disimpan pada variabel `c`.

## Operator penugasan (*Assignment operators*)

Operator penugasan digunakan untuk memberikan nilai pada variabel.

```python
umur = 17
```

Disini, kita menggunakan `=` untuk memberikan nilai 17 pada variabel `umur`. Selain `=`, ada lagi operator penugasan lain.
Lihat tabel di bawah ini.

| nama                      | operator | contoh    | sama dengan  |
|:--------------------------|:--------:|:---------:|:------------:|
| Assignment operator       | =        | a = b     |              |
| Addition Assignment       | +=       | a += b    | a = a + b    |
| Subtraction Assignment    | -=       | a -= b    | a = a - b    |
| Multiplication Assignment | \*=      | a \*= b   | a = a \* b   |
| Division Assignment       | /=       | a /= b    | a = a / b    |
| Remainder Assignment      | %=       | a %= b    | a = a % b    |
| Exponent Assignment       | \*\*=    | a \*\*= b | a = a \*\* b |

```python
a = 5
b = 2

a = a + b # tanpa operator penugasan
print(a)
a += b # dengan operator penugasan
print(a)

# output
# 7
# 7
```


Pada contoh di atas, kita menggunakan operator `+=` untuk memberikan nilai baru pada variabel `a`. Yaitu hasil penjumlahan
`a + b`. Hal yang sama juga berlaku untuk operator penugasan yang lain.


## Operator perbandingan (*Comparison operators*) 

Logical operators
Identity operators
Membership operators
Bitwise operators
