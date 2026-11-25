# Panduan Gambar Website Disporapar

Gambar diambil otomatis dari folder `images/` di repository GitHub. Nama file BEBAS
(tidak perlu diganti dan boleh acak dari kamera). Yang menentukan gambar itu milik siapa
adalah FOLDER tempat file diunggah.

## Foto destinasi
Folder: `images/destinasi/<id-destinasi>/`

`<id-destinasi>` = nama destinasi huruf kecil, spasi jadi tanda hubung.
Contoh: "Danau Sentarum" -> `images/destinasi/danau-sentarum/`

Cara termudah: buka Admin -> Edit/Tambah destinasi -> klik "Buka halaman unggah folder ini".
GitHub akan terbuka langsung di folder yang tepat. Seret semua foto, lalu Commit.

Aturan otomatis di dalam folder:
- `profil.jpg` (jika ada) = Foto Profil (lingkaran di header detail)
- `latar.jpg` (jika ada) = Foto Background (header detail dan sampul card)
- Foto lainnya (nama apa saja) = Foto Galeri, diurutkan menurut nama
- Jika tidak ada `latar.jpg`, foto pertama dipakai sebagai background/sampul

Foto yang diunggah ke folder Danau Sentarum hanya tampil di Danau Sentarum.

## Foto card Wilayah
Folder: `images/wilayah/` dengan nama file = nama wilayah huruf kecil, spasi jadi tanda hubung.
Contoh: `bengkayang.jpg`, `kapuas-hulu.jpg`, `kayong-utara.jpg`, `ketapang.jpg`, `melawi.jpg`,
`mempawah.jpg`, `sambas.jpg`, `sanggau.jpg`, `singkawang.jpg`, `sintang.jpg`.
Wilayah yang belum punya foto (Pontianak, Landak, Sekadau, Kubu Raya) tetap memakai warna bawaan.
Untuk menambah, cukup unggah file dengan nama wilayahnya, misalnya `landak.jpg`.

## Foto halaman Tentang
Folder: `images/tentang/`
- `pesona.jpg` = foto bagian "Pesona Pariwisata & Kekayaan Budaya"
- `pembinaan.jpg` = foto bagian "Pembinaan Pemuda & Prestasi Olahraga" (foto vertikal)

## Foto event
Folder: `images/event/` dengan nama file = id event (judul huruf kecil, spasi jadi tanda hubung).
Contoh: event "Festival Uji Coba" memakai `images/event/festival-uji-coba.jpg` sebagai foto sampul halaman event.
Jika tidak ada foto, area sampul disembunyikan.

## Foto default
Jika sebuah destinasi belum punya foto, situs memakai:
- `images/default/profil.jpg` (1:1) sebagai Foto Profil
- `images/default/latar.jpg` (lebar) sebagai Foto Background dan sampul card
Foto default hanya dipakai jika folder destinasi tidak punya foto profil/latar/galeri sendiri.

## Carousel Beranda
Folder: `images/hero/` (nama file bebas, maksimal 12 foto).
File lama `images/hero-1.jpg`, `hero-2.jpg`, dst. tetap terbaca.
Tombol unggah ada di halaman Admin (bagian "Foto carousel Beranda").

## Catatan
- Setelah commit, GitHub Pages butuh sekitar 1-2 menit sebelum foto tampil.
- Daftar file di-cache 5 menit di browser. Muat ulang (Ctrl+F5) jika foto baru belum muncul.
- Format: jpg, jpeg, png, webp, avif, gif. Usahakan lebar sekitar 1400 px dan di bawah 300 KB.
- Hindari tanda kutip di nama file; spasi diperbolehkan.
