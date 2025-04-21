+++
title = 'Multiplexer Dan Demultiplexer'
date = 2025-04-21T19:21:43+08:00
draft = false
+++

# Multiplexer

Multiplexer adalah rangkaian digital yang memproses banyak input dan meneruskannya ke output.
Rangkaian ini digunakan untuk memilih data yang akan diproses.


## Table Kebenaran Mux 2 to 1

| Selector | Output |
|----------|--------|
|    0     |   A    |
|    1     |   B    |

## Table Kebenaran Mux 4 to 1


| S1 | S0 | Output |
|----|----|--------|
|  0 |  0 |   A    |
|  0 |  1 |   B    |
|  1 |  0 |   C    |
|  1 |  1 |   D    |

Di bawah ini adalah gambar multiplexer 2x1 dan 4x1.

![Multiplexer](/img/multiplexer.png)


Multiplexer biasa digunakan pada perangkat memori, antarmuka I/O, dan memproses sinyal digital.

# Demultiplexer
 Juka multiplexer berfungsi sebagai data selector, maka demultiplexer berfungsi sebagai data distributor.
Maksudnya adalah demultiplexer akan menerima satu input dan mengirimnya ke salah satu dari beberapa output.
Untuk mengatur output diperlukan yang namanya sinyal kontrol.


# Table Kebenaran Demux 1 to 2

| S | D | Y0 | Y1 |
|---|---|----|----|
| 0 | 0 |  0 |  0 |
| 0 | 1 |  1 |  0 |
| 1 | 0 |  0 |  0 |
| 1 | 1 |  0 |  1 |


# Table Kebenaran Demux 1 to 4

| S1 | S0 | D | Y0 | Y1 | Y2 | Y3 |
|----|----|---|----|----|----|----|
|  0 |  0 | 0 |  0 |  0 |  0 |  0 |
|  0 |  0 | 1 |  1 |  0 |  0 |  0 |
|  0 |  1 | 0 |  0 |  0 |  0 |  0 |
|  0 |  1 | 1 |  0 |  1 |  0 |  0 |
|  1 |  0 | 0 |  0 |  0 |  0 |  0 |
|  1 |  0 | 1 |  0 |  0 |  1 |  0 |
|  1 |  1 | 0 |  0 |  0 |  0 |  0 |
|  1 |  1 | 1 |  0 |  0 |  0 |  1 |

Di bawah ini adalah gambar demultiplexer 1x2 dan 1x4.

![Demultiplexer](/img/demultiplexer.png)

Penerapan dari rangkaian demultiplexer meliputi:

- Pemilihan perangkan I/O untuk trasfer data
- Mengatifkan unit fungsi yang berbeda
- Sistem pemantauan keamanan
