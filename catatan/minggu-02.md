# Catatan Minggu 02: Struktur OOP: Class, Object, Encapsulation

## Yang saya kerjakan
Minggu ini saya bikin class `Aset` yang field-nya semua private, lengkap dengan
konstruktor, getter, dan setter yang ada validasinya. 

## Keputusan desain
Untuk `kode`, saya tidak bikin setter sama sekali karena sesuai aturan tugas,
kode tidak boleh berubah setelah objek dibuat.

## Kendala
Saya bingung kenapa tes gagal waktu kode diisi cuma spasi, ternyata harus dicek pakai isBlank(), bukan cuma null. Dan saya juga harus belajar bahasa dan syntax java dengan lebih baik lagi karena saya masih bingung.

## Penggunaan AI
- Alat yang dipakai: Claude Ai
- Bagian yang dibantu AI: penjelasan konsep (class, object, encapsulation) dan
  pemahaman instruksi tugas. 
- Prompt utama:
  1. "pada minggu ini saya di suruh apa?"
  2. "coba jelaskan kepada saya tentang materi ini apa itu Class, Object, Encapsulation"
- Yang saya ubah atau tolak dari saran AI, dan alasannya: Tidak ada
- Satu hal yang saya pahami lebih baik sekarang: kenapa validasi ditaruh di dalam
  class (konstruktor dan setter), bukan di kode yang memakai class-nya. Dulu saya
  kira cukup dicek di tempat objeknya dipakai. Ternyata kalau begitu, setiap kali
  ada yang lupa ngecek, datanya bisa rusak (misalnya nama jadi null). Kalau
  validasinya ada di dalam class dan field-nya private, objek `Aset` tidak mungkin
  berada dalam keadaan tidak valid, siapa pun yang memakainya. Itu inti
  encapsulation yang baru saya sadari.