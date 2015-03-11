# Soal 06

## Topik

* Bruteforce
* Dynamic Programming

## Deskripsi

Terdapat 5 orang petualang dan mereka semua lapar. Di tengah perjalanan mereka memutuskan untuk makan siang di TOKI Fried Kitchen. Berikut adalah menu yang ditawarkan TOKI Fried Kitchen dengan harga dalam ribuan rupiah.
	-Nasi 				4
	-Burger 			5
	-Paket Lauk 		2
	-Es Cendol 			1

Secara kolektif mereka semua hanya memiliki 30 ribu rupiah untuk makan siang. Berikut adalah cara mereka menentukan makanan yang dipesan:
	- setiap orang akan makan nasi atau burger;
	- setiap orang yang memesan nasi harus memesan juga paket lauk;
	- setiap orang, baik yang memesan nasi maupun burger, dapat memesan paling banyak satu es cendol.

Jika uang mereka tidak harus seluruhnya dibelanjakan (tetapi tetap harus memenuhi kriteria diatas), tentukan ada berapa banyak cara mereka membagi menu makan siang.

* A. 638
* B. 613
* C. 546
* D. 462
* E. 372

## Jawaban
**A. 638**

## Pembahasan

Konvensi:

	C(n,k) adalah notasi untuk nilai yang menyatakan banyaknya kombinasi untuk memilih k dari n objek berbeda

Fakta:
	Terdapat X pilihan 'paket' makanan untuk setiap orang:
		1) Nasi, paket lauk (total 6 ribu rupiah);
		2) Nasi, paket lauk, es cendol (total 7 ribu rupiah);
		3) Burger (total 5 ribu rupiah);
		4) Burger, es cendol (total 6 ribu rupiah).

Dari fakta-fakta tersebut, dapat ditarik beberapa kesimpulan:
	* Memesan makanan untuk kelima orang tersebut membutuhkan minimal 25 ribu rupiah (yaitu dengan membeli burger untuk masing-masing dari kelima orang tersebut) [1]

	* Dari premis [1], dapat ditarik kesimpulan juga bahwa untuk seseorang yang telah membeli burger, terdapat tiga buah 'aksi' yang dapat dilakukan:
>1) Tidak melakukan apa-apa (tetap memesan burger) dengan biaya tambahan 0 ribu rupiah;
>2) Mengganti pilihan makanan utama menjadi nasi + paket lauk dengan biaya tambahan 1 ribu rupiah;
>3) Mengganti pilihan makanan utama menjadi nasi + paket lauk dan es cendol dengan biaya tambahan 2 ribu rupiah;
>4) Menambah es cendol dengan biaya tambahan 1 ribu rupiah.

