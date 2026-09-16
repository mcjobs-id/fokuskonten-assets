# FokusKonten Official Asset CDN 🚀

Repositori aset publik terdistribusi untuk platform **FokusKonten** (`fokuskonte.my.id`).
Dirancang dengan arsitektur **Zero-Bloat Asset Delivery** menggunakan jsDelivr Edge CDN dan GitHub Pages.

---

## 📁 Struktur Direktori
 
```text
fokuskonten-assets/
├── toko-digital/                 # 742 SKU Katalog Toko Digital (4.077 Berkas WebP: Cover & Preview Slides)
│   └── [SKU]/
│       ├── [SKU]_cover.webp      # Cover Utama Resolusi Tinggi
│       └── [SKU]_slide_[n].webp  # Preview Sheet Desain / Galeri
├── ebook/                        # 2.471 Cover WebP E-Book Digital & Buku Elektronik
├── covers/                       # Banner & Cover Produk Digital Pelengkap
├── testpoint/                    # 1.042 Foto Diagram Motherboard & Titik Testpoint EDL 9008
├── isp/                          # 1.565 Diagram Skema Pinout Direct ISP eMMC/UFS
├── toko_digital_assets_index.json # Indeks SSOT 742 SKU Toko Digital (O(1) CDN Lookup)
├── technician_assets_index.json  # Indeks Gabungan Testpoint & ISP Hardware
└── testpoints_index.json         # Indeks Pemetaan Model & Slug Teknisi
```

---

## ⚡ URL Akses CDN Global

Setiap aset dapat diakses secara publik dengan latency ultra-rendah melalui jaringan global:

### 1. jsDelivr Edge CDN (Rekomendasi Utama)
```text
# Toko Digital Covers & Slides:
https://cdn.jsdelivr.net/gh/mcjobs-id/fokuskonten-assets@main/toko-digital/[SKU]/[filename].webp

# E-Book Covers:
https://cdn.jsdelivr.net/gh/mcjobs-id/fokuskonten-assets@main/ebook/[SKU]/[filename].webp

# Hardware Technician (Testpoint & ISP):
https://cdn.jsdelivr.net/gh/mcjobs-id/fokuskonten-assets@main/testpoint/[brand]/[filename].webp
https://cdn.jsdelivr.net/gh/mcjobs-id/fokuskonten-assets@main/isp/[brand]/[filename].webp

# Manifest & Indices:
https://cdn.jsdelivr.net/gh/mcjobs-id/fokuskonten-assets@main/toko_digital_assets_index.json
https://cdn.jsdelivr.net/gh/mcjobs-id/fokuskonten-assets@main/technician_assets_index.json
```

### 2. Fallback Remote (Raw GitHub)
```text
https://raw.githubusercontent.com/mcjobs-id/fokuskonten-assets/main/toko-digital/[SKU]/[filename].webp
```

---

## 📊 Metrik Efisiensi Penyimpanan

* **Toko Digital Assets** : 742 SKU | 4.077 Berkas (Dikurangi dari 1.13 GB RAW menjadi 376 MB WebP, hemat 66.8%)
* **E-Book WebP Covers**   : 2.471 File (~88 MB)
* **Hardware Testpoints**  : 1.042 File (~118 MB)
* **Direct ISP Pinouts**   : 1.565 File (~142 MB)
* **Total Media Terdistribusi**: >9.100 Berkas Statis
* **Efisiensi Bandwidth**  : **Zero Hosting Cost & Zero Bandwidth Load di Server Utama**
* **Keamanan & Lisensi**   : Verified by FokusKonten Team
