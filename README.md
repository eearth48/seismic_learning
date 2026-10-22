# seismic_learning
# 🌋 Pusat Informasi Seismik & Geologi Indonesia (WebGIS)

Aplikasi WebGIS interaktif berbasis Leaflet.js untuk memvisualisasikan data kegempaan *real-time*, batas lempeng tektonik regional, sebaran sesar/patahan aktif darat, dan status aktivitas gunung api di seluruh wilayah Indonesia.

🔗 **Live Demo:** [https://eearth48.github.io/seismic_learning/](https://eearth48.github.io/seismic_learning/)](https://eearth48.github.io/seismic_learning/)

---

## ✨ Fitur Utama

- **Integrasi API Real-time BMKG:** Mengambil otomatis data gempa terkini (M ≥ 5.0) langsung dari *endpoint* terbuka BMKG dengan indikator status koneksi server.
- **Visualisasi Animasi Gempa:** Marker gempa terbaru dilengkapi animasi gelombang denyut (*pulsing circle*), dengan ukuran lingkaran proporsional terhadap besaran magnitudo gempa.
- **Interaksi Dua Arah (*Reverse Trigger*):** 
  - Mengeklik baris gempa atau gunung pada daftar sidebar akan memicu efek kamera melayang (*flyTo*) dan membuka *popup* informasi di peta.
  - Mengeklik penanda di peta akan otomatis menyorot dan menggulir ke entri data terkait pada daftar sidebar.
- **Layer Geologi Komprehensif:**
  - Batas lempeng tektonik regional (garis merah tebal).
  - Jalur sesar aktif daratan Indonesia (garis putus-putus oranye Pusgen).
  - Pemantauan status gunung api (Awas, Siaga, Waspada, Normal).
- **Pengalih Basemap (Dual Basemap):** Pilihan tampilan peta kartografi (OpenStreetMap) dan citra satelit resolusi tinggi (Esri World Imagery) dengan label toponimi.
- **Filter Dinamis & Indikator KPI:** Ringkasan statistik jumlah gempa dan gunung berstatus Siaga/Awas, serta penyaringan daftar gunung api interaktif berdasarkan tingkat statusnya.
- **Antarmuka Responsif:** Panel kontrol *floating* gelap (*dark mode*) dengan efek *backdrop blur*, tombol sembunyikan/tampilkan sidebar, serta penyesuaian tata letak untuk perangkat seluler.

---

## 🛠️ Tumpukan Teknologi (Tech Stack)

- **Pustaka Pemetaan:** [Leaflet.js](https://leafletjs.com/) (v1.9.4)
- **Basemap Providers:** OpenStreetMap & Esri World Imagery
- **Format Data Spasial:** GeoJSON (garis lempeng & sesar aktif)
- **Gaya Visual:** HTML5, CSS3 kustom (Dark Glassmorphism, CSS Keyframe Animations)
- **Deployment:** GitHub Pages (Statis, tanpa dependensi server backend)

---

## 📡 Sumber Data

1. **Data Gempa Terkini:** Badan Meteorologi, Klimatologi, dan Geofisika ([BMKG Open Data](https://data.bmkg.go.id/))
2. **Batas Lempeng Tektonik:** Peter Bird (2002) via *fraxen/tectonicplates*
3. **Patahan / Sesar Aktif Indonesia:** Pusat Studi Gempa Nasional (Pusgen) via *GEMScienceTools*
4. **Data Sebaran Gunung Api:** Pusat Vulkanologi dan Mitigasi Bencana Geologi (PVMBG)

---

## 💻 Penggunaan Lokal

1. Salin repositori ini:
   ```bash
   git clone [https://github.com/marseventz48/seismic_learning.git](https://github.com/marseventz48/seismic_learning.git)
