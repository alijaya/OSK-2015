# Soal 08

## Topik

* Ad Hoc

## Deskripsi

Suatu lomba maraton diikuti oleh empat kelompok: Melati, Mawar, Dahlia, dan Anggrek. Setiap kelompok mengirimkan lima pelari. Pelari yang masuk finish ke-1, 2, 3, 4, 5, 6 memperoleh nilai berturut-turut 7, 5, 4, 3, 2, 1. Nilai setiap kelompok adalah jumlah nilai kelima pelarinya. Kelompok dengan nilai terbesar adalah juara lomba. Di akhir lomba ternyata kelompok Dahlia menjadi juara dan tidak ada dua pelari yang masuk finish bersamaan. Berapa banyak kemungkinan nilai kelompok
pemenang? 

* A. 13
* B. 14
* C. 15
* D. 16
* E. 17

---

## Jawaban
**C. 15**

## Pembahasan

Perhatikan bahwa minimal kelompok Dahlia mendapat total nilai **7**. Jika kelompok Dahlia mendapat total nilai kurang dari **7**, maka pasti ada setidaknya ada satu kelompok yang mendapat total nilai sekurangnya **7**.

Diketahui juga bahwa nilai total maksimal dari kelompok Dahlia adalah **21**, yaitu dengan mendapatkan nilai-nilai berikut: **7, 5, 4, 3, 2**.

Sehingga, untuk mengetahui banyaknya kemungkinan nilai yang diraih oleh kelompok Dahlia cukup dengan mengecek banyaknya nilai di antara **7** hingga **21** *(inklusif)* yang dapat dibentuk dengan menjumlahkan satu atau lebih bilangan dari antara **7, 5, 4, 3, 2, dan 1**.

     7 = 7
     8 = 7 + 1
     9 = 7 + 2
    10 = 7 + 3
    11 = 7 + 4
    12 = 7 + 5
    13 = 5 + 4 + 3 + 1
    14 = 5 + 4 + 3 + 2
    15 = 7 + 5 + 3
    16 = 7 + 5 + 4
    17 = 7 + 5 + 4 + 1
    18 = 7 + 5 + 4 + 2
    19 = 7 + 5 + 4 + 3
    20 = 7 + 5 + 4 + 3 + 1
    21 = 7 + 5 + 4 + 3 + 2

Sehingga, terdapat `21 - 7 + 1 = 15` kemungkinan nilai total berbeda.

Jawaban: **15**.
