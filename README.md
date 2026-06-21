# Restauran Kuliner Indonesia

Project dummy landing page restoran multi-halaman, dibuat sebagai latihan penggunaan **Tailwind CSS (CLI)** dari nol — mencakup custom theme, komponen reusable, carousel, dan responsive design.

> ⚠️ Ini project dummy untuk portofolio, bukan project produksi untuk klien.

## Tentang Project

Dipakai buat latihan beberapa hal:
- Setup Tailwind CSS lewat CLI (bukan CDN/Play)
- Custom design token (`@theme`) — warna & font brand kustom
- Layout responsive multi-breakpoint (mobile, tablet, desktop)
- Integrasi Swiper.js untuk carousel testimoni
- Vanilla JavaScript (mobile menu, filter & search menu, active nav state)

## Tech Stack

- HTML5
- Tailwind CSS v4 (CLI)
- Swiper.js — carousel testimoni
- Vanilla JavaScript
- Google Fonts: **Mada** (sans) & **Philosopher** (serif)

## Struktur Folder

```
project/
├── src/
│   └── input.css          # Source Tailwind + custom theme (@theme)
├── dist/
│   └── output.css         # Hasil compile Tailwind (jangan edit manual)
├── assets/
│   └── images/             # Semua aset gambar
├── home.html
├── menu.html
├── about.html
├── contact.html
└── README.md
```

## Custom Theme

Warna & font brand didefinisikan di `src/input.css`:

| Token | Hex | Keterangan |
|---|---|---|
| `--color-brand-black` | `#1F160F` | Cokelat tua aristokrat |
| `--color-brand-gold` | `#CBA75C` | Emas kuliner |
| `--color-brand-white` | `#FFFFFF` | Putih bersih |
| `--color-brand-brown` | `#9B8370` | Cokelat kulit |
| `--color-brand-pale` | `#FAF4EC` | Krem pucat hangat |

| Token | Font | Penggunaan |
|---|---|---|
| `font-sans` | Mada | Teks konten |
| `font-serif` | Philosopher | Judul/heading mewah |

## Cara Menjalankan

1. Clone repo ini
   ```bash
   git clone <url-repo-ini>
   cd <nama-folder>
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Jalankan Tailwind CLI (watch mode) — wajib jalan tiap kali develop, biar class baru ke-compile
   ```bash
   npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
   ```

4. Buka `home.html` lewat Live Server (VS Code extension) atau server lokal lainnya

## Halaman

| File | Isi |
|---|---|
| `home.html` | Hero, preview menu, about, testimoni (Swiper), kontak, footer |
| `menu.html` | Daftar menu lengkap + filter kategori & search |
| `about.html` | Suasana restoran & profil tim chef |
| `contact.html` | Info kontak, jam operasional, lokasi (Google Maps) |

## Kontributor

- Yuwanda Aji Pangestu — *(Developer)*


## Lisensi

Project ini menggunakan [MIT License](./LICENSE).
