# Fase 3: Eksekusi dan Implementasi

Pembuatan *landing page* dilakukan menggunakan bahasa inti web tanpa kerangka kerja (*framework*) atau pustaka eksternal pihak ketiga (seperti Bootstrap atau Tailwind), guna membuktikan kontrol penuh terhadap kode dan desain.

## Langkah 1: Struktur HTML (`index.html`)
- Menyiapkan elemen `<!DOCTYPE html>` dan pengaturan *meta viewport* untuk responsivitas.
- Mengimpor font 'Inter'.
- Membangun struktur semantik (menggunakan tag `<nav>`, `<section>`, `<footer>`).
- Menyisipkan aset foto sementara dari Unsplash dan menyiapkan struktur penampungnya.

## Langkah 2: Pemberian Gaya dengan CSS (`styles.css`)
- Mendeklarasikan CSS Variables (`:root`) untuk mempermudah pengaturan dan perubahan tema (di kemudian hari diubah menjadi *Dark Mode*).
- Membuat sistem *Grid* dan *Flexbox* untuk mengatur letak konten (*layouting*), memastikan desain tetap rapi baik pada layar *desktop* (1200px) maupun layar *mobile* (di bawah 768px).
- Menuliskan kelas-kelas utilitas untuk animasi (*keyframes float*, *fadeInUp*, dan transisi *.reveal*).

## Langkah 3: Interaktivitas JavaScript (`script.js`)
- Menggunakan event listener `DOMContentLoaded` untuk memastikan skrip berjalan setelah HTML siap.
- **Sticky Navbar**: Memanfaatkan objek `window.scrollY` untuk menambahkan kelas `.scrolled` pada navbar jika layar digulir lebih dari 50px.
- **Scroll Reveal**: Mengimplementasikan `IntersectionObserver` API. Pendekatan ini jauh lebih hemat performa (*performant*) daripada menggunakan event *onscroll* tradisional untuk mendeteksi visibilitas elemen.
- **Formulir**: Menambahkan simulasi fungsional menggunakan `setTimeout` untuk mengubah status tombol "Kirim" menjadi "Mengirim..." lalu "Berhasil", guna memberikan *User Experience* (UX) yang nyata.
