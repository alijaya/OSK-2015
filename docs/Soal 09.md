# Soal 09

## Topik

* Teori Bilangan

## Deskripsi

Ada berapa banyak bilangan 3-digit yang habis dibagi dengan 13?

* A. 68
* B. 69
* C. 70
* D. 71
* E. 72

## Jawaban

**B. 69**

## Pembahasan

Bilangan tiga digit berbeda yaitu seluruh bilangan bulat di antara 100 dan 999 inklusif. Sehingga, kita tinggal mencari banyaknya kelipatan 13 di antara 100 hingga 999.

Banyaknya kelipatan x dalam range [1,a] yaitu sebanyak `a div x`.

Dengan mengetahui formula di atas, kita dapat mencari banyaknya kelipatan 13 dalam range [100,999] dengan cara berikut:

Banyak kelipatan 13 dalam range [100,999] = Banyak kelipatan 13 dalam range [1,999] - Banyak kelipatan 13 dalam range [1,99]
                                          = 999 div 13 - 99 div 13
                                          = 69

Jawaban: **69** bilangan.
