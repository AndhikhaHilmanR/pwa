Berdasarkan gambar papan tulis yang Anda lampirkan mengenai perbandingan pengembangan aplikasi (**Native, Hybrid, dan PWA**), berikut adalah penjelasan komprehensif menggunakan pola **PREP** (*Point, Reason, Evidence, Example*):

---

### **P: Point (Titik Utama)**
Papan tulis tersebut membandingkan tiga metodologi utama dalam pengembangan aplikasi seluler—yaitu **Native, Hybrid, dan PWA (Progressive Web App)**—berdasarkan aspek performa, akses perangkat keras, dan skalabilitas biaya.

### **R: Reason (Alasan)**
Perbedaan ini sangat krusial bagi pengembang atau bisnis karena setiap metode memiliki keseimbangan antara **kualitas performa** dan **efisiensi sumber daya**. Aplikasi Native unggul di performa tinggi namun mahal, sementara PWA unggul di kemudahan akses (URL) namun memiliki keterbatasan fitur sistem.

### **E: Evidence (Bukti/Data pada Gambar)**
Berdasarkan catatan di papan tulis, berikut rincian perbandingannya:

* **Native:**
    * **Teknologi:** Menggunakan bahasa asli seperti Kotlin atau Java untuk Android (APK).
    * **Akses Hardware:** Memiliki akses penuh ke sensor perangkat seperti NFC, Bluetooth (BT), dan Kamera (Cam).
    * **Performa:** Ditandai dengan "Height" (Tinggi) dan merupakan pilihan tepat untuk aplikasi kompleks seperti **Game** atau **VR/AR**.
    * **Biaya:** Cenderung paling mahal (tertulis perbandingan "3x").

* **Hybrid:**
    * **Teknologi:** Menggunakan *plugin* untuk menjembatani kode web dengan fungsi perangkat seluler.
    * **Karakteristik:** Ditandai sebagai solusi "Web App + plug".
    * **Biaya:** Berada di tengah-tengah (tertulis perbandingan "2x"). Disebutkan sebagai pilihan untuk kebutuhan **Aplikasi Bisnis**.

* **PWA (Progressive Web App):**
    * **Teknologi:** Berbasis HTML, JS, dan CSS. Berjalan melalui URL di browser.
    * **Akses Hardware:** Terbatas pada API web tertentu (Cam, GPS, BT).
    * **Efisiensi:** Merupakan pilihan paling hemat biaya (tertulis perbandingan "1x") karena tidak perlu pengembangan khusus untuk setiap sistem operasi.

### **P: Point (Kesimpulan Kembali)**
Secara garis besar, pemilihan jenis aplikasi bergantung pada tujuan akhir: **Native** untuk pengalaman pengguna yang intensif dan performa maksimal, **Hybrid** untuk keseimbangan fungsionalitas bisnis, dan **PWA** untuk kecepatan distribusi serta efisiensi biaya pengembangan.

---

**Catatan Tambahan:**
Screenshot kedua menunjukkan hasil *speed test* dengan kecepatan **0.24 Mbps (Download)** dan **0.19 Mbps (Upload)** serta ping yang sangat tinggi (**3897 ms**). Dalam konteks pengembangan aplikasi di atas, koneksi seperti ini akan sangat menghambat performa **PWA** dan **Hybrid** yang sangat bergantung pada pemuatan data dari server (Web-based), dibandingkan aplikasi **Native** yang sebagian besar asetnya sudah terpasang secara lokal di perangkat.
