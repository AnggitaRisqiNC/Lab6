# Lab6
Anggita Risqi Nur Clarita (312210450)

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Latihan|[Click Here](#latihan)|
|2|Lab 6|[Click Here](#lab-6)|
|3|Flowchart Lab 6|[Click Here](#flowchart)|

## Latihan
Ubahlah Kode dibawah ini menjadi fungsi menggunakan lambda.
```python
import math

def a(x):
return x**2

def b(x, y):
return math.sqrt(x**2 + y**2)

def c(*args):
return sum(args)/len(args)

def d(s):
return "".join(set(s))
```
### Rumusnya
```python
# Latihan

print("Nama : Anggita Risqi Nur Clarita")
print("NIM  : 312210450")
print("--------------------------------")

import math
def a(x):
    return x**2
    a = lambda x: x**2, a
print(a(2))

def b(x, y):
    return math.sqrt(x**2 + y**2)
    b = lambda x, y: x**2 + y**2, b
print(b(2, 4))

def c(*args):
    return sum(args) / len(args)
    c = lambda*args: sum(args) / len(args)
print(c(10, 50))

def d(s):
    return "".join(set(s))
    d = lambda s: "".join(set(s))
print(d("Hilmy"))
```
### Programnya
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Lat%201.png)

### Hasil dari programnya (RUN)
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Lat%201%20(run).png)

## Lab 6
Buat program sederhana dengan mengaplikasikan penggunaan fungsi yang akan menampilkan daftar nilai mahasiswa, dengan ketentuan:
* Fungsi _tambah()_ untuk menambah data.
* Fungsi _tampilkan()_ untuk menampilkan data.
* Fungsi _hapus(nama)_ untuk menghapus data berdasarkan nama.
* Fungsi _ubah(nama)_ untuk mengubah data berdasarkan nama.
* Buat Flowchart dan Penjelasan Programnya pada README.md.
* Commit dan push repository ke github.

### Rumusnya
```python
# Lab 6

print("Nama : Anggita Risqi Nur Clarita")
print("NIM  : 312210450")
print("--------------------------------")

data = {}
# Untuk Menambahkan Data
def tambah():
    print()
    print("Tambah Data")
    nama  = input    ("Nama        : ")
    nim   = input    ("NIM         : ")
    tugas = int(input("Nilai Tugas : "))
    uts   = int(input("Nilai UTS   : "))
    uas   = int(input("Nilai UAS   : "))
    nilaiakhir = ((tugas) * 30 / 100 + (uts) * 35 / 100 + (uas) * 35 / 100)
    data[nama] = [nim, tugas, uts, uas, nilaiakhir]
    return

# Untuk Menampilkan Data
def tampilkan():
    if data.items():
        print()
        print("Daftar Nilai")
        print()
        print("=======================================================================================");
        print("|     NAMA    |      NIM      |    TUGAS    |     UTS     |     UAS     | Nilai Akhir |");
        print("=======================================================================================");
        i = 0
        for x in data.items():
            i+=i
            print("|  {0:9}  |   {1:9}   |  {2:9}  |  {3:9}  |  {4:9}  |  {5:9}  |"
                  .format(x[0][: 14], x[1][0], x[1][1], x[1][2], x[1][3], x[1][4], i))
            print("=======================================================================================");

    else :
        print()
        print("Daftar Nilai")
        print()
        print("======================================================================================");
        print("|    NAMA    |      NIM      |    TUGAS    |     UTS     |     UAS     | Nilai Akhir |");
        print("======================================================================================");
        print("|                                  TIDAK ADA DATA                                    |");
        print("======================================================================================");
    return

# Untuk Menghapus data  Berdasarkan Nama
def hapus():
    print()
    print("Hapus Data Mahasiswa")
    nama  = input    ("Nama       : ")
    if nama in data.keys():
        del data[nama]
    else:
        print("Data {0} tidak ada".format(nama))
    return

# Untuk Mengubah data Berdasarkan Nama
def ubah():
    print()
    print("Ubah Data Mahasiswa")
    nama = input("Nama        : ")
    if nama in data.keys():
        nim   = input    ("NIM         : ")
        tugas = int(input("Nilai Tugas : "))
        uts   = int(input("Nilai UTS   : "))
        uas   = int(input("Nilai UAS   : "))
        nilaiakhir = ((tugas) * 30 / 100 + (uts) * 35 / 100 + (uas) * 35 / 100)
        data[nama] = [nim, tugas, uts, uas, nilaiakhir]
    else:
        print("Data nilai{0} tidak ada".format(nama))

while True:
    print()
    print("|1| Lihat Data")
    print("|2| Tambah Data")
    print("|3| Ubah Data")
    print("|4| Hapus Data")
    print("|5| Keluar")

    x = input(">> PILIH MENU : ")

    if x == '1':
        tampilkan()
    elif x == '2':
        tambah()
    elif x == '3':
        ubah()
    elif x == '4':
        hapus()

    else:

        exit()
```
### Programnya
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Lab%206%20(1).png)
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Lab%206%20(2).png)
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Lab%206%20(3).png)
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Lab%206%20(4).png)

