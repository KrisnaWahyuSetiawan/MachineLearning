# 🎓 Prediksi Kelulusan Mahasiswa

Proyek ini bertujuan untuk **memprediksi kelulusan mahasiswa** berdasarkan data akademik seperti IPK, jumlah absensi, dan waktu belajar. Model dikembangkan menggunakan Python dan beberapa algoritma Machine Learning untuk membandingkan performa tiap model.

---

## 📂 Struktur Folder

| Nama File | Deskripsi |
|------------|------------|
| `kelulusan_mahasiswa.csv` | Dataset mentah berisi data mahasiswa (IPK, absensi, waktu belajar, dan status kelulusan). |
| `processed_kelulusan.csv` | Dataset hasil preprocessing (siap untuk digunakan dalam model). |
| `X_train.csv`, `X_val.csv`, `X_test.csv` | Data fitur (independen variables) yang dibagi ke dalam data latih, validasi, dan uji. |
| `y_train.csv`, `y_val.csv`, `y_test.csv` | Label target (`Lulus`) untuk data latih, validasi, dan uji. |
| `rf_model.pkl` | Model Random Forest yang telah dilatih dan disimpan. |
| `learning_curve.png`, `learning_curve_Model_1(baseline).png`, `learning_curve_Model_2.png`, `learning_curve_Model_3.png`, `learning_curve_Model_4.png` | Visualisasi kurva pembelajaran dari berbagai model yang diuji. |
| `roc_test.png` | Grafik ROC Curve hasil pengujian model. |
| `pr_test.png` | Grafik Precision-Recall Curve hasil pengujian model. |
| `pertemuan4.ipynb`, `pertemuan5.ipynb`, `pertemuan6.ipynb`, `pertemuan7.ipynb` | Notebook berisi eksperimen dan pelatihan model pada setiap tahap pembelajaran. |

---

## 🧠 Deskripsi Dataset

Kolom pada dataset utama:
| Kolom | Keterangan |
|--------|-------------|
| `IPK` | Indeks Prestasi Kumulatif mahasiswa |
| `Jumlah_Absensi` | Jumlah ketidakhadiran mahasiswa |
| `Waktu_Belajar_Jam` | Rata-rata waktu belajar mandiri per minggu |
| `Lulus` | Label hasil akhir (1 = Lulus, 0 = Tidak Lulus) |

---

## ⚙️ Tahapan Proyek

1. **Data Preparation**
   - Pembersihan dan normalisasi data (`processed_kelulusan.csv`)
   - Split data menjadi train/val/test (`X_train.csv`, dll)

2. **Model Training**
   - Model baseline dan model lanjutan diuji di notebook `pertemuan4.ipynb` s.d. `pertemuan7.ipynb`
   - Algoritma: Logistic Regression, Decision Tree, Random Forest, dan lain-lain

3. **Evaluasi**
   - Hasil dievaluasi menggunakan **akurasi, ROC, precision-recall**, dan **learning curve**
   - Model terbaik disimpan sebagai `rf_model.pkl`

---

## 📊 Visualisasi Hasil
- **Learning Curves:** menunjukkan proses konvergensi model pada data training dan validation.
- **ROC Curve (`roc_test.png`):** mengevaluasi trade-off antara True Positive Rate dan False Positive Rate.
- **PR Curve (`pr_test.png`):** menunjukkan performa model dalam mendeteksi kelas positif (kelulusan).

---

## 💡 Cara Menggunakan
1. Clone atau download folder proyek ini.
2. Buka salah satu notebook (`pertemuan4.ipynb` - `pertemuan7.ipynb`) di **Jupyter Notebook / Google Colab**.
3. Jalankan seluruh sel kode untuk memuat data, melatih model, dan melihat hasil prediksi.
4. Model terlatih dapat digunakan kembali dengan memuat file `rf_model.pkl`.

---

## 🧾 Lisensi
Proyek ini dibuat untuk **keperluan pembelajaran (akademik)** — bebas digunakan dan dimodifikasi dengan menyertakan atribusi.
