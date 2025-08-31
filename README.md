# Romantic Galaxy Sakura (Static Site)

Satu halaman `index.html` bertema galaxy+sakura: surat cinta, janji, efek sakura, galeri 3D, countdown anniversary, musik.

## Struktur
```
romantis_galaxy_sakura/
├─ index.html
├─ .nojekyll
├─ audio/
│  └─ lagu.mp3
└─ galeri/
   ├─ 01.jpg ... 08.jpg
   └─ index.json
```

## Deploy ke GitHub Pages (tanpa build)
1. Buat repository baru, misal `romantis-galaxy-sakura`.
2. Upload seluruh isi folder (index.html, .nojekyll, audio/, galeri/).
3. Buka **Settings → Pages**.
4. Di **Build and deployment**, pilih **Source: Deploy from a branch**.
5. Pilih **Branch: main** dan **/ (root)** → **Save**.
6. Tunggu sebentar, situs akan aktif di:
   `https://<username>.github.io/romantis-galaxy-sakura/`

> Jika ingin domain sendiri, tambahkan **Custom domain** di Settings → Pages dan buat DNS CNAME.

## Catatan
- Path relatif sudah digunakan (`galeri/...`, `audio/...`) jadi aman untuk GitHub Pages.
- Browser mungkin menolak autoplay musik; akan muncul overlay “Tap untuk Memulai”.
- Jika gambar tidak tampil otomatis, pastikan `galeri/index.json` ada. (File ini sudah disertakan.)
