Tentu, mari kita bedah materi **Mobile Computing** dari catatan tersebut secara mendalam menggunakan struktur **PREP** (*Point, Reason, Example, Point*) agar lebih terstruktur dan komprehensif.

---

### **P: Point (Titik Utama)**
**Mobile Computing** adalah sistem yang memungkinkan komputasi dilakukan secara berpindah-pindah melalui perangkat nirkabel, dengan fokus utama pada efisiensi manajemen sumber daya (baterai dan memori) melalui klasifikasi prioritas proses (Foreground, Background, dan Cache).

### **R: Reason (Alasan & Penjelasan)**
Mengapa sistem perangkat mobile harus diatur sedemikian rupa seperti yang tertulis di papan tulis?
1.  **Resource Constraints:** Perangkat mobile memiliki memori ($RAM$) dan daya baterai yang terbatas. Sistem operasi harus bertindak sebagai wasit untuk menentukan aplikasi mana yang berhak mendapatkan sumber daya penuh.
2.  **User Experience (UX):** Agar perangkat tidak "lemot", aplikasi yang sedang dilihat pengguna (*Foreground*) harus diprioritaskan di atas aplikasi yang berjalan di balik layar (*Background*).
3.  **Security (FBE):** Keamanan data di perangkat mobile menggunakan *File-Based Encryption* untuk memastikan data tetap terlindungi bahkan dalam kondisi perangkat baru menyala atau terkunci.

### **E: Example (Contoh & Komponen Teknis)**
Berdasarkan catatan Anda, berikut adalah elemen-elemen yang bekerja di lapangan:

* **Klasifikasi Proses (Killer Priorities):**
    * **Foreground:** Anda sedang membalas pesan di WhatsApp. Aplikasi ini berada di prioritas tertinggi.
    * **Background:** Sambil membalas pesan, aplikasi Dropbox sedang mengunggah file di belakang layar atau Spotify sedang memutar musik.
    * **Cache:** Aplikasi Instagram yang Anda buka 10 menit lalu; ia "tidur" di memori agar saat dibuka kembali, tidak perlu memuat dari awal (lebih cepat).
* **Mekanisme Komunikasi:**
    * **Intent:** Pesan perintah antar aplikasi (misal: aplikasi belanja memanggil aplikasi bank untuk pembayaran).
    * **Provider:** Jembatan data (misal: WhatsApp meminta akses ke daftar kontak telepon Anda).
* **Arsitektur Keamanan & Event:**
    * **FBE:** Enkripsi per file agar data pribadi tetap aman meski sistem sedang melakukan *reboot*.
    * **EDA (Event-Driven Architecture):** Sistem hanya bekerja jika ada "kejadian" tertentu, seperti saat baterai turun ke $10\%$ atau saat ada pesan masuk, sehingga tidak membuang energi secara sia-sia.

### **P: Point (Kesimpulan)**
Secara komprehensif, mobile computing dalam catatan tersebut adalah tentang **harmonisasi antara performa dan efisiensi**. Dengan menggunakan manajemen prioritas (Foreground hingga Cache) dan arsitektur berbasis *event* (EDA), perangkat mobile dapat memberikan pengalaman yang mulus bagi pengguna tanpa menghabiskan daya secara boros.
