# Soal 14

## Topik

* Kombinatorik
* Inklusi-Eksklusi

## Deskripsi

Berapa banyak susunan kata yang dapat dibuat dari huruf-huruf penyusun kata “INFORMATIKA” yang mengandung “RM” tetapi tidak mengandung “OF”?

* A. 816480
* B. 816408
* C. 816840
* D. 848160
* E. 846180

---

## Jawaban

**A. 816480**

## Pembahasan

Pertama kita hitung banyaknya permutasi berbeda yang dapat dibuat dari huruf-huruf penyusun kata **"INFORMATIKA"** yang mengandung **"RM"**. Kita kelompokkan menjadi **"INFOATIKA[RM]"**, banyaknya permutasinya: `10!/(2! 2!) = 907200`.

Kemudian kita menghitung banyaknya permutasi berbeda yang dapat dibuat dari huruf-huruf penyusun kata **"INFORMATIKA"** yang mengandung **"RM"** dan mengandung **"OF"**. Kita kelompokkan menjadi **"INATIKA[RM][OF]"**, banyaknya permutasinya: `9!/(2! 2!) = 90720`.

Maka banyaknya permutasi berbeda yang dapat dibuat dari huruf-huruf penyusun kata **"INFORMATIKA"** yang mengandung **"RM"** dan **tidak** mengandung **"OF"** yaitu `907200 - 90720 = 816480`.

Jawaban: **816480**.