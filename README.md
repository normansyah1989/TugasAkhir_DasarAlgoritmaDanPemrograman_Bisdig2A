📘 User Manual – Aplikasi Inventori Toko Bahan Kue
1. Deskripsi Program
Aplikasi ini merupakan program berbasis Python yang digunakan untuk mengelola data bahan baku pada toko kue secara sederhana. Pengguna dapat menambahkan, melihat, mengedit, menghapus, dan menampilkan laporan stok bahan seperti tepung, gula, telur, mentega, dan lainnya.
Semua data disimpan secara permanen dalam file bahan_kue.json.

2. Persyaratan Sistem
Python versi 3.6 atau lebih tinggi

Dapat dijalankan melalui:

VS Code / Terminal (Windows/Linux/macOS)

Google Colab (langsung di browser)

3. Struktur File
Nama File	Keterangan
bahan_kue.py	File utama berisi kode program inventori
bahan_kue.json	File tempat penyimpanan data bahan kue
user_manual.md	Dokumentasi penggunaan program

4. Cara Menjalankan Program
🔹 Di VS Code / Terminal

Pastikan Python sudah terinstall.

Buka terminal atau command prompt.

Jalankan perintah:

bash
Salin
Edit
python bahan_kue.py
🔹 Di Google Colab

Upload file bahan_kue.py ke Google Colab.

Jalankan sel untuk mengeksekusi program.

File bahan_kue.json akan otomatis dibuat di direktori kerja.

5. Panduan Menu Program
Saat program dijalankan, pengguna akan melihat menu berikut:

markdown
Salin
Edit
=== Menu Inventori Bahan Kue ===
1. Tambah Bahan
2. Lihat Semua Bahan
3. Edit Stok Bahan
4. Hapus Bahan
5. Laporan Stok
6. Simpan & Keluar
No	Menu	Deskripsi
1	Tambah Bahan	Menambahkan bahan baru (kode, nama, stok). Kode tidak boleh duplikat.
2	Lihat Semua	Menampilkan semua data bahan dan stok saat ini.
3	Edit Stok	Mengubah jumlah stok berdasarkan kode bahan.
4	Hapus Bahan	Menghapus bahan dari daftar berdasarkan kode.
5	Laporan Stok	Menampilkan laporan stok dari jumlah terbanyak ke yang paling sedikit.
6	Simpan & Keluar	Menyimpan data ke file JSON dan keluar dari aplikasi.

6. Format Input
Field	Format	Contoh
Kode Bahan	String tanpa spasi	BHN001
Nama Bahan	String bebas	Tepung Terigu
Jumlah Stok	Angka bulat positif (gram)	500

7. Fitur Optimasi & Penanganan Error
✅ File Handling menggunakan with open dan error handling try-except
✅ Pengukuran performa dengan time.time() untuk melihat waktu eksekusi fungsi
✅ Komentar kode lengkap agar mudah dipelajari dan dikembangkan
✅ Validasi kode bahan unik saat menambahkan bahan baru
✅ Struktur data fleksibel (list of dictionary) – dapat dikembangkan jadi dict indexing
✅ Program tetap berjalan meski file JSON belum ada

8. Catatan Tambahan
File bahan_kue.json akan otomatis diperbarui saat memilih menu "Simpan & Keluar".

Jangan mengedit file JSON secara manual, agar struktur data tetap konsisten.

Jika program dijalankan untuk pertama kali dan file JSON belum tersedia, maka data akan dimulai dari kosong.

Data stok disimpan dalam satuan gram agar sesuai dengan kebutuhan toko bahan kue.

💡 Saran Pengembangan (Opsional)
Gunakan struktur dictionary dengan indexing kode bahan untuk pencarian lebih cepat (O(1)).

Tambahkan validasi angka positif pada input stok.

Buat fitur ekspor laporan stok ke file .txt atau .csv.

Tambahkan fitur kategori bahan (misal: kering, cair, basah).
