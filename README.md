# Portofolio — Muhammad Fahri Fadillah

Website portofolio satu halaman (single-page) bertema dark/futuristik untuk Computer Engineering.
Dibuat dengan HTML, CSS, dan JavaScript murni — tanpa build step, tanpa dependency. Siap langsung di-deploy ke Vercel.

## Isi folder
```
portfolio/
├── index.html      ← seluruh website (HTML + CSS + JS dalam satu file)
├── vercel.json     ← konfigurasi Vercel (opsional, untuk clean URL)
└── README.md       ← panduan ini
```

## Cara Deploy ke Vercel

### Opsi A — Drag & Drop (paling cepat, tanpa GitHub)
1. Buka https://vercel.com lalu login (bisa pakai akun GitHub/Google).
2. Klik **Add New… → Project**.
3. Pilih opsi untuk upload folder, atau cukup **seret folder `portfolio` ini** ke area upload.
4. Vercel otomatis mendeteksi ini sebagai static site. Klik **Deploy**.
5. Selesai — Anda akan dapat URL seperti `https://nama-anda.vercel.app`.

### Opsi B — Lewat GitHub (rekomendasi, agar mudah update)
1. Buat repository baru di GitHub, misalnya `portfolio`.
2. Upload semua file di folder ini ke repo tersebut (`index.html`, `vercel.json`, `README.md`).
3. Buka https://vercel.com → **Add New… → Project** → **Import** repo `portfolio` Anda.
4. Biarkan semua setting default (Framework Preset: **Other**), lalu **Deploy**.
5. Setiap kali Anda push perubahan ke GitHub, Vercel otomatis re-deploy.

### Opsi C — Lewat Vercel CLI (untuk yang terbiasa terminal)
```bash
npm i -g vercel      # instal CLI sekali saja
cd portfolio         # masuk ke folder ini
vercel               # ikuti prompt, jawab default
vercel --prod        # untuk publish ke production
```

## Custom Domain (opsional)
Setelah deploy, di dashboard Vercel buka **Settings → Domains** untuk menambahkan domain pribadi
(misalnya `fahrifadillah.com`) jika Anda punya.

## Cara Edit Konten
Semua teks ada di dalam `index.html`. Beberapa yang mungkin ingin Anda ubah:
- **Email / nomor HP / link** → cari di bagian `#contact` dan `<footer>`.
- **Statistik di hero** (`5+ Projects`, `2027`, dll) → cari `class="hero-meta"`.
- **Warna tema** → ubah variabel CSS di bagian `:root` paling atas
  (`--accent` hijau, `--accent-2` biru, `--accent-3` amber).
- **Foto profil** → saat ini belum ada foto; bisa ditambahkan jika Anda mau.

## Catatan
- Link GitHub mengarah ke profil utama. Jika ingin tiap kartu project menautkan ke repo spesifik,
  beri tahu saya repo mana untuk tiap project dan saya tambahkan tautannya.
