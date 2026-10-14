# Estimasi Kecepatan Kendaraan Berbasis Video Menggunakan MOG2 dan KNN

## Deskripsi Proyek
Proyek ini bertujuan untuk mendeteksi kendaraan, melacak pergerakannya, dan mengestimasi kecepatan berdasarkan rekaman video lalu lintas menggunakan teknik *Computer Vision*. Sistem dikembangkan menggunakan Python dan OpenCV dengan menerapkan metode *Background Subtraction* untuk memisahkan kendaraan yang bergerak dari latar belakang.
Dua metode yang digunakan adalah MOG2 (*Mixture of Gaussians Version 2*) dan KNN (*K-Nearest Neighbors*). Hasil deteksi kemudian diproses menggunakan operasi morfologi, ekstraksi fitur kontur, dan *Centroid Tracking* untuk membantu pelacakan kendaraan serta analisis pergerakannya.

## Dataset
- **Nama:** Vehicle Detection Image Dataset
- **Sumber:** [Kaggle – Vehicle Detection Image Dataset](https://www.kaggle.com/datasets/pkdarabi/vehicle-detection-image-dataset)
- **Penggunaan:** Data pendukung untuk pengembangan sistem deteksi kendaraan.

## Metode yang Digunakan
1. **Preprocessing Video:** konversi grayscale dan Gaussian Blur untuk mempersiapkan frame.
2. **Background Subtraction:** menggunakan MOG2 dan KNN untuk mendeteksi objek bergerak.
3. **Morphological Processing:** operasi opening dan closing untuk membantu mengurangi noise.
4. **Contour Feature Extraction:** menentukan area objek, bounding box, dan centroid.
5. **Centroid Tracking:** melacak posisi kendaraan dan memberikan identitas objek.
6. **Motion Analysis:** menganalisis perpindahan kendaraan untuk mengestimasi kecepatan.
7. **Visualisasi:** menampilkan hasil deteksi dan pelacakan pada video keluaran.

## Hasil dan Tujuan
Sistem menghasilkan visualisasi deteksi dan pelacakan kendaraan, estimasi kecepatan dalam km/jam, serta video hasil pemrosesan dalam format MP4. Proyek ini memberikan pengalaman dalam menerapkan teknik Pengolahan Citra Digital untuk analisis pergerakan kendaraan tanpa bergantung pada model *deep learning*.
Akurasi estimasi kecepatan bergantung pada kualitas deteksi, pelacakan objek, frame rate video, dan kalibrasi jarak pada citra.
