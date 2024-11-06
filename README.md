---

# Cek Nomor Genap/Ganjil

Aplikasi sederhana berbasis GUI menggunakan Java Swing untuk memeriksa apakah suatu angka adalah bilangan **genap** atau **ganjil**. Aplikasi ini juga memiliki fitur tambahan untuk memeriksa apakah angka tersebut merupakan **bilangan prima**.

## Fitur

- **Cek Genap/Ganjil**: Aplikasi akan menampilkan apakah angka yang dimasukkan adalah genap atau ganjil.
- **Cek Bilangan Prima**: Aplikasi akan memberi tahu apakah angka yang dimasukkan adalah bilangan prima.
- **Validasi Input**: Hanya angka yang bisa dimasukkan di `JTextField`.
- **JOptionPane untuk Error Handling**: Menampilkan pesan error jika input tidak valid atau kosong.
- **Auto-clear pada JTextField**: `JTextField` otomatis bersih saat mendapat fokus.

## Teknologi yang Digunakan

- **Java** (JDK 8 atau yang lebih baru)
- **Java Swing** untuk GUI

## Prasyarat

- **Java Development Kit (JDK)** versi 8 atau yang lebih baru
- **Apache NetBeans** atau IDE Java lainnya

#### Komponen GUI
- `JFrame`: Sebagai window utama aplikasi.
- `JPanel`: Untuk mengelompokkan komponen input dan tombol.
- `JTextField`: Untuk memasukkan angka yang akan dicek.
- `JButton`: Tombol "Cek" untuk memulai proses pengecekan.
- `JLabel`: Menampilkan hasil pengecekan.
- `JOptionPane`: Menampilkan pesan error jika input tidak valid.

#### Logika Program
- **Event Handling** menggunakan `ActionListener` untuk tombol dan `KeyAdapter` untuk membatasi input hanya angka.
- **Cek Genap/Ganjil** menggunakan operator modulus (`%`).
- **Cek Bilangan Prima** menggunakan loop untuk memeriksa apakah angka hanya memiliki dua faktor.
- **FocusListener** untuk menghapus input pada `JTextField` saat mendapat fokus.

## Cara Kerja

1. Pengguna memasukkan angka di `JTextField`.
2. Pengguna mengklik tombol **Cek** untuk melihat hasilnya.
3. Aplikasi memvalidasi input, lalu:
   - Menampilkan apakah angka tersebut **Genap** atau **Ganjil**.
   - Menambahkan informasi apakah angka tersebut adalah **Bilangan Prima** jika berlaku.
4. Jika input tidak valid, aplikasi akan menampilkan pesan error menggunakan `JOptionPane`.

## Contoh Penggunaan

| Input | Output                                |
|-------|---------------------------------------|
| 2     | Angka 2 adalah Genap (Bilangan Prima) |
| 3     | Angka 3 adalah Ganjil (Bilangan Prima)|
| 4     | Angka 4 adalah Genap                  |
| 9     | Angka 9 adalah Ganjil                 |
| 13    | Angka 13 adalah Ganjil (Bilangan Prima)|
