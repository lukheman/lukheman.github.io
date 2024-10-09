+++
title = 'Tipe Data'
date = 2024-09-25T14:21:35+08:00
draft = false
+++

Dalam dunia pemrograman, tipe data adalah adalah konsep yang sangat penting untuk dipahami. Variabel dapat
menyimpan berbagai tipe data yang berbeda, dan setiap tipe data dapat melakukan hal yang berbeda pula.

Dalam bahasa pemrograman python, setidaknya ada x jenis tipe data yang paling sering digunakan, yaitu *str*,
*int*, *float*, *list*, *tuple*, *dict*, *set*, dan *bool*.

## String

String atau *str* adalah tipe data yang kita gunakan untuk menyimpan data dalam bentuk text. String dalam python
dibuat menggunakan tanda petik satu `''` atau petik dua `""`. Anda dapat menampilkan string dengan menggunakan `print()`.

```python
nama = "Feni"
print(nama)

hobi = 'Bermain basket'
print(hobi)

# output:
# Feni
# Bermain basket
```

Pada contoh di atas, kita membuat variabel dan `nama` dan `hobi` yang masing-masing kita isi dengan string `"Feni"` dan `'Bermain basket'`.

## Tipe data angka

Tipe data angka digunakan untuk menyimpan nilai dalam bentuk bilangan. Python sendiri mempunyai 2 tipe data angka
yaitu `int` untuk bilangan bulat dan `float` untuk bilangan pecahan. Misalkan anda punya data umur dan tinggi badan seperti di bawah

- umur 18
- tinggi 165.5

Data di atas ketika disimpan di dalam sebuah variabel dapat menjadi seperti di bawah.

```python
umur = 18 # int (tidak memiliki angka di belakang titik)
tinggi = 165.5 # float (memiliki angka di belakang titik)

print('Umur saya adalah ', umur, ' tahun')
print('Tinggi saya adalah ', tinggi, ' cm')

# Output:
# Umur saya adalah 18 tahun
# Tinggi saya adalah 165.5 cm
```

## Boolean

Selanjutnya ada tipe data boolean. Tipe data ini hanya memiliki dua nilai yaitu `True` dan `False`. Meskipun hanya memiliki dua nilai,
tapi inilah yang menjadi landasan dalam menentukan alur program kita. Nanti kita akan pelajari pada bagian tentang *control flow*. Coba
lihat contoh tipe data boolean di bawah.

```python
menikah = False
makan = True

print(menikah)
print(makan)

# output:
# False
# True
```

Nilai `False` pada variabel menikah merepresentasikan keadaan belum. Sedangkan `True` pada variabel makan berarti sudah.
Saya belum menikah dan saya sudah makan. Begitulah kira-kira kalau dibaca dalam bahasa "kasar".

## List

Bayangkan Anda memiliki daftar 5 orang teman kelas dan Anda akan menyimpan setiap nama mereka ke dalam sebuah variabel. Secara
sederhana Anda dapat membuat membuat satu variabel untuk setiap nama. Lihatlah contoh di bawah.

```python
nama1 = 'akmal'
nama2 = 'dimas'
nama3 = 'yudha'
nama4 = 'teteh'
nama5 = 'veni'
```

Seolah tidak ada yang aneh dengan kodingan di atas, ketika dijalankanpun tidak akan *error*.Tapi coba bayangkan Anda memiliki 50 daftar
nama dan harus menampungnya ke variabel satu persatu. Itu berarti Anda harus membuat 50 variabel nama mulai dari `nama1`, `nama2`, `nama3`,
dan seterusnya sampai `nama50`. Cara tersebut pastinya sangat merepotkan dan sangat tidak disarankan.

Alih-alih membuat banyak variabel mengapa tidak kita tampung saja daftar nama itu ke dalam satu variabel `daftar_nama`. Disinilah
kita akan menggunakan *list* .

```python
daftar_nama = ['akmal', 'dimas', 'yudha', 'teteh', 'veni']

print(daftar_nama)

# output:
# ['akmal', 'dimas', 'yudha', 'teteh', 'veni']
```