### Hasil dari programnya (RUN)
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Lab%206%20(run%201).png)
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Lab%206%20(run%202).png)
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Lab%206%20(run%203).png)
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Lab%206%20(run%204).png)
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Lab%206%20(run%205).png)
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Lab%206%20(run%206).png)

### Penjelasan Programnya
1. Definisikan dictionary terlebih dahulu _data = {}_.
2. Membuat fungsi
* Fungsi tampilkan(), untuk menambahkan data _def tampilkan()_
* Fungsi tambah(), untuk menampilkan data _def tambah()_
* Fungsi hapus(nama), untuk menghapus nama pada data _def hapus(nama)_
* Fungsi ubah(nama), untuk mengubah nama pada data _def ubah(nama)_
3. Menggunakan Perulangan _while True:_ dapat diartikan perulangan akan terus mengulang jika inputan benar dan masuk kedalam proses jika tidak maka perulangan berhenti atau lanjut ke proses selanjutnya. Gunakan statement if untuk memproses perintah yang di inginkan sesuai inputan.
4. Untuk menambahkan data pilih _"[1] Tambah"_ gunakan fungsi _if_ gunakan perintah _"1"_, lalu masukan nama, nim, tugas, uts, uas, nilaiakhir, nilai akhir didapat dari _= ((tugas)*30/100 + (uts)*35/100 + (uas)*35/100_.
5. Lalu jika ingin memilih "[2] Lihat" gunakan fungsi _'elif'_ dan gunakan fungsi _'for x in data.items():'_ untuk melihat data pada tabel data yang kita inputkan, dengan perintah _"2"_. Jika data tidak terdaftar maka akan tampil _"TIDAK ADA DATA"_ atau = 0.
6. Lalu untuk menampilan pilihan _"[3] Ubah"_ gunakan fungsi _'elif'_ kemudian gunakan fungsi _'if nama in data.keys():'_ kemudian input nama, nim, nilai tugas, nilai uts, nilai uas untuk mengubah data nama kemudian gunakan fungsi _'else'_ untuk menampilkan data nama yang kita ingin ubah tidak ada.
7. Untuk menghapus data pilih _"[4] Hapus"_ gunakan fungsi _'elif'_ kemudian gunakan fungsi _'if nama in data.keys():'_ kemudian fungsi _'del.data[nama]_ jika nama yang kita hapus tidak ada dalam tabel maka gunakan fungsi _'else'_ untuk menampilkan _"TIDAK ADA DATA"_.
8. Untuk keluar maka gunakan fungsi _else_ dan _exit()_ atau gunakan perintah _[5] Keluar_.
9. Selesai.

### Flowchart
![image](https://github.com/AnggitaRisqiNC/Lab6/blob/main/Screenshot/Flowchart%20Lab6.png)

## Finish