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
# Hasil kode program
![foto](https://github.com/aprilia55/flowchart-new/blob/5072a635cf61e26e1f786ceb00f85800e3d01c2e/gaji%20py..png)

## pengunaan `if`,`else` dan `elif` untuk nilai 
```python
if akhir > 80:
    huruf = "A"
elif akhir > 70:
    huruf = "B"
elif akhir > 50:
    huruf = "C"
elif akhir > 40:
    huruf = "D"
else:
    huruf = "E"
```
`if`: Mengecek apakah nilai akhir lebih dari 80.

Jika True, variabel huruf diisi dengan "A", dan program tidak memeriksa kondisi lainnya (blok selesai di sini).

`elif`: (else if) Memeriksa kondisi tambahan jika kondisi pertama (nilai akhir > 80) False.

Jika akhir > 70: Huruf diisi "B".
Jika akhir > 50: Huruf diisi "C".
Jika akhir > 40: Huruf diisi "D".

`else`: Menangani semua kondisi lainnya (yaitu jika nilai akhir ≤ 40). Dalam kasus ini, huruf diisi dengan "E".
# flowchart
![foto](https://github.com/aprilia55/flowchart-new/blob/6fb2ec2e78af4819f6b28ea0b66f85df55b8cbea/Algorithm%20flowchart%20example%20(1).png)
# hasil kode program
![foto](https://github.com/aprilia55/flowchart-new/blob/a56d53a40545a3b2c2dd1a45acc963f9e30f29de/Rapot%20py..png)

## pengunaan kondisi `OR`

```python
if a + b == c or b + c == a or c + a == b:
```
Pada baris ini, program memeriksa beberapa kondisi menggunakan operator logika `or`.
Operator `or` digunakan untuk menggabungkan beberapa kondisi. Jika salah satu dari kondisi yang digabungkan dengan `or` adalah `True`, maka seluruh pernyataan akan dianggap `True`.
# flowchart 
![foto](https://github.com/aprilia55/flowchart-new/blob/a56d53a40545a3b2c2dd1a45acc963f9e30f29de/Algorithm%20flowchart%20bilangan%20input.png)
# hasil kode program 
![foto](https://github.com/aprilia55/flowchart-new/blob/e2a3b7a37bb96a02d6617a12df8f391e4db5688e/Bilangan%20input.png)

# Hasil kode pemrograman Ticket Bioskop 
```
python
# Fungsi untuk menghitung harga tiket
def hitung_harga_tiket(tipe_tiket, status_member):
    # Harga tiket reguler dan VIP
    harga_reguler = 50000
    harga_vip = 100000

    # Menentukan harga berdasarkan tipe tiket
    if tipe_tiket.lower() == 'reguler':
        harga_tiket = harga_reguler
    elif tipe_tiket.lower() == 'vip':
        harga_tiket = harga_vip
    else:
        print("Tipe tiket tidak valid. Silakan masukkan 'reguler' atau 'vip'.")
        return None

    # Menghitung diskon jika pengguna adalah member
    if status_member.lower() == 'ya':
        diskon = 0.2 * harga_tiket
        total_harga = harga_tiket - diskon
    elif status_member.lower() == 'tidak':
        total_harga = harga_tiket
    else:
        print("Status member tidak valid. Silakan masukkan 'ya' atau 'tidak'.")
        return None

    return total_harga

# Meminta input dari pengguna
tipe_tiket = input("Masukkan tipe tiket (reguler/vip): ")
status_member = input("Apakah Anda memiliki kartu member? (ya/tidak): ")

# Menghitung total harga
total_harga = hitung_harga_tiket(tipe_tiket, status_member)

# Menampilkan hasil jika valid
if total_harga is not None:
    print(f"Total harga yang harus dibayar: Rp{total_harga:.2f}")

```

# Penjelasan Terkait Kode Pemrograman Ticket Bioskop

# 1.Definisi Fungsi
```
python
def hitung_harga_tiket(tipe_tiket, status_member):
```
Fungsi `hitung_harga_ticket`didefinisikan menghitung total harga tiket
Menentukan tipe tiket `VIP/REGULER`
Menentukan status member (`apakah member atau tidak`)

# 2.Harga tiket
```
python
harga_reguler = 50000
harga_vip = 100000
```
Dua variabel ini ditentukan untuk menyimpan harga tiket reguler atau VIP

# 3.Menentukan harga berdasarkan tipe tiket
```
python
if tipe_tiket.lower() == 'reguler':
    harga_tiket = harga_reguler
elif tipe_tiket.lower() == 'vip':
    harga_tiket = harga_vip
else:
    print("Tipe tiket tidak valid. Silakan masukkan 'reguler' atau 'vip'.")
    return None
```
Kondisi: Menggunakan pernyataan `if` untuk memeriksa tipe tiket yang dimasukkan.
Jika pengguna memasukkan `reguler`, maka `harga_tiket` diatur ke `harga_reguler`.
Jika pengguna memasukkan `vip`, maka `harga_tiket` diatur ke `harga_vip`.
Jika tidak valid, program akan mencetak pesan kesalahan dan mengembalikan `None`

# 4.Menghitung Diskon Untuk Member
```
python
if status_member.lower() == 'ya':
    diskon = 0.2 * harga_tiket
    total_harga = harga_tiket - diskon
elif status_member.lower() == 'tidak':
    total_harga = harga_tiket
else:
    print("Status member tidak valid. Silakan masukkan 'ya' atau 'tidak'.")
    return None
```
Kondisi:Memeriksa status keanggotaan.
Jika pengguna adalah member (`ya`), diskon sebesar 20% dari `harga_tiket` dihitung dan dikurangi dari harga tiket untuk mendapatkan `total_harga`.
Jika bukan member (`tidak`), maka `total_harga` sama dengan `harga_tiket`.
Jika status member tidak valid, program akan mencetak pesan kesalahan dan mengembalikan `None`.

# 5.return total_harga
```
python
return total_harga
```
Fungsi mengembalikan nilai `total_harga`, yang merupakan jumlah yang harus dibayar oleh pengguna.

# 6.Meminta input dari pengguna
```
python
tipe_tiket = input("Masukkan tipe tiket (reguler/vip): ")
status_member = input("Apakah Anda memiliki kartu member? (ya/tidak): ")
```
Program meminta pengguna untuk memasukkan tipe tiket dan status keanggotaan.

# 7.Menghitung Total Harga
```
python
total_harga = hitung_harga_tiket(tipe_tiket, status_member)
```
Memanggil fungsi `hitung_harga_tiket` dengan `parameter` yang diberikan oleh pengguna dan menyimpan hasilnya dalam `variabel total_harga`

#8.Menampilkan Hasil
```
python
if total_harga is not None:
    print(f"Total harga yang harus dibayar: Rp{total_harga:.2f}")
```
Jika `total_harga` tidak bernilai `None`, program mencetak total harga yang harus dibayar dengan format dua desimal.

# flowchart

# hasil program 
![foto](https://github.com/aprilia55/flowchart-new/blob/cf9c4f49027ba5d9bfddafcf7e94f3f38d5392f1/Tiket%20bioskop%20py..png)







