# PDF Editor

Aplikasi web client-side untuk menggabungkan gambar dan PDF menjadi satu dokumen PDF, dengan kemampuan reorder, rotate, dan cetak booklet A5 di kertas A4. Semua proses berjalan di browser — tidak ada upload ke server.

## Cara pakai

1. Buka `index.html` langsung di browser (Chrome/Firefox/Safari), atau host via GitHub Pages.
2. Upload gambar dan/atau file PDF.
3. Atur urutan halaman lewat drag & drop di tab **Grid** atau **Reorder & Edit**.
4. Rotate halaman individual atau semua sekaligus jika perlu.
5. Export jadi satu file PDF, atau gunakan panel **Print Booklet** untuk menyusun ulang halaman ke format imposition A5 (saddle-stitch) siap cetak duplex manual di kertas A4.

## Fitur

- Upload banyak gambar (JPG/PNG/WEBP/GIF) sekaligus, otomatis diurutkan ascending berdasarkan nama file.
- Upload satu atau lebih file PDF — semua halaman diimpor sebagai halaman individual dengan preview thumbnail (via PDF.js).
- Drag & drop reorder, tombol naik/turun, dan input nomor halaman langsung.
- Rotate per halaman (90° increment) atau rotate semua sekaligus.
- Export ke PDF dengan pilihan ukuran halaman (A4, Letter, A3, atau ukuran asli), orientasi, dan margin.
- **Print Booklet**: hitung otomatis imposition saddle-stitch A5 di A4 — generate file PDF sisi depan dan sisi belakang terpisah untuk dicetak manual duplex, lalu dilipat & dijilid tengah (staples).

## Teknologi

- Vanilla HTML/CSS/JavaScript, tanpa build step.
- [pdf-lib](https://pdf-lib.js.org/) untuk membuat dan memanipulasi PDF.
- [PDF.js](https://mozilla.github.io/pdf.js/) untuk membaca dan merender preview PDF.
- Library dimuat dari CDN dengan fallback otomatis (cdnjs → unpkg → jsdelivr) jika salah satu sumber gagal.

## Lisensi

Bebas digunakan dan dimodifikasi.
