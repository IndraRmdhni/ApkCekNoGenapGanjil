## Logika Program

Aplikasi ini menggunakan beberapa logika dasar dalam Java untuk memeriksa input angka yang diberikan pengguna. Berikut ini adalah elemen utama dari logika program:

1. **Pengecekan Genap/Ganjil dengan Kondisional (if-else)**
   - Program mengecek apakah angka yang dimasukkan habis dibagi 2:
     ```java
     if (angka % 2 == 0) {
         // Jika angka genap
     } else {
         // Jika angka ganjil
     }
     ```

2. **Validasi Input**
   - Menggunakan `try-catch` untuk memastikan bahwa input yang dimasukkan adalah angka. Jika bukan angka, maka `NumberFormatException` akan ditangkap dan pesan kesalahan akan ditampilkan menggunakan `JOptionPane`:
     ```java
     try {
         int angka = Integer.parseInt(input);
         // Lanjutkan pengecekan genap/ganjil
     } catch (NumberFormatException e) {
         JOptionPane.showMessageDialog(this, "Masukkan hanya angka!", "Error", JOptionPane.ERROR_MESSAGE);
     }
     ```

3. **Penggunaan JOptionPane**
   - `JOptionPane` digunakan untuk menampilkan pesan kesalahan ketika input tidak valid. Selain itu, bisa juga digunakan untuk menampilkan hasil:
     ```java
     JOptionPane.showMessageDialog(this, "Angka " + angka + " adalah Genap");  // Untuk angka genap
     JOptionPane.showMessageDialog(this, "Angka " + angka + " adalah Ganjil");  // Untuk angka ganjil
     ```
