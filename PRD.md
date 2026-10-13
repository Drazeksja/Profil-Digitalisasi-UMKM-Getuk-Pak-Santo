# PRD — Website Getuk Berkah Santoso

## 1. Latar Belakang
Getuk Berkah Santoso adalah UMKM getuk lindri tradisional milik Bapak Santo (Kuntet) di Dukuh Bojong, Desa Bojong, Kecamatan Wonosegoro, Kabupaten Boyolali, yang telah berproduksi sejak era 1980-an dan berjalan mandiri sejak ±4 tahun terakhir. Usaha ini memproduksi 4.000–5.000 biji getuk/hari dari 150 kg singkong, didistribusikan lewat 6–7 pedagang keliling setiap pukul 02.00–04.00 WIB.

Sebagai bagian dari Program Kerja Multidisiplin KKN Tim II UNDIP 2026, mahasiswa membangun jejak digital resmi bagi usaha ini karena mayoritas pelanggan adalah lansia yang tidak memakai media sosial, sementara pemilik usaha ingin memperluas pasar tanpa harus mengelola platform yang rumit sehari-hari.

## 2. Tujuan Produk
- Menyediakan profil usaha yang profesional, mudah ditemukan di Google (SEO lokal), dan dapat diakses tanpa memerlukan pengelolaan aktif dari Pak Santo.
- Menampilkan cerita, proses produksi, keunggulan, dan varian produk Getuk Berkah Santoso secara jujur dan sesuai kondisi lapangan (bukan klaim berlebihan).
- Menjadi kanal pemesanan/kontak sederhana lewat WhatsApp — tanpa fitur pembayaran digital (QRIS ditolak mitra pedagang di lapangan, lihat catatan riset).
- Menjadi wadah publikasi "Jejak KKN": ringkasan program legalitas usaha, hygiene produksi, efisiensi dapur, administrasi logistik, dan promosi digital yang dijalankan tim multidisiplin.

## 3. Target Pengguna
| Persona | Kebutuhan |
|---|---|
| Calon pembeli baru / warga luar desa | Info produk, rasa, cara pesan, lokasi, jam buka |
| Mitra distribusi / pedagang gerobak | Info kontak & jadwal pengambilan produk |
| Pemangku kepentingan desa / instansi | Bukti legalitas, program pemberdayaan, dampak SDGs |
| Tim KKN berikutnya | Referensi konten & histori program yang sudah berjalan |

## 4. Ruang Lingkup (In Scope)
1. **Beranda/Hero** — perkenalan merek "Getuk Berkah Santoso, Getuk Lindri Asli Boyolali sejak 1980-an".
2. **Tentang Kami** — sejarah singkat usaha, sosok Pak Santo, lokasi & filosofi.
3. **Proses Pembuatan** — 8 tahapan produksi getuk (dari pengupasan singkong hingga hasil akhir).
4. **Varian Produk** — 4 varian: Original, Coklat, Stroberi, Pandan.
5. **Keunggulan** — 100% singkong asli, pengolahan tradisional, alami tanpa pengawet.
6. **Testimoni Pelanggan**
7. **Jejak KKN & Artikel Detail** — Grid 11 program kerja multidisiplin KKN (legalitas, cuci tangan, digital marketing, dll). Masing-masing kartu dapat diklik untuk membuka tampilan artikel berita lengkap tanpa memuat halaman baru (menggunakan *hash routing* `index.html#artikel/...`).
8. **Kontak & Ajakan Pesan** — nomor WhatsApp, alamat, jam operasional, tautan lokasi.
9. **Footer** — ringkasan tautan, kontak, hak cipta.

## 5. Di Luar Ruang Lingkup (Out of Scope)
- Sistem pembayaran online / QRIS (ditolak oleh mitra pedagang berdasarkan riset lapangan).
- Login/akun pengguna, dashboard admin, atau CMS berbasis database.
- Pemesanan otomatis dengan keranjang belanja — cukup arahkan ke WhatsApp.

## 6. Kebutuhan Konten (sumber: NOTUL.pdf)
Seluruh konten teks diambil & disederhanakan dari hasil wawancara dan artikel KKN Tim II UNDIP 2026 Desa Bojong (NOTUL.pdf), meliputi: sejarah usaha, visi-misi, proses produksi, keunggulan produk, varian produk, serta ringkasan lima program kerja pendukung (legalitas, hygiene, efisiensi dapur, administrasi logistik, promosi digital).

## 7. Kebutuhan Non-Fungsional
- **Tanpa perawatan lanjutan**: situs statis (HTML/CSS/JS), tidak butuh server, database, atau login admin — selaras dengan pendekatan *Static Site Generator* yang sudah diterapkan tim KKN di lapangan.
- **Ringan & cepat**: aset gambar berupa ilustrasi vektor (SVG) buatan sendiri, bukan foto berat.
- **Responsif**: nyaman diakses dari HP (mayoritas calon pembeli mengakses lewat ponsel).
- **SEO dasar**: meta title/description, struktur heading yang jelas, teks alt pada ilustrasi.
- **Aksesibel**: kontras warna cukup, navigasi bisa dipakai dengan keyboard.

## 8. Metrik Keberhasilan
- Situs dapat diakses & tampil benar di perangkat mobile dan desktop.
- Semua informasi kontak (WhatsApp, alamat, jam buka) akurat sesuai NOTUL.pdf.
- Tombol "Pesan via WhatsApp" berfungsi membuka chat langsung.
- Biaya hosting tahunan tetap di bawah Rp100.000 (mengikuti pendekatan hosting statis gratis yang sudah dipakai tim KKN).

## 9. Referensi Desain
Tata letak & gaya visual mengacu pada mockup "HieuBowl" yang diberikan pengguna (skema warna biru muda–ungu–merah, tipografi script pada judul, elemen lingkaran dekoratif, kartu menu berbentuk bundar). Detail lengkap ada di `DESIGN.md`.
