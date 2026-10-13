# Profil-Digitalisasi-UMKM-Getuk-Pak-Santo
Profil UMKM Getuk Berkah Santoso, usaha getuk lindri milik Pak Santo di Dukuh Bojong, Desa Bojong, Kecamatan Wonosegoro, Kabupaten Boyolali, yang telah berproduksi sejak 1980-an. Dibuat sebagai luaran Program Kerja Multidisiplin KKN Tim II UNDIP 2026 untuk membantu memperkenalkan usaha dan produk getuk lindri kepada masyarakat melalui internet.

# Website Getuk Berkah Santoso

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
</p>

Website profil UMKM Getuk Berkah Santoso, usaha getuk lindri milik Pak Santo di Dukuh Bojong, Desa Bojong, Kecamatan Wonosegoro, Kabupaten Boyolali. Website ini dikembangkan sebagai luaran Program Kerja Multidisiplin KKN Tim II UNDIP 2026 untuk memperkenalkan produk, sejarah usaha, dan kegiatan pendampingan UMKM kepada masyarakat melalui media digital.

---

## Daftar Isi

- [Fitur Utama](#fitur-utama)
- [Informasi Produk](#informasi-produk)
- [Teknologi yang Digunakan](#teknologi-yang-digunakan)
- [Instalasi dan Menjalankan Lokal](#instalasi-dan-menjalankan-lokal)
- [Struktur Proyek](#struktur-proyek)
- [Hosting dan Deployment](#hosting-dan-deployment)
- [Program Kerja Multidisiplin KKN](#program-kerja-multidisiplin-kkn)

---

## Fitur Utama

| Fitur | Deskripsi |
|---|---|
| Beranda | Pengenalan Getuk Berkah Santoso dengan identitas usaha dan informasi produk. |
| Tentang Kami | Menampilkan sejarah usaha, profil Pak Santo, dan lokasi produksi. |
| Proses Pembuatan | Menjelaskan tahapan pembuatan getuk lindri dari pengolahan singkong hingga produk siap dijual. |
| Varian Produk | Informasi empat varian getuk: Original, Coklat, Stroberi, dan Pandan. |
| Keunggulan Produk | Informasi mengenai bahan singkong, proses pengolahan tradisional, dan produk tanpa pengawet. |
| Testimoni | Menampilkan tanggapan pelanggan mengenai produk. |
| Jejak KKN | Dokumentasi 11 program kerja multidisiplin yang berkaitan dengan pendampingan UMKM. |
| Artikel Kegiatan | Menampilkan informasi lengkap setiap program kerja melalui navigasi berbasis hash tanpa memuat ulang halaman. |
| Kontak dan Lokasi | Informasi alamat usaha, jam operasional, lokasi, dan kontak pemesanan. |
| Pemesanan WhatsApp | Mengarahkan pengunjung ke WhatsApp untuk menghubungi pemilik usaha. |
| Desain Responsif | Menyesuaikan tampilan untuk perangkat mobile maupun desktop. |

**Karakteristik Website**

- Website statis tanpa backend dan database.
- Tidak memerlukan akun pengguna atau dashboard admin.
- Informasi usaha dapat diakses langsung melalui browser.
- Menggunakan ilustrasi SVG untuk mendukung tampilan website.
- Memiliki SEO dasar melalui metadata, struktur heading, dan teks alternatif gambar.
- Navigasi dirancang agar dapat digunakan melalui keyboard.

---

## Informasi Produk

Getuk Berkah Santoso merupakan usaha getuk lindri tradisional yang telah berproduksi sejak era 1980-an di Dukuh Bojong, Desa Bojong, Kecamatan Wonosegoro, Kabupaten Boyolali.

Informasi yang ditampilkan pada website meliputi:

- **Nama usaha:** Getuk Berkah Santoso.
- **Pemilik:** Bapak Santo (Kuntet).
- **Produk utama:** Getuk lindri tradisional.
- **Varian:** Original, Coklat, Stroberi, dan Pandan.
- **Lokasi:** Dukuh Bojong, Desa Bojong, Kecamatan Wonosegoro, Kabupaten Boyolali.

Website juga menjadi media dokumentasi kegiatan KKN yang mendukung pengembangan usaha, mulai dari promosi digital, kebersihan produksi, legalitas usaha, hingga administrasi dan efisiensi dapur.

---

## Teknologi yang Digunakan

| Komponen | Teknologi |
|---|---|
| Struktur halaman | HTML5 |
| Tampilan dan layout | CSS3 |
| Interaksi dan navigasi | JavaScript |
| Ilustrasi | SVG |
| Kontak pemesanan | WhatsApp |
| Routing artikel | Hash-based routing |
| Deployment | Hosting statis |

Website tidak menggunakan framework frontend, server backend, maupun database. Pendekatan ini dipilih agar website tetap ringan dan tidak membutuhkan pengelolaan sistem yang rumit untuk menampilkan informasi usaha.

---

## Instalasi dan Menjalankan Lokal

### 1. Clone Repository

```bash
git clone <URL-REPOSITORY>
cd <NAMA-REPOSITORY>
```

Ganti `<URL-REPOSITORY>` dan `<NAMA-REPOSITORY>` sesuai alamat repository GitHub.

### 2. Buka Proyek

Buka folder proyek menggunakan Visual Studio Code atau editor pilihanmu.

### 3. Jalankan Website

Website dapat dibuka langsung melalui file `index.html` di browser.

Untuk pengalaman pengembangan yang lebih nyaman, gunakan ekstensi Live Server pada Visual Studio Code, kemudian pilih **Open with Live Server**.

Tidak diperlukan instalasi dependensi melalui npm maupun konfigurasi database untuk menjalankan website.

---

## Struktur Proyek

Struktur berikut merupakan gambaran umum dan perlu disesuaikan dengan susunan file aktual repository.

```text
.
├── index.html
├── assets/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── script.js
│   └── images/
├── DESIGN.md
└── README.md
```

Keterangan:

- `index.html` — struktur halaman utama website.
- `assets/css/` — file stylesheet untuk layout, warna, tipografi, dan tampilan responsif.
- `assets/js/` — logika interaksi, navigasi artikel, dan fitur website.
- `assets/images/` — aset visual dan ilustrasi yang digunakan.
- `DESIGN.md` — dokumentasi referensi dan keputusan desain website.
- `README.md` — dokumentasi proyek dan panduan penggunaan.

---

## Hosting dan Deployment

Website dapat di-deploy menggunakan layanan hosting statis, seperti Vercel atau GitHub Pages, karena tidak memerlukan proses backend maupun database.

Langkah deployment secara umum:

1. Push repository ke GitHub.
2. Hubungkan repository dengan layanan hosting statis.
3. Atur direktori publik sesuai struktur proyek.
4. Jalankan deployment dan periksa tampilan website.
5. Pastikan tautan WhatsApp, alamat, navigasi artikel, dan tampilan mobile berfungsi dengan benar.

Penggunaan hosting statis memungkinkan website berjalan tanpa server aplikasi khusus. Apabila menggunakan domain khusus, perpanjangan domain tetap perlu diperhatikan sesuai layanan yang digunakan.

---

## Program Kerja Multidisiplin KKN

Website ini merupakan bagian dari Program Kerja Multidisiplin KKN Tim II UNDIP 2026 di Desa Bojong, Kecamatan Wonosegoro, Kabupaten Boyolali.

Selain memperkenalkan produk Getuk Berkah Santoso, website mendokumentasikan kegiatan pendampingan UMKM yang dilaksanakan oleh tim KKN. Dokumentasi tersebut mencakup program terkait legalitas usaha, kebersihan produksi, efisiensi dapur, administrasi logistik, dan promosi digital.

Website diharapkan dapat menjadi media informasi yang tetap dapat diakses setelah program KKN selesai serta menjadi dokumentasi kegiatan mahasiswa bersama mitra UMKM.

---

**Developed as part of KKN Tim II UNDIP 2026 — Desa Bojong, Boyolali.**
