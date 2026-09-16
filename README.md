# FokusKonten Official Asset CDN 🚀

Repositori aset publik terdistribusi untuk platform **FokusKonten** (`fokuskonte.my.id`).
Dirancang dengan arsitektur **Zero-Bloat Asset Delivery** menggunakan jsDelivr Edge CDN dan GitHub Pages.

---

## 📁 Struktur Direktori

```text
fokuskonten-assets/
├── testpoint/             # 1.513 Skema Titik Jumper EDL 9008 & ISP Pinout (WebP HD)
│   ├── advan/
│   ├── asus/
│   ├── huawei/
│   ├── oppo/
│   ├── samsung/
│   ├── vivo/
│   └── xiaomi/
├── ebook/                 # Cover E-Book Digital & Modul Panduan (WebP)
├── covers/                # Banner & Cover Produk Digital
└── testpoints_index.json  # Indeks O(1) Pemetaan Model & Slug
```

---

## ⚡ URL Akses CDN Global

Setiap aset dapat diakses secara publik dengan latency ultra-rendah melalui dua jalur:

### 1. jsDelivr Edge CDN (Rekomendasi Utama)
```text
https://cdn.jsdelivr.net/gh/mcjobs-id/fokuskonten-assets@main/testpoint/[brand]/[filename].webp
https://cdn.jsdelivr.net/gh/mcjobs-id/fokuskonten-assets@main/testpoints_index.json
```

### 2. GitHub Pages
```text
https://mcjobs-id.github.io/fokuskonten-assets/testpoint/[brand]/[filename].webp
https://mcjobs-id.github.io/fokuskonten-assets/testpoints_index.json
```

---

## 📊 Metrik Efisiensi Penyimpanan

* **Total Berkas Skema** : 1352 file
* **Ukuran Awal (RAW)**   : 409.9 MB
* **Ukuran WebP HD (q82)**: 163.6 MB
* **Efisiensi Bandwidth** : **Hemat 60%**
* **Keamanan & Lisensi**  : Verified by FokusKonten Team
