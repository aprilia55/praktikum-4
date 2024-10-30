# Praktikum 2 - Stuktur kondisi

Nama : Alfarizki Aprilia Putri

Kelas : TI.24.A.5

NIM : 312410455

Mata Kuliah : Bahasa Pemograman

## penggunaan stuktur kondisi menggunakan statsment `if`,`else` dan `elif` dalam python
Dalam Python, `if` dan `else` digunakan untuk pengambilan keputusan berdasarkan kondisi tertentu. Program akan mengeksekusi blok kode tertentu jika kondisi pada `if` bernilai True, dan blok lainnya (yang berada di dalam `else`) jika kondisi tersebut `False`

apa itu `elif`?

`elif` adalah singkatan dari `else if`." Ini digunakan dalam struktur kontrol `if` untuk menambahkan kondisi tambahan setelah kondisi awal yang diuji. Jika kondisi pertama (yang diawali dengan `if`) adalah `False`, maka Python akan memeriksa kondisi-kondisi yang ada di setiap pernyataan `elif` secara berurutan. Jika salah satu dari kondisi `elif` tersebut adalah True, maka blok kode yang sesuai akan dieksekusi.

<font color    ## penggunaan `if` dan `else` untuk gaji karyawan

```python
if gaji > 3000000:
    print ("gaji sudah di atas UMR")
    if berkeluarga:
        print ("wajib ikutan asuransi dan menabung ntuk pensiun")
```
memeriksa apakah gaji lebih dari 3.000.000.

jika true akan mencetak "gaji sudah di atas UMR"

memeriksa apakah sudah berkeluarga?

jika true maka akan mencetak "wajib ikutan asuransi dan menabung ntuk pensiun"

```python
else:
    print ("tidak perlu ikutan asuransi")
    if punya_rumah:
        print("wajib bayar pajak rumah")

```
jika kurang dari 3.000.000. maka akan mencetak "tidak perlu ikutan asuransi"

'if punya_rumah` kalau true akan mencetak "wajib bayar pajak rumah"
![foto](https://github.com/aprilia55/flowchart-new/blob/f4f57a5d11e5f6149ec3b72f73f85adff7cd8701/Algorithm%20flowchart%20example.png)



