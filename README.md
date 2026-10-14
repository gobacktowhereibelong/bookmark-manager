# Bookmark Manager Personal

Ekstensi Chrome (Manifest V3) untuk mengelola bookmark dan menyimpan tab yang sedang terbuka. Halaman tab baru diganti dengan dashboard pribadi yang menyimpan data lewat API bookmark Chrome — tidak ada server, semua lokal di peramban.

## Fitur

- **Dashboard tab baru** — semua bookmark tampil dalam satu ruang kerja
- **Simpan semua tab** — sekali klik, seluruh tab di jendela aktif menjadi bookmark
- **Folder & subfolder** — koleksi bertingkat, bisa dibuat, di-rename inline, dipindah, dan dihapus
- **Pencarian, urutan & filter** — cari kata kunci, urutkan terbaru/terlama, filter per bulan
- **Deteksi duplikat** — pindai bookmark ganda (URL dan judul serupa) lalu hapus massal
- **Kustomisasi kartu** — judul tampilan khusus, warna background, gambar dari URL/file, dan pengaturan gelap
- **Wallpaper dashboard** — ganti background, atur tingkat gelap dan warna teks lewat tombol 🎨
- **Drag & drop** — pindahkan bookmark antar folder dengan menyeret
- **Pindah cepat** — dialog pindah ke folder lain dari menu kartu

## Instalasi (Load unpacked)

1. Buka `chrome://extensions`
2. Aktifkan **Developer mode** (pojok kanan atas)
3. Klik **Load unpacked** dan pilih folder proyek ini
4. Buka tab baru — dashboard Bookmark Manager akan muncul
5. Klik ikon ekstensi di toolbar untuk membuka dashboard dari tab mana pun

## Struktur file

| File | Fungsi |
| --- | --- |
| `manifest.json` | Konfigurasi ekstensi (MV3, izin `bookmarks` & `tabs`) |
| `dashboard.html` | Halaman dashboard dan dialog-dialog UI |
| `dashboard.js` | Seluruh logika bookmark, folder, tema, dan interaksi |
| `styles.css` | Gaya dashboard |
| `background.js` | Membuka dashboard saat ikon ekstensi diklik |

## Teknologi

- Chrome Extension Manifest V3
- `chrome.bookmarks` & `chrome.tabs` API
- HTML, CSS, JavaScript vanilla (tanpa framework, tanpa build step)

## Lisensi

Untuk penggunaan pribadi.