Sehingga, banyak kemungkinan pemesanan adalah:
	1) Dengan tambahan 0 ribu rupiah, maka hanya ada tepat satu kombinasi pemesanan makanan (seluruhnya burger)
	2) Dengan tambahan 1 ribu rupiah, maka ada beberapa kombinasi pemesanan makanan:
		i) 	 Satu orang melakukan aksi (2): Ada C(5,1) = 5 cara
		ii)	 Satu orang melakukan aksi (4): Ada C(5,1) = 5 cara
	3) Dengan tambahan 2 ribu rupiah, maka ada beberapa kombinasi pemesanan makanan:
		i) 	 Dua orang melakukan aksi (2): Ada C(5,2) = 10 cara
		ii)  Dua orang melakukan aksi (4): Ada C(5,2) = 10 cara
		iii) Satu orang melakukan aksi (2), satu orang lainnya melakukan aksi (4): Ada C(5,1) * C(4,1) = 20 cara
		iv)  Satu orang melakukan aksi (3): Ada C(5,1) = 5 cara
	4) Dengan tambahan 3 ribu rupiah, maka ada beberapa kombinasi pemesanan makanan:
		i)   Tiga orang melakukan aksi (2): Ada C(5,3) = 10 cara
		ii)  Dua orang melakukan aksi (2), satu orang lainnya melakukan aksi (4): Ada C(5,2) * C(3,1) = 30 cara
		iii) Dua orang melakukan aksi (4), satu orang lainnya melakukan aksi (2): Ada C(5,2) * C(3,1) = 30 cara
		iv)  Tiga orang melakukan aksi (4): Ada C(5,3) = 10 cara
		v)   Satu orang melakukan aksi (3), satu orang lainnya melakukan aksi (2): Ada C(5,1) * C(4,1) = 20 cara
		vi)  Satu orang melakukan aksi (3), satu orang lainnya melakukan aksi (4): Ada C(5,1) * C(4,1) = 20 cara
	5) Dengan tambahan 4 ribu rupiah, maka ada beberapa kombinasi pemesanan makanan:
		i)   Empat orang melakukan aksi (2): Ada C(5,4) = 5 cara
		ii)  Tiga orang melakukan aksi (2), satu orang lainnya melakukan aksi (4): Ada C(5,3) * C(2,1) = 20 cara
		iii) Dua orang melakukan aksi (2), dua orang lainnya melakukan aksi (4): Ada C(5,2) * C(3,2) = 30 cara
		iv)  Dua orang melakukan aksi (2), satu orang lainnya melakukan aksi (3): Ada C(5,2) * C(3,1) = 30 cara
		v)   Satu orang melakukan aksi (2), tiga orang lainnya melakukan aksi (4): Ada C(5,1) * C(4,3) = 20 cara
		vi)	 Satu orang melakukan aksi (2), satu orang lainnya melakukan aksi (4), satu orang lainnya lagi melakukan aksi (3): Ada C(5,1) * C(4,1) * C(3,1) = 60 cara
		vii) Dua orang melakukan aksi (3): Ada C(5,2) = 10 cara
		viii)Satu orang melakukan aksi (3), dua orang lainnya melakukan aksi (4): Ada C(5,1) * C(4,2) = 30 cara
		ix)  Empat orang melakukan aksi (4): Ada C(5,4) = 5 cara
	6) Dengan tambahan 5 ribu rupiah, maka ada beberapa kombinasi pemesanan makanan:
		i)   Lima orang melakukan aksi (2): Ada C(5,5) = 1 cara
		ii)  Empat orang melakukan aksi (2), satu orang sisanya melakukan aksi (4): Ada C(5,4) * C(1,1) = 5 cara
		iii) Tiga orang melakukan aksi (2), dua orang sisanya melakukan aksi (4): Ada C(5,3) * C(2,2) = 10 cara
		iv)  Tiga orang melakukan aksi (2), satu orang lainnya melakukan aksi (3): Ada C(5,3) * C(2,1) = 20 cara
		v)   Dua orang melakukan aksi (2), tiga orang sisanya melakukan aksi (4): Ada C(5,2) * C(3,3) = 10 cara
		vi)  Dua orang melakukan aksi (2), satu orang melakukan aksi (4), satu orang lainnya melakukan aksi (3): Ada C(5,2) * C(3,1) * C(2,1) = 60 cara
		vii) Satu orang melakukan aksi (2), empat orang lainnya melakukan aksi (4): Ada C(5,1) * C(4,4) = 5 cara
		viii)Satu orang melakukan aksi (2), dua orang lainnya melakukan aksi (4), satu orang lainnya melakukan aksi (3): Ada C(5,1) * C(4,2) * C(2,1) = 60 cara
		ix)  Satu orang melakukan aksi (2), dua orang lainnya melakukan aksi (4): Ada C(5,1) * C(4,2) = 30 cara
		x)   Lima orang melakukan aksi (4): Ada C(5,5) = 1 cara
		xi)  Tiga orang melakukan aksi (4), satu orang lainnya melakukan aksi (3): Ada C(5,3) * C(2,1) = 20 cara
		xii) Satu orang melakukan aksi (4), dua orang lainnya melakukan aksi (3): Ada C(5,1) * C(4,2) = 30 cara

Total cara: 1 + 10 + 45 + 120 + 210 + 252 = **638** cara.

Jawaban: **638** cara.
