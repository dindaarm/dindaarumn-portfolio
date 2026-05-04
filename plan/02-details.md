# Fase 2: Detail dan Perencanaan

## Struktur Halaman (Arsitektur Informasi)
- `<nav>`: Menu navigasi lengket (*sticky*) dengan tautan ke tiap bagian.
- `<header id="home">`: Judul utama, perkenalan, tombol *Call-to-Action* (CTA), dan foto profil dengan dekorasi *badge* mengambang.
- `<section id="about">`: Penjelasan deskriptif mengenai fokus kerja dan *skill tags* (Python, SQL, Tableau, dll).
- `<section id="projects">`: Sistem *grid* responsif berisi kartu-kartu proyek.
- `<section id="contact">`: Layout terbagi dua (*split-layout*) untuk teks ajakan dan formulir input.

## Panduan Visual (*Style Guide*)
- **Tipografi**: Menggunakan `Inter` dari Google Fonts untuk kesan antarmuka yang bersih dan mudah dibaca (pembobotan: 300, 400, 500, 600, 700).
- **Warna Latar Belakang Utama**: `#0f172a` (Slate 900)
- **Warna Teks Utama**: `#f8fafc` (Slate 50)
- **Warna Aksen / Gradien Utama**: `linear-gradient(135deg, #3b82f6 0%, #60a5fa 100%)`
- **Efek Glassmorphism**: `background: rgba(30, 41, 59, 0.5); backdrop-filter: blur(12px); border: 1px solid rgba(255, 255, 255, 0.1);`

## Perencanaan Interaksi
1. Navigasi: Menempel di atas layar, latar belakangnya berubah menjadi *glassmorphism* saat pengguna melakukan *scroll*.
2. Animasi Muncul (*Reveal*): Konten pada bagian About, Projects, dan Contact awalnya akan berstatus tak terlihat (*opacity: 0*) dan bergeser ke bawah. Saat di-*scroll* dan masuk ke jangkauan pandangan, elemen tersebut akan muncul (*fade in up*).
