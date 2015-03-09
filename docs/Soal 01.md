# Soal 01

## Topik

* Kombinatorika

## Deskripsi

Pak Dengklek baru saja membuat sebuah koper. Koper tersebut memiliki sistem pengunci yang unik. Pada koper terdapat 10 tombol. Untuk membuka koper tersebut, pak Dengklek harus menekan 7 tombol yang berbeda dengan urutan tertentu. Berapa banyaknya kemungkinan urutan penekanan tombol yang ada?

* A. 604800
* B. 700
* C. 40640
* D. 120
* E. 34360

---

## Jawaban

**A. 604800**

## Pembahasan

### Pembahasan Singkat

Ini hanya soal *Permutasi* sederhana.
Dapat diselesaikan dengan rumus `P(7, 10) = **604800** cara`.

### Pembahasan Lengkap

Pekerjaan memilih urutan tombol-tombol yang akan ditekan dapat didekomposisi menjadi pekerjaan-pekerjaan berikut:

1. Memilih satu tombol yang akan ditekan **pertama**. Banyak tombol yang dapat dipilih adalah **10**.
2. Memilih satu tombol lain yang akan ditekan **kedua**. Banyak tombol yang dapat dipilih adalah **9**.
3. Memilih satu tombol lain yang akan ditekan **ketiga**. Banyak tombol yang dapat dipilih adalah **8**.
4. Memilih satu tombol lain yang akan ditekan **keempat**. Banyak tombol yang dapat dipilih adalah **7**.
5. Memilih satu tombol lain yang akan ditekan **kelima**. Banyak tombol yang dapat dipilih adalah **6**.
6. Memilih satu tombol lain yang akan ditekan **keenam**. Banyak tombol yang dapat dipilih adalah **5**.
7. Memilih satu tombol lain yang akan ditekan **ketujuh** *(terakhir)*. Banyak tombol yang dapat dipilih adalah **4**.

Sehingga, berdasarkan aturan kali, terdapat `10 * 9 * 8 * 7 * 6 * 5 * 4 = **604800** cara`.