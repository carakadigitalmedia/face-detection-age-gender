# Face Detection & Age/Gender Estimation Web App

Aplikasi ini menggunakan [face-api.js](https://github.com/justadudewhohacks/face-api.js) untuk mendeteksi wajah, memperkirakan usia, jenis kelamin, dan ekspresi secara realtime di browser.

---

## Cara Menggunakan

- Klik **Start Camera** untuk mulai menggunakan webcam.
- Klik **Stop Camera** untuk berhenti.
- Klik **Open Image** untuk mengunggah gambar dan analisis.
- Klik **Capture Snapshot** untuk mengambil screenshot dengan overlay.
- Klik **Download Result** untuk mengunduh gambar hasil deteksi.

---

## Menyiapkan Model

1. Unduh model-model dari repository resmi face-api.js:  
   https://github.com/justadudewhohacks/face-api.js/tree/master/weights

   File yang diperlukan:  
   - tiny_face_detector_model-weights_manifest.json dan file biner terkait  
   - age_gender_model-weights_manifest.json dan file biner terkait  
   - face_landmark_68_model-weights_manifest.json dan file biner terkait  
   - face_expression_model-weights_manifest.json dan file biner terkait

2. Letakkan semua file model tersebut ke folder `/models` di lokasi yang sama dengan `index.html`.

---

## Deploy ke GitHub Pages

1. Buat repository baru di GitHub dan upload semua file (`index.html`, folder `models`, dan `README.md`).

2. Aktifkan GitHub Pages di **Settings > Pages** dengan sumber dari branch `main` dan folder `/ (root)`.

3. Akses URL GitHub Pages yang diberikan.

---

## Catatan

- Aplikasi ini berjalan 100% di client (browser), tidak butuh server backend.
- Pastikan akses menggunakan protokol `https` agar kamera dapat diakses.
- Jika tidak ingin repot upload model, bisa gunakan model remote dengan mengubah variabel `MODEL_URL` di `index.html` menjadi:  
  `https://justadudewhohacks.github.io/face-api.js/models`

---

## Lisensi

Open source, gunakan sesuai kebutuhan.
