# Website Disporapar Kalimantan Barat (multi-page)

Situs statis: setiap halaman adalah file HTML sendiri, memakai CSS dan JavaScript bersama.
Cocok untuk GitHub Pages (tanpa build, tanpa server).

## Struktur
```
index.html                  Beranda (hero, kalender event, destinasi populer)
tentang.html                Tentang
wilayah.html                Daftar kota dan kabupaten
wilayah-detail.html?w=      Destinasi per wilayah        (contoh: ?w=sintang)
jelajahi.html[?k=]          Telusuri semua destinasi     (contoh: ?k=hotel)
destinasi.html?id=          Detail destinasi             (contoh: ?id=danau-sentarum)
event.html?id=              Detail event
kontak.html                 Kontak
login.html / daftar.html    Akun pengguna / admin
bookmark.html               Bookmark pengguna
rencana.html                Rencana perjalanan pengguna
admin.html                  Dashboard admin
admin-destinasi.html        Kelola destinasi
admin-destinasi-form.html   Tambah / edit destinasi      (edit: ?id=)
admin-event.html            Kelola event
admin-event-form.html       Tambah / edit event          (edit: ?id=)
404.html                    Halaman tidak ditemukan
assets/css/style.css        Gaya bersama
assets/js/app.js            Logika bersama (render, akun, bookmark, rencana, kalender, admin)
assets/img/                 Logo dan favicon
images/                     Foto (lihat PANDUAN-GAMBAR.md)
```

## Memasang di GitHub Pages
1. Hapus `index.html` lama di repo (versi satu halaman).
2. Unggah **seluruh isi** folder ini ke root repo (semua file `.html`, folder `assets` dan `images`).
3. Settings → Pages → Deploy from a branch → `main` / root. Tunggu 1–2 menit.

Tautan lama berbentuk `index.html#d-danau-sentarum` otomatis dialihkan ke `destinasi.html?id=danau-sentarum`.

## Menjalankan di komputer
Jangan buka lewat `file://`; jalankan server sederhana di folder ini:
`python3 -m http.server 8000` lalu buka `http://localhost:8000`.

## Catatan
- Akun, bookmark, rencana, event, dan perubahan destinasi tersimpan di browser (localStorage), belum dibagikan antar pengunjung.
- Sesi admin berlaku selama tab dibuka (sessionStorage). Login admin saat ini hanya demo.
- Untuk data bersama dan login yang aman diperlukan backend (mis. Supabase atau Firebase).
