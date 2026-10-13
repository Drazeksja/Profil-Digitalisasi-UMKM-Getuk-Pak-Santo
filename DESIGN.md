# DESIGN.md — Sistem Desain Website Getuk Berkah Santoso

Referensi visual: mockup "HieuBowl" (food-bowl landing page). Struktur, komposisi, dan bahasa visual mockup direplikasi seakurat mungkin, dengan konten & warna diselaraskan ke identitas Getuk Berkah Santoso (getuk singkong tradisional Boyolali).

## 1. Palet Warna

| Token | Hex | Penggunaan |
|---|---|---|
| `--bg-hero` | `#DCEEF7` | Latar hero (biru muda, sama seperti referensi) |
| `--cream` | `#FBF6EC` | Latar bagian putih/alternatif |
| `--purple` | `#6C5FC7` | Judul script, aksen lingkaran, band "Proses Pembuatan" |
| `--purple-dark` | `#4F45A8` | Latar band ungu tua, hover state |
| `--red` | `#B23A2E` | Tombol CTA utama (mengikuti tombol merah referensi) |
| `--red-dark` | `#8F2C22` | Hover tombol CTA |
| `--yellow` | `#EFC244` | Lingkaran aksen di bagian "Tentang" |
| `--green` | `#5F8A4B` | Aksen varian Pandan, daun dekoratif |
| `--ink` | `#231B36` | Warna teks utama (ungu gelap kehitaman) |
| `--ink-soft` | `#5C5470` | Teks sekunder/paragraf |

## 2. Tipografi

- **Display/Script** — `Caveat` (Google Fonts): dipakai untuk kata kunci besar bergaya tulisan tangan, meniru kata "Rice" pada referensi → dipakai pada "Getuk", "Berkah Santoso".
- **Heading** — `Poppins` 600–700: judul section, nama produk, nav.
- **Body** — `Poppins` 400–500: paragraf, deskripsi, tombol.

Skala: H1 56–64px / H2 36px / H3 22px / Body 16px / Caption 13px. Line-height longgar (1.5–1.6) untuk paragraf, ketat (1.1) untuk display script.

## 3. Layout per Section (mengikuti urutan mockup referensi)

```
┌───────────────────────────────────────────┐
│ NAV: logo | menu | (mobile: hamburger)     │
├───────────────────────────────────────────┤
│ HERO (bg biru muda)                        │
│  kiri: script "Getuk" + subjudul + CTA     │
│  kanan: ilustrasi bundar bowl + daun       │
│  bawah: pita "PILIH VARIAN ▾"              │
├───────────────────────────────────────────┤
│ TENTANG (bg putih)                         │
│  kiri: ilustrasi bowl + lingkaran kuning   │
│  kanan: "Tentang" + script nama usaha      │
│         + paragraf + CTA merah             │
├───────────────────────────────────────────┤
│ PROSES PEMBUATAN (bg ungu tua)             │
│  grid 8 langkah bernomor (numbering sah    │
│  karena memang proses berurutan)           │
├───────────────────────────────────────────┤
│ VARIAN GETUK (bg putih)                    │
│  4 kartu bundar: Original/Coklat/          │
│  Stroberi/Pandan — ring warna sesuai rasa  │
├───────────────────────────────────────────┤
│ KEUNGGULAN (bg krem) — 3 kolom ikon        │
├───────────────────────────────────────────┤
│ TESTIMONI (bg putih, mengikuti pola        │
│  "Our Happy Customers" pada referensi)     │
├───────────────────────────────────────────┤
│ JEJAK KKN (bg krem) — 5 kartu program      │
├───────────────────────────────────────────┤
│ CTA PESAN (bg ungu tua, seperti pita       │
│  "Ready to get started?" pada referensi)   │
├───────────────────────────────────────────┤
│ FOOTER (bg putih/krem, 3 kolom + copyright)│
└───────────────────────────────────────────┘
```

## 4. Komponen

- **Tombol utama**: latar `--red`, teks putih, radius penuh (pill), padding 14px 32px, huruf kapital kecil dengan letter-spacing — meniru tombol "VIEW OUR MENU" pada referensi.
- **Lingkaran dekoratif**: elemen `border-radius:50%` besar di belakang ilustrasi bowl (ungu di hero, kuning di Tentang) — signature visual yang direplikasi langsung dari mockup.
- **Kartu varian bundar**: bowl SVG di dalam lingkaran dengan ring warna tipis sesuai rasa (coklat/pink/hijau/krem), nama varian + tombol "Pesan" di bawahnya, sama seperti 3 kartu menu bundar pada referensi.
- **Pita label**: tombol kecil rounded dengan ikon, seperti "COUNTING CALORIES" pada referensi → diganti "VARIAN GETUK ▾".
- **Daun/ilustrasi dekoratif**: elemen SVG daun singkong melayang di sudut hero & CTA, menggantikan daun mint pada referensi — tetap mempertahankan posisi & fungsi dekoratif yang sama.

## 5. Ilustrasi & Citra
Karena tidak tersedia foto asli produk, semua visual bowl/produk dibuat sebagai **ilustrasi SVG orisinal** (bukan reproduksi foto/desain pihak lain), memakai palet warna makanan getuk (cokelat singkong, cokelat, pink stroberi, hijau pandan) dan komposisi tampak-atas (top-down) seperti pada referensi.

## 6. Signature Element
Lingkaran ganda (ungu di hero, kuning di Tentang) yang menaungi ilustrasi bowl tampak-atas — elemen paling khas dari mockup referensi — dipertahankan sebagai identitas visual utama situs ini, konsisten di seluruh section yang menampilkan produk.

## 7. Responsif
- **Desktop (>1024px)**: layout 2 kolom di hero & tentang, grid 4 kolom di varian, grid 4 kolom di proses.
- **Tablet (768–1024px)**: grid menyesuaikan jadi 2 kolom.
- **Mobile (<768px)**: seluruh section jadi 1 kolom, nav berubah jadi hamburger menu, ilustrasi diletakkan di atas teks.

## 8. Aksesibilitas
- Kontras teks ungu tua (`--ink`) di atas latar terang memenuhi rasio AA.
- Semua tombol punya focus state terlihat (outline 2px `--purple`).
- Animasi scroll-reveal ringan, dihormati `prefers-reduced-motion`.
