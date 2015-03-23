# Soal 15

## Topik

* Inklusi-Eksklusi

## Deskripsi

Berapa banyak bilangan bulat antara 1 sampai dengan 100 yang habis dibagi 3 atau 5?

* A. 6
* B. 10
* C. 15
* D. 47
* E. 49

---

## Jawaban

**D. 47**

## Pembahasan

Untuk menghitung banyaknya bilangan **[1..100]** yang habis dibagi **3** *atau* **5**, kita perlu menghitung:

* banyaknya bilangan bulat antara **1** sampai dengan **100** yang habis dibagi **3**: `floor (100 / 3) = 33`
* banyaknya bilangan bulat antara **[1..100]** yang habis dibagi **5**: `floor (100 / 5) = 20`
* banyaknya bilangan bulat antara **[1..100]** yang habis dibagi **3** *dan* **5**: `floor (100 / 15) = 6`

Maka banyaknya bilangan bulat dari **1** sampai **100** yang habis dibagi **3** *atau* **5** yaitu: `33 + 20 - 6 = 47`

Jawaban: **47**.