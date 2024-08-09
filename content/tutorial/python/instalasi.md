+++
title = 'Instalasi'
date = 2024-08-07T12:09:53+08:00
draft = false
tags = ['pemrograman', 'python']
+++

Python termasuk ke dalam bahasa pemrograman tingkat tinggi yang mampu berjalan di atas berbagai
sistem operasi, entah itu Windows ataupun Linux.

Untuk mengeksekusi kode Python, Anda perlu menginstall Interpreter Python di sistem operasi yang
anda gunakan. Interpreter berfungsi untuk mengubah kode python yang Anda tulis menjadi Kode mesin
yang dimengerti oleh komputer.

Pada tutorial ini saya akan menjelaskan tahapan instalasi python pada sistem operasi Windows dan
linux.

## 1. Mengekstrak Binary File

Cara yang pertama ini berlaku untuk Anda yang menggunakan Windows dan linux.

Yang pertama harus Anda lakukan untuk menginstall python di sistem operasi Anda adalah mendownload
*binary file* dari website resmi python. Untuk tutorial ini saya menggunakan versi python yang paling
baru yaitu Python 3.12.4. Anda dapat mendownloadnya [di sini](https://www.python.org/ftp/python/3.12.4/Python-3.12.4.tar.xz).

Jika Anda telah mendownloadnya maka tahap selanjutnya adalah mengekstrak file tersebut. Untuk
mengekstrak file saya biasanya menggunakan CLI (Command Line Interface). Caranya anda bisa membuka
terminal alacritty, kitty, atau apapun itu lalu masuk ke folder Downloads dan masukan perintah di bawah.

```fish
tar -xzvf Python-3.12.4.tar.xz
```

Setelah itu akan ada folder Python-3.12.4. Masuk ke folder tersebut lalu masukan perintah di bawah
secara berurutan.

```fish
./configure
make
```

Perintah di atas akan melakukan konfigurasi dan instalasi python secara otomatis. Silahkan tunnggu beberapa
menit sampai proses instalasi selesai. Jika proses telah selesai maka akan ada file dengan nama `python`.
Untuk mengecek versi python yang telah anda install, silahkan masukan perintah di bawah.

```fish
python --version

# Output:
# Python 3.12.4
```

Pada tahap ini Anda telah berhasil menginstall python di komputer yang Anda gunakan. Selanjutnya
silahkan pindahkan file `python` ke folder `bin`.

<blockquote>
Cara lain untuk pengguna windows adalah dengan mendownload Python melalui Microsoft Store.
</blockquote>

## 2. Menginstall Python Melalui Package Manager

Untuk cara yang kedua ini berlaku hanya untuk para pengguna Linux. Caranya pun cukup mudah. Cukup
masuk ke terminal lalu install dengan *Package Manager* yang Anda gunakan.

### ArchLinux
```fish
sudo pacman -S python3
```
### Ubuntu/Debian
```fish
sudo apt update
sudo apt install python3
```

### Fedora
```fish
sudo dnf install python3
```

### CentOS/RHEL
```fish
sudo yum install python3
```

Jika proses instalasi telah selesai, Anda bisa memastikan versi python yang terinstall dengan
perintah `python --version`.

Sampai di sini anda telah berhasil menginstall python dan siap untuk menulis *codingan*. Anda akan
belajar hal itu di tutorial selanjutnya.
