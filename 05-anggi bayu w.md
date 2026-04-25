Berikut penjelasan dari isi papan tulis itu dengan pola PREP (Point–Reason–Example–Point) agar runtut dan mudah dipahami:


---

1. POINT (Inti Utama)

Materi di papan membahas arsitektur sistem pada mobile computing (Android), khususnya bagaimana aplikasi berjalan melalui:

Foreground & Background process

Manajemen memori & resource

Arsitektur komunikasi (client–provider–database–cache)

Prioritas proses & request query


Intinya: bagaimana aplikasi mobile mengelola proses, data, dan performa agar tetap efisien di perangkat dengan resource terbatas.


---

2. REASON (Alasan / Konsep Dasar)

a. Foreground vs Background

Foreground: aplikasi yang sedang dipakai user (aktif di layar)

Contoh aktivitas: klik, input, swipe


Background: proses berjalan tanpa interaksi langsung

Contoh: sinkronisasi data, GPS, NFC



👉 Kenapa penting? Karena sistem operasi (Android) harus mengatur prioritas agar aplikasi yang sedang digunakan tetap lancar.


---

b. Memory & Resource Management

Di papan tertulis:

Memory

WM (Window Manager)

PBE (kemungkinan maksudnya File-Based Encryption / keamanan data)

EDA (Event Driven Architecture)


👉 Artinya:

Sistem mobile punya RAM terbatas, jadi harus pintar mengatur aplikasi mana yang tetap hidup.

Data juga harus aman (enkripsi).

Sistem berbasis event → hanya aktif saat ada aksi (hemat resource).



---

c. Provider & Data Flow

Diagram menunjukkan alur:

User → WA/WB → Backend → Database → Cache

👉 Artinya:

Aplikasi tidak langsung ke database

Lewat provider / API / backend

Cache digunakan untuk mempercepat akses data



---

d. Cache & Inactive State

Cache = penyimpanan sementara

Inactive = aplikasi tidak aktif tapi belum ditutup


👉 Kenapa penting? Supaya:

Aplikasi bisa dibuka cepat lagi

Tidak perlu load ulang dari awal



---

e. Process Priority

Di kanan atas tertulis “caller priorities”

👉 Android punya prioritas:

1. Foreground (tertinggi)


2. Visible


3. Service


4. Background


5. Cached (paling rendah, bisa dibunuh sistem)



Tujuannya: optimasi performa & baterai


---

f. Request & Query Flow

Bagian bawah ada:

Request Query → Backend → DB → Response

👉 Ini menjelaskan:

Cara aplikasi mengambil data

Ada delay (misalnya 0.5s, 1.5s, dll)

Perlu optimasi (cache, indexing)



---

3. EXAMPLE (Contoh Nyata)

Misalnya kamu buka WhatsApp:

1. Kamu chat → Foreground


2. WhatsApp sync pesan → Background service


3. Data chat:

Diambil dari cache (cepat)

Jika belum ada → ambil dari server/database



4. Kalau kamu pindah ke aplikasi lain:

WhatsApp jadi background



5. Kalau RAM penuh:

Sistem bisa kill aplikasi cached





---

4. POINT (Penegasan Ulang)

Jadi kesimpulannya:

Sistem mobile dirancang dengan manajemen proses & memori yang ketat

Ada pembagian jelas:

Foreground (aktif)

Background (pasif)


Data mengalir melalui:

Provider → Backend → Database → Cache


Semua ini bertujuan: 👉 menjaga performa, hemat baterai, dan respons cepat
