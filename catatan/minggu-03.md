# Catatan Minggu 03: Inheritance

## Yang saya kerjakan
Ada 3 Subclass yang saya isi pada minggu ini dari `Aset`, `Ruang`, `Labtop`, `AlatLab`.Di setiap konstruktornya memanggil  `super(kode, nama)`, lalu memvalidasikan fieldnya: kapasitas harus > 0, spesifikasi dan nomor pada variable inventaris tidak boleh kosong, laboratorium , dan juga tingkat risiko. Juga meng-Override `getJenis()` dan mengembalikan nilai enum `jenisAset` yang sesuai hingga semua  `minggu03HierarkiTest` berhasil.

## Keputusan desain
Field yang dipakai semua jenis aset (kode, nama) saya taruh di Aset supaya tidak ditulis ulang. Field yang hanya relevan untuk satu jenis saya taruh di subclass: kapasitas di Ruang, spesifikasi dan nomorInventaris di Laptop, laboratorium dan tingkatRisiko di AlatLab. Validasi khusus tiap subclass saya taruh di konstruktornya masing-masing, setelah super(kode, nama), sehingga validasi dari Aset tetap berjalan.

## Kendala
Pada bagian code saya masih cukup bingung mengisinya, masih banyak kesalahan syntax sebelum semua hasil yang saya kerjakan benar.

## Penggunaan AI
- Alat yang dipakai: Claude, Co pilot
- Bagian yang dibantu AI: Saya meminta ai untuk menjelaskan apa yang saya kerjakan pada minggu 3, dan juga ai membantu saya membuat code dan juga membenarkan code.
- Prompt utama: 
1. Ini di suruh apa? dan penjelasanya seperti apa?
2. Ini pada bagian catatan saya cukup bingung bisa jelaskan?
3. Bantu Saya menyelesaikan code ini.
- Yang saya ubah atau tolak dari saran AI, dan alasannya: Tidak ada yang saya tolak
- Satu hal yang saya pahami lebih baik sekarang: Konstruktor subclass harus memanggil `super(kode, nama.)` supaya validasi induk tetap berlaku, dan sebuah field hanya ditaruh di induk kalau dipakai oleh semua subclass.
