# 🌌 Interstellar Black Hole — 3D Gravitational Lensing

Simulasi ** Interstellar Black Hole** berbasis HTML, WebGL, GLSL Shader, dan Three.js.

Fitur:
- 🕳️ Black-hole shadow berbentuk bulat
- 🌀 Rotasi accretion disk
- 🌌 Gravitational lensing
- 🧲 Efek Kerr frame-dragging
- ✨ Background berotasi otomatis secara perlahan
- 🔥 Efek Doppler pada accretion disk
- 📱 Kontrol touchscreen
- 🖱️ Kontrol mouse
- 📊 FPS counter yang bisa hide/show
- ⚙️ Panel pengaturan yang bisa hide/show
- 🚀 Tidak membutuhkan backend

> **Catatan:** efek relativistik di project ini adalah simulasi visual berbasis shader dan ray-bending, bukan solver numerik relativitas umum penuh.

---

## 📁 Struktur Project

```text
black-hole-html/
├── index.html
└── README.md
```

---

# 🚀 Instalasi

## Cara 1 — Buka langsung

Buka:

```text
index.html
```

dengan browser modern seperti Chrome, Edge, Firefox, atau Safari.

> ⚠️ Three.js dimuat dari CDN, sehingga koneksi internet diperlukan saat library diambil.

## Cara 2 — Local Server

Masuk ke folder project:

```bash
cd kerr-black-hole
```

Jalankan:

```bash
python -m http.server 8000
```

Windows juga dapat menggunakan:

```bash
py -m http.server 8000
```

Kemudian buka:

```text
http://localhost:8000
```

---

# 🍴 Cara Fork Repository

1. Buka repository project di GitHub.
2. Klik **Fork**.
3. Pilih akun GitHub kamu.
4. GitHub akan membuat salinan repository ke akunmu.

Contoh:

```text
https://github.com/bahrizalmulyawa /black-hole-html
```

---

# 💻 Clone Repository

Setelah fork:

```bash
git clone https://github.com/bahrizalmulyawan/black-hole-html.git
```

Masuk ke folder:

```bash
cd black-hole-html
```

Jalankan:

```bash
python -m http.server 8000
```

Buka:

```text
http://localhost:8000
```

---

# 🔄 Update dari Repository Original

Tambahkan repository original sebagai upstream:

```bash
git remote add upstream https://github.com/bahrizalmulyawan/black-hole-html.git
```

Cek:

```bash
git remote -v
```

Ambil update:

```bash
git fetch upstream
```

Gabungkan:

```bash
git merge upstream/main
```

---

# 📱 Kontrol

## Mobile

| Gesture | Fungsi |
|---|---|
| 👆 1 jari + drag | Orbit / geser sudut pandang |
| 🤏 Pinch | Zoom |
| 👆 Geser vertikal | Mengubah sudut kamera |

## Desktop / Laptop

| Input | Fungsi |
|---|---|
| 🖱️ Klik kiri + drag | Orbit / geser sudut pandang |
| 🖱️ Scroll | Zoom |
| ⚙️ Settings | Hide/show panel |
| 📊 FPS (optional) | Hide/show FPS |

---

# ⚙️ Pengaturan

### Kerr Spin

Mengatur parameter spin:

```text
0 → 0.998
```

### Disk Brightness

Mengatur kecerahan accretion disk.

### Rotation

Mengatur rotasi visual material accretion disk.

---

# 🌌 Background Rotation

Background dapat berotasi otomatis dengan kecepatan rendah untuk memberikan efek visual frame-dragging Kerr tanpa membuat animasi terlalu berat.

---

# 📊 FPS Counter

Klik:

```text
FPS (optional)
```

untuk menampilkan atau menyembunyikan FPS.

Contoh:

```text
FPS: 60
```

FPS diperbarui secara berkala agar overhead tetap kecil.

---

# ⚡ Performa

Project menggunakan WebGL shader untuk efek visual.

Pixel ratio dibatasi:

```javascript
Math.min(devicePixelRatio, 1.25)
```

Jika FPS rendah:
1. Tutup tab browser yang tidak diperlukan.
2. Gunakan browser dengan dukungan WebGL yang baik.
3. Kurangi ukuran window jika diperlukan.
4. Pantau FPS menggunakan FPS counter.
5. Hindari menjalankan beberapa aplikasi WebGL berat bersamaan.

---

# 🛠️ Teknologi

- **HTML5**
- **JavaScript**
- **WebGL**
- **GLSL**
- **Three.js**

Three.js:

```html
https://cdn.jsdelivr.net/npm/three@0.168.0/
```

---

# 🌐 Deploy ke GitHub Pages

Push project:

```bash
git add .
git commit -m "Initial release"
git push origin main
```

Kemudian buka:

**Settings → Pages**

Pilih:

```text
Deploy from a branch
```

Branch:

```text
main
```

Folder:

```text
/ (root)
```

Klik **Save**.

URL akan berbentuk:

```text
https://USERNAME.github.io/kerr-black-hole/
```

---

# 🔧 Development

Setelah melakukan perubahan:

```bash
git add .
git commit -m "Update black hole simulation"
git push origin main
```

---

# 🤝 Contributing

Pull Request dipersilakan.

Workflow:

```text
Fork
  ↓
Clone
  ↓
Edit
  ↓
Test
  ↓
Commit
  ↓
Push
  ↓
Pull Request
```

Pastikan simulasi dan kontrol mouse/touch tetap berfungsi sebelum membuat Pull Request.

---

# 📜 License

Tambahkan license sesuai kebutuhan project.

Contoh:

```text
MIT License
```

Jika menggunakan library atau asset pihak ketiga, ikuti license masing-masing dependency.

---

## 🌌 Selamat Bereksperimen!

Eksplorasi black hole, accretion disk, gravitational lensing, dan frame-dragging langsung di browser. 🕳️🌀✨
