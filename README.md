# 👁️ Real-Time Face Detection with OpenCV

Proyek ini adalah implementasi sederhana dari deteksi wajah secara real-time menggunakan Python dan OpenCV. Kamera akan menangkap video secara langsung, mendeteksi wajah menggunakan Haar Cascade Classifier, dan menggambar kotak merah di sekitar wajah yang terdeteksi.

## 📦 Fitur

- Deteksi wajah secara real-time menggunakan webcam
- Visualisasi deteksi dengan kotak merah di sekitar wajah
- Tekan `q` untuk keluar dari aplikasi

## 🛠️ Persyaratan

Pastikan kamu memiliki:

- Python 3.x
- OpenCV (`cv2`)
- File Haar Cascade XML (misalnya: `venv_ref.xml`)

## 📥 Instalasi

1. **Clone repositori ini** (jika belum):
   ```bash
   git clone https://github.com/username/face-detection-opencv.git
   cd face-detection-opencv
   ```

2. **Buat virtual environment (opsional tapi disarankan)**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/macOS
   venv\Scripts\activate     # Windows
   ```

3. **Install dependensi**:
   ```bash
   pip install opencv-python
   ```

4. **Pastikan file Haar Cascade (`venv_ref.xml`) tersedia**  
   Jika belum punya, kamu bisa mengunduh dari [OpenCV GitHub](https://github.com/opencv/opencv/tree/master/data/haarcascades), misalnya:
   - `haarcascade_frontalface_default.xml`

   Lalu ubah nama file tersebut menjadi `venv_ref.xml` atau sesuaikan di kode.

## 🚀 Menjalankan Program

Jalankan skrip Python:

```bash
python face_detection.py
```

Jendela baru akan terbuka menampilkan video dari webcam dengan deteksi wajah. Tekan `q` untuk keluar dari aplikasi.

## 🧠 Struktur Kode

- `face_detection(frame)`: Mengubah frame menjadi grayscale dan mendeteksi wajah.
- `drawer_box(frame)`: Menggambar kotak merah di sekitar wajah yang terdeteksi.
- `close_camera()`: Menutup kamera dan jendela aplikasi.
- `main()`: Loop utama untuk membaca frame dan menampilkan hasil deteksi.

## 📌 Catatan

- Pastikan webcam terhubung dan dapat diakses oleh sistem.
- Jika kamera tidak terbuka, periksa apakah ada aplikasi lain yang sedang menggunakannya.

## 📄 Lisensi

Proyek ini bebas digunakan untuk keperluan pembelajaran dan pengembangan. Silakan modifikasi sesuai kebutuhan.
