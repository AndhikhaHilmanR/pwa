================================================================
  PERBANDINGAN TIPE PENGEMBANGAN APLIKASI MOBILE
  (Native vs Hybrid vs PWA)
================================================================

ASPEK            | NATIVE              | HYBRID                  | PWA
-----------------|---------------------|-------------------------|-------------------------
Teknologi        | Kotlin / iOS / ARK  | HTML/JS/CSS + Plugin    | HTML/JS/CSS + Web Worker
Akses Hardware   | NFC, BT, Cam        | Via Plugin              | API: Cam, GPS, Mic, BT
Performa         | Tinggi (3x)         | Sedang (2x)             | Standar (1x)
Biaya Develop    | Mahal (AP, PJ, MS)  | Npm/Yarn + HTML/JS/CSS  | HTML/JS/CSS
Distribusi       | App Store / Play    | App Store (review)      | URL (langsung)
Cocok untuk      | Game, VR/AR         | App Bisnis              | Web Apps
Kode Basis       | Per platform        | 2x (web + plugin)       | 1x

================================================================
PENJELASAN SINGKAT (Pola PREP)
================================================================

1. NATIVE
   - Point   : Aplikasi dibuat khusus per platform (Android/iOS)
   - Reason  : Akses penuh ke hardware, performa tertinggi (3x)
   - Example : Game berat, aplikasi VR/AR, fitur NFC/BT/Kamera
   - Point   : Pilihan terbaik jika performa adalah prioritas utama

2. HYBRID
   - Point   : Gabungan teknologi web + native melalui plugin
   - Reason  : Satu kode web bisa jalan di banyak platform
   - Example : Aplikasi bisnis dengan Ionic/Capacitor
   - Point   : Kompromi terbaik antara biaya dan kemampuan native

3. PWA (Progressive Web App)
   - Point   : Aplikasi web yang terasa seperti aplikasi native
   - Reason  : Tidak perlu unduh dari toko, distribusi via URL
   - Example : Twitter Lite, Starbucks Web App
   - Point   : Biaya paling rendah, 1x kode, distribusi paling cepat

================================================================
KESIMPULAN
================================================================

Pilih NATIVE   -> jika butuh performa maksimal & akses hardware penuh
Pilih HYBRID   -> jika butuh fitur native tapi hemat biaya develop
Pilih PWA      -> jika target distribusi cepat & berbasis web

================================================================
