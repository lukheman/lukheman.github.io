+++
title = 'Tmux Sebagai Terminal Manager'
date = 2024-08-10T23:49:33+08:00
+++

Sebagai seorang Programmer, pastinya kita sudah tidak asing dengan terminal dan *Command Line
Interface*. Keduanya adalah dua hal yang saling terkait, sebab untuk mengakses CLI, Kita harus
menggunakan terminal. Entah itu Alacritty, Kitty, st, dan lain sebagainya. Tak jarang pula kita
membuka banyak terminal untuk menjalankan berbagai program/proses yang berbeda secara bersamaan. Seperti
menjalankan server, memantau proses yang berjalan di latar belakang, *ngoding* (yah ngoding di terminal dengan neovim),
debugging, dan lain sebagainya. Tentunya hal ini sangat merepotkan dan sangat tidak efisien jika
kita harus menjalankan terminal berkali-kali.

<!--more-->

Untuk memecahkan masalah tersebut dibuatlah *tool* bernama [tmux](https://github.com/tmux/tmux/wiki).
Tmux adalah *tool* yang memungkinkan Anda untuk menjalankan berbagai macam program secara bersamaan
cukup dengan satu terminal. Tmux bekerja dengan membuat beberapa sesi shell yang masing-masing
menjalankan berbagai proses yang berbeda. Tidak hanya itu, di setiap sesi tmux kita bisa menambahkan
*window* dan di dalam *window* kita bisa membuat beberapa *pane*. Hal ini membuat tmux menjadi
sangat fleksibel dan menciptakan kolaborasi yang efisien.

## Menginstall Tmux
Tmux ini sudah tersedia di banyak distribusi linux. Jadi untuk menginstallnya sesuaikan saja dengan
distro linux yang Anda gunakan. Sebagai contoh saya menggunakan ArchLinux, jadi saya bisa
menggunakan pacman (package manager arch).

```fish
pacman -S tmux
```

Tunggu sampai proses instalasi selesai dan Anda siap untuk menggunakan tmux.

## Menggunakan Tmux

### Membuat Sesi (*Session*)
Untuk memulai sesi tmux, anda bisa menggunakan salah satu perintah di bawah.

```fish
# cara 1: membuat sesi
tmux
tmux new

# cara 2: membuat sesi dengan nama
tmux new -s namasesi

```

Setelah memasukan perintah di atas, Anda akan langsung berpindah ke sesi tmux dan Anda siap
menggunakan terminal Anda seperti biasanya.

![Tmux Starter Session](/img/tmux-starter.png)

Ketika membuat sesi baru, tmux secara otomatis juga membuat window dan pane baru. Jadi perintah di
atas, selain membuat sesi juga membuat *window* yang didalamnya ada *pane*.

### Membuat Window

Sekarang kita akan membuat window baru. Bagi yang kurang familiar dengan istilah window, jadi, window ini
seperti tab yang ada di browser. Nantinya Anda bisa membuat banyak window di dalam satu sesi. Untuk
membuat window baru, Anda bisa menggunakan kombinasi key `ctrl-b + c`.

![Tmux New Window](/img/tmux-new-window.png)

Perhatikan bagian bawah dari gambar di atas. Sekarang terdapat 2 window dengan nama yang sama yaitu
*fish*. Nama itu diambil dari default shell yang Anda gunakan. Anda bisa mengubah nama window yang
aktif dengan masuk ke *command mode*. Caranya dengan menekan `ctrl-b + :`. Lalu masukkan
perintah `rename-window windowbaru`.
![Tmux Rename Window](/img/tmux-rename-window.png)

![Tmux Rename Window](/img/tmux-rename-window-result.png)

`windowbaru` akan menjadi nama dari window saat ini (window aktif).

Gunakan perintah `ctrl-b + n` untuk berpindah ke window selanjutnya dan `ctrl-b + p` untuk ke window
sebelumnya.

<!-- ```fish -->
<!-- # membuat window baru -->
<!-- ctrl+b + c -->
<!---->
<!-- # berpindah ke window selanjutnya -->
<!-- ctrl+b + n -->
<!---->
<!-- # berpindah ke window sebelumnya -->
<!-- ctrl+b + p -->
<!-- ``` -->


### Membuat Pane

Seperti yang sudah saya jelaskan sebelumnya bahwa di dalam window kita bisa membuat beberapa pane.
Untuk membuat pane secara *vertical* gunakan perintah `ctrl-b + %`. Hasilnya akan terlihat seperti
di bawah.

![Tmux Vertical Pane](/img/tmux-vertical-pane.png)

Selain *vertical pane* Anda juga dapat membuat *horizontal pane*. Perintahnya adalah `ctrl-b + "`
dan hasilnya akan seperti gambar di bawah.

![Tmux Vertical Pane](/img/tmux-horizontal-pane.png)

Anda dapat berpindah pane dengan menggunakan perintah `ctrl-b + <arrow key>`.

Selanjutnya sesuaikan saya penggunaan *session*, *window*, dan *pane* dengan kebutuhan kalian.
Misalnya Anda ingin satu *session* untuk setiap projek yang berbeda. Lalu di dalam *session*
tersebut Anda menjalankan neovim di window pertama, lalu membuat window baru dan menjalankan server
di window tersebut. Selanjutnya Anda ingin menjalankan database client seperti [pgcli](https://www.pgcli.com/)
di samping server Anda.

Itulah dasar penggunaan tmux. Selain perintah di atas, masih banyak lagi perintah-perintah yang dapat Anda gunakan
untuk mengelola session, window, dan pane. Anda juga dapat menyesuaikan konfigurasi tmux mulai dari
tampilan sampai keybind yang digunakan.

## Referensi

- https://tmuxcheatsheet.com
- https://quickref.me/tmux
- https://github.com/tmux/tmux/wiki