Kode di atas terlihat lebih rapih dan lebih mudah dibaca bukan? *List* di dalam python adalah tipe data yang dapat menampung banyak data
di dalamnya. Tipe data ini dibuat dengan menggunakan tanda kurung siku `[]`. Sangat mudah bukan?

Data yang bisa kita simpan di dalam list tidak terbatas pada satu jenis data, namun dapat berbagai tipe data yang berbeda. Anda bahkan
dapat menyimpan list di dalam list (*multi dimensional list*), itu akan kita pelajari nanti.

```python
angka = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10] # list dengan satu jenis data
biodata = ['Lukhe', 18, False] # list dengan beberapa tipe data yang berbeda
matrix = [
 [1, 2, 3],
 [4, 5, 6],
 [7, 8, 9],
] # multi dimensional list
```

Ketiga contoh di atas valid dan untuk lebih meyakinkan Anda silahkan tulis kode tersebut di kode editor lalu jalankan dan lihat hasilnya.

## Tuple

Tuple adalah tipe data yang sangat mirip dengan list dari segi fungsi. Namun dalam pembuatan tuple Kita tidak menggunakan tanda kurung siku `[]`
melainkan kurung biasa `()`.

```python
angka_ganjil = (1, 3, 5, 7, 9) # tuple yang di isi dengan angka
biodata = ('Afe', 17, True) # tuple yang di isi dengan tipe data yang berbeda

print(angka_ganjil)
print(biodata)

# output:
# (1, 3, 5, 7, 9)
# ('Afe', 17, True)
```

Bagaimana? Sangat mirip dengan list bukan? Meskipun terlihat sangat mirip, namun *list* dan *tuple* sangatlah berbeda. Perbedaan keduanya
akan kita bahasa di artikel terpisah.


## Dictionary

Dictionary atau *dict* digunakan untuk menyimpan data dalam format key:value. Dictionary dibuat dengan menempatkan pasangan key:value di
dalam tanda kurung kurawal `{}`, dan dipisahkan oleh tanda koma.

```python
# membuat dictionary

biodata = {
    'nama': 'Lukmanul Rahman',
    'umur': 18,
    'prodi': 'Ilmu Komputer',
}

# tampilkan biodata
print(biodata)

# output:
# {'Nama': 'Lukmanul Rahman', 'Umur': 18, 'Prodi': 'Ilmu Komputer'}
```

Variabel `biodata` berisi tiga buah item (pasangan key:value), yang mana *'nama'* akan menjadi key dari nilai *'Lukmanul Rahman'*.
Begitu pula seterusnya. Lantas bagaimana cara kita mengakses nilai yang ada dalam dictionary? Kita dapat mengakses nilai dari sebuah
dictionary dengan menggunakan format berikut.

nama_variabel[key]

Sekarang kita akan mengakses setiap nilai yang ada dalam dictionary dan menyimpannya ke suatu variabel.

```python
# dapatkan setiap data dan simpan di variabel baru
nama  = biodata['nama']
umur  = biodata['umur']
prodi = biodata['prodi']

# tampilkan setiap data
print('Nama:', nama)
print('Umur:', umur)
print('Prodi:', prodi)

# output:
# Nama: Lukmanul Rahman
# Umur: 18
# Prodi: Ilmu Komputer
```

Jika kode yang Anda tuliskan benar maka seharusnya Anda bisa melihat output seperti di atas. Kelebihan menggunakan dictionary adalah
data yang Anda buat akan terlihat lebih rapih dan mudah dimengerti. Namun tidak hanya itu, karna masih banyak kelebihan dari dictionary
yang akan kita bahasa di artikel terpisah.

## Kesimpulan

Itulah beberapa tipe data yang paling sering digunakan dalam bahasa pemrograman python. Sebenarnya data-data tersebut dapat kita manipulasi.
Namun materi tersebut akan kita bahas di bagian terpisah.
