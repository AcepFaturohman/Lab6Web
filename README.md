# Nama : Acep Faturrohman
# NIM : 312410098
# Kelas : TI.24.A1

**Output**
<img width="959" height="435" alt="image" src="https://github.com/user-attachments/assets/ba30e59e-b2c4-448d-a71d-5d47205a3868" />

**Penjelasan**
# Layout Sederhana (Bootstrap 5)

Proyek ini adalah template halaman web sederhana berbasis **Bootstrap 5** dengan sedikit gaya kustom dan interaksi ringan menggunakan jQuery.

---

## 1) Prasyarat

Tidak ada instalasi khusus. Kamu cukup memakai browser modern. (Opsional) Editor seperti **VS Code** dengan ekstensi *Live Server* akan memudahkan pengembangan lokal.

---

## 2) Struktur Proyek

- **Home.html** — halaman utama yang memuat Bootstrap dari CDN, jQuery dari CDN, serta file CSS/JS kustom proyek. :contentReference[oaicite:0]{index=0}  
- **bootstrap.min.css** — stylesheet kustom untuk tema (warna navbar, panel, widget, tombol, dll). :contentReference[oaicite:1]{index=1}  
- **bootstrap.bundle.min.js** — skrip kustom (jQuery) untuk interaksi ringan; bisa menandai item navbar aktif dan demo tombol “View detail”. :contentReference[oaicite:2]{index=2}

---

## 3) Cara Menjalankan Secara Lokal (Paling Cepat)

1. **Download** atau **clone** repo ini.
2. Buka file **`Home.html`** langsung di browser (double-click).
3. Kamu sudah bisa melihat tampilan layout, termasuk:
   - *Brand bar* dan **navbar** berwarna biru. :contentReference[oaicite:3]{index=3}
   - *Hero section*, *panel content*, ikon lingkaran, *featurette*, dan *sidebar widget*. :contentReference[oaicite:4]{index=4}
   - Interaksi klik tombol **“View detail”** yang memunculkan *alert*. :contentReference[oaicite:5]{index=5}

> Alternatif (disarankan untuk dev): pakai ekstensi **Live Server** (VS Code) agar *auto reload* saat kamu mengubah file.

---

## 4) Dependensi & Pemuatan Aset

File **`Home.html`** sudah memuat:
- **Bootstrap CSS** via CDN (5.3.3) dan **Bootstrap JS** via CDN,  
- **jQuery 3.7.1** via CDN,  
- CSS kustom `bootstrap.min.css` dan JS kustom `bootstrap.bundle.min.js` dari root proyek. :contentReference[oaicite:6]{index=6}

Tidak perlu build step atau package manager.

---

## 5) Kustomisasi

### 5.1. Gaya (CSS)
Semua penyesuaian tema ada di **`bootstrap.min.css`**:
- Kelas `navblue` untuk warna navbar, `panel`, `widget`, `btn-ghost`, `circle`, `thumb`, hingga *footer*.  
- Responsif halus untuk perangkat kecil. :contentReference[oaicite:7]{index=7}

Edit nilai warna/ukuran sesuai kebutuhanmu.

### 5.2. Interaksi (JS)
Interaksi ringan berada di **`bootstrap.bundle.min.js`**:
- Menandai link navbar aktif berdasarkan URL.
- Demo klik tombol “View detail” yang menampilkan judul item. :contentReference[oaicite:8]{index=8}

Tambah logika lain (mis. *modal*, *toast*, AJAX) di file yang sama atau pecah ke file baru.

### 5.3. Konten (HTML)
Ubah struktur, teks, atau komponen langsung di **`Home.html`**:
- *Hero section*, 3 ikon lingkaran, *featurette* kiri/kanan, dan *sidebar widget* siap diubah. :contentReference[oaicite:9]{index=9}

---

## 6) Deploy ke GitHub Pages

1. Push kode ke branch `main` (atau `master`).
2. Di GitHub repo → **Settings** → **Pages**.
3. **Source**: pilih `Deploy from a branch`.
4. **Branch**: pilih `main` dan folder `/root` (jika file di root).
5. Klik **Save** dan tunggu situs aktif di URL GitHub Pages yang disediakan.

---

## 7) Troubleshooting

- **Tampilan tidak sesuai / tanpa gaya**  
  Pastikan `bootstrap.min.css` dipanggil setelah CSS Bootstrap CDN di `<head>`. :contentReference[oaicite:10]{index=10}

- **Tombol “View detail” tidak bereaksi**  
  Pastikan urutan skrip: jQuery CDN → Bootstrap JS CDN → `bootstrap.bundle.min.js` (kustom). :contentReference[oaicite:11]{index=11}

- **Ikon lingkaran/warna tidak muncul**  
  Cek kelas `circle`, `bg-orange`, `bg-blue`, `bg-teal` di CSS kustom. :contentReference[oaicite:12]{index=12}

---

## 8) Kontribusi

1. Fork repo ini.
2. Buat branch fitur: `git checkout -b fitur-ku`.
3. Commit perubahan: `git commit -m "Tambah fitur X"`.
4. Push branch: `git push origin fitur-ku`.
5. Buka **Pull Request**.

---

## 9) Lisensi

Tentukan lisensi sesuai kebutuhan (mis. MIT). Sertakan file `LICENSE` bila diperlukan.

---

## 10) Kredit

- [Bootstrap 5] untuk kerangka CSS.
- [jQuery] untuk interaksi ringan.
- Struktur & gaya kustom di file `Home.html`, `bootstrap.min.css`, dan `bootstrap.bundle.min.js`. :contentReference[oaicite:13]{index=13} :contentReference[oaicite:14]{index=14} :contentReference[oaicite:15]{index=15}
