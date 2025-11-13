# Praktikum7

Project Modul 7 - Navigasi Antar Halaman (Routing)

📖 Deskripsi

Project ini adalah langkah penting di mana Anda akan beralih dari aplikasi satu halaman ke aplikasi multi-halaman. Fokusnya adalah mempelajari cara berpindah (navigasi) antar halaman atau screen yang berbeda.

Meskipun modul ini mengenalkan MaterialPageRoute (navigasi dasar), tugas utama project ini berfokus pada implementasi Named Routes (navigasi menggunakan nama/rute terdaftar), yang merupakan cara yang lebih terorganisir untuk mengelola perpindahan halaman.

🎯 Tujuan Utama Project

Memahami Konsep: Mengerti konsep stack navigasi (routing) di Flutter, di mana halaman ditumpuk di atas satu sama lain.

Mendaftarkan Rute: Mampu mendaftarkan halaman-halaman aplikasi menggunakan properti routes di MaterialApp.

Navigasi Maju: Mengimplementasikan perpindahan halaman ke depan (maju) menggunakan Navigator.pushNamed().

Navigasi Mundur: Mengimplementasikan perpindahan halaman kembali (mundur/pop) menggunakan Navigator.pop().

Membuat Aplikasi Multi-halaman: Membuat aplikasi sederhana dengan dua halaman yang saling terhubung.

✅ Daftar Tugas (To-Do List)

Berikut adalah hal-hal yang harus Anda kerjakan berdasarkan modul:

Buat Project Baru:

[ ] Buat "New Flutter Project" (misalnya dengan nama navigation_named_route).

Buat File Halaman:

[ ] Buat file baru, home.dart, untuk berisi widget HalamanUtama.

[ ] Buat file baru, tujuan.dart, untuk berisi widget HalamanTujuan.

Konfigurasi main.dart (File Utama):

[ ] import kedua file (home.dart dan tujuan.dart).

[ ] Di dalam MaterialApp, atur properti initialRoute ke /.

[ ] Definisikan properti routes. Ini adalah Map yang memetakan nama rute ke widget halaman:

routes: {
  '/': (context) => HalamanUtama(),
  '/tujuan': (context) => HalamanTujuan(),
},


Kode Halaman Utama (home.dart):

[ ] Buat StatelessWidget bernama HalamanUtama.

[ ] Di dalam Scaffold, tambahkan sebuah tombol (misal: ElevatedButton).

[ ] Beri teks pada tombol, contoh: "Pindah ke Halaman Tujuan".

[ ] Di dalam onPressed tombol tersebut, panggil fungsi:
Navigator.pushNamed(context, '/tujuan');

Kode Halaman Tujuan (tujuan.dart):

[ ] Buat StatelessWidget bernama HalamanTujuan.

[ ] Di dalam Scaffold, tambahkan sebuah tombol (misal: ElevatedButton).

[ ] Beri teks pada tombol, contoh: "Kembali ke Halaman Utama".

[ ] Di dalam onPressed tombol tersebut, panggil fungsi:
Navigator.pop(context);
