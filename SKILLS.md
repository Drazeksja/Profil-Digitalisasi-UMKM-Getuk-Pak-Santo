# SKILLS.md — Panduan Teknis & Pemeliharaan Website Getuk Berkah Santoso

Dokumen ini untuk tim KKN berikutnya atau siapa pun yang perlu mengubah isi website tanpa latar belakang pemrograman mendalam.

## 1. Filosofi Teknis
Website ini dibangun sebagai **situs statis** (satu file HTML berisi HTML + CSS + JavaScript ringan): tidak ada database, tidak ada sistem login, tidak ada panel admin. Pendekatan ini dipilih karena:
- Pak Santo tidak terbiasa mengelola teknologi digital sehari-hari.
- Situs statis lebih ringan, cepat diakses, dan minim risiko keamanan siber karena tidak ada sistem yang perlu diperbarui.
- Biaya hosting bisa ditekan di bawah Rp100.000/tahun memakai layanan hosting statis gratis (mis. GitHub Pages, Cloudflare Pages, Netlify) + domain murah.

## 2. Struktur Berkas
```
index.html   → seluruh halaman (struktur, gaya, dan skrip interaktif)
PRD.md       → dokumen kebutuhan produk
DESIGN.md    → sistem desain & alasan pilihan visual
SKILLS.md    → berkas ini
assets/      → folder berisi gambar dan foto (seperti foto getuk asli dan Bapak Santo)
```
Folder `assets/` menampung file-file eksternal yang dibutuhkan oleh halaman web. Pastikan folder ini turut diunggah (di-upload) bersamaan dengan `index.html` saat situs diterbitkan agar gambar dapat tampil dengan baik. Sebagian ilustrasi lainnya tetap menggunakan format SVG sebaris.

## 3. Cara Mengedit Konten
Semua teks dapat diedit langsung di `index.html` memakai aplikasi teks biasa (Notepad, VS Code, dll):

| Ingin mengubah | Cari di file |
|---|---|
| Nomor WhatsApp | cari `wa.me` — ganti angka setelah `wa.me/` |
| Alamat / jam buka | bagian `<section id="kontak">` |
| Menambah varian getuk baru | salin satu blok `<article class="menu-card">…</article>` di bagian `#menu`, ubah nama, warna ring (`--flavor`), dan deskripsi |
| Mengubah harga/promo | tambahkan teks bebas di dalam `menu-card`, situs ini sengaja tidak menampilkan harga tetap agar mudah menyesuaikan kondisi pasar |
| Menambah/mengedit program KKN | **Langkah 1:** Ubah teks/gambar pada kartu di bagian `<div class="kkn-grid">` (cari `#jejak-kkn`). Pastikan `href="#artikel/nama-slug"` terhubung dengan ID artikel.<br>**Langkah 2:** Edit/tambahkan konten lengkapnya di bagian `<div id="artikel-container">` yang terletak di bagian bawah file `index.html`. Pastikan `<article id="nama-slug">` sesuai dengan `href` pada kartu. |

## 4. Cara Deploy / Menerbitkan
1. Buat akun gratis di penyedia hosting statis (contoh: Cloudflare Pages, Netlify, atau GitHub Pages).
2. Unggah file `index.html` (cukup satu file).
3. Hubungkan domain murah (`.my.id`, `.web.id`, atau serupa) jika tersedia — biaya umumnya < Rp100.000/tahun.
4. Tidak perlu server tambahan, build step, atau instalasi paket apa pun.

## 5. SEO Dasar yang Sudah Disiapkan
- Tag `<title>` dan `<meta name="description">` sudah diisi sesuai identitas usaha.
- Struktur heading (`h1` → `h2` → `h3`) mengikuti urutan informasi yang logis.
- Disarankan didaftarkan ke Google Search Console & Google Business Profile agar muncul saat calon pembeli mencari "getuk Boyolali" atau "getuk Wonosegoro".

## 6. Batasan yang Disengaja
- **Tidak ada QRIS / pembayaran online** — berdasarkan riset lapangan, mitra pedagang keliling kurang setuju dengan sistem ini; pemesanan diarahkan lewat WhatsApp.
- **Tidak ada login admin** — mencegah kompleksitas yang tidak dibutuhkan pemilik usaha.
- **Sebagian besar ilustrasi vektor** — untuk menghemat bandwidth dan storage, meski kini situs juga memanfaatkan folder `assets/` untuk memuat foto riil yang lebih menarik, menggantikan beberapa SVG sebelumnya.

## 7. Perawatan Jangka Panjang
Karena tanpa database, "perawatan" hanya berarti mengedit teks di `index.html` sesekali (mis. saat ada varian baru atau perubahan jam buka), lalu mengunggah ulang file ke hosting. Tidak ada pembaruan sistem/keamanan rutin yang wajib dilakukan.
