# Capstone Project Module 3 - Prediksi Pembatalan Pemesanan Hotel

## 📌 Pengantar Proyek
Proyek ini bertujuan untuk memprediksi pembatalan pemesanan hotel menggunakan teknik machine learning. Dengan menganalisis data pemesanan, kami memberikan wawasan yang dapat membantu mengurangi tingkat pembatalan dan meningkatkan efisiensi operasional hotel.

### **Permasalahan**
Tingkat pembatalan pemesanan yang tinggi menyebabkan kerugian finansial dan gangguan operasional. Dengan memprediksi kemungkinan pembatalan, hotel dapat mengambil langkah proaktif untuk mengurangi risiko dan mengoptimalkan pendapatan.

### **Tujuan**
- Mengembangkan model machine learning untuk memprediksi pembatalan pemesanan.
- Mencapai **akurasi minimal 75%** dengan fokus pada recall untuk meminimalkan false negatives.
- Memberikan wawasan bisnis yang dapat membantu pengambilan keputusan.

---

## 🗂️ Gambaran Dataset
Dataset yang digunakan mencakup lebih dari **83.000 data pemesanan hotel**, dengan fitur seperti:
- **Market Segment:** Sumber pemesanan (misalnya, Online Travel Agent, Direct).
- **Lead Time:** Jumlah hari antara pemesanan dan check-in.
- **Deposit Type:** Status deposit (misalnya, No Deposit, Non-Refund).
- **Total Special Requests:** Jumlah permintaan khusus oleh pelanggan.
- **Target Variable:** `is_canceled` (1 = Pesanan dibatalkan, 0 = Tidak dibatalkan).

---

## 🛠️ Alur Proyek
1. **Pemahaman Data**
   - Mengeksplorasi struktur dataset, distribusi target, dan hubungan antar fitur.
   - Visualisasi nilai yang hilang dan distribusi target.

2. **Persiapan Data**
   - Menangani nilai yang hilang dengan metode imputasi.
   - Encoding variabel kategorikal.
   - Feature engineering untuk meningkatkan kualitas data.

3. **Pemodelan**
   - Membangun model baseline menggunakan Logistic Regression.
   - Mengoptimasi model melalui GridSearchCV.
   - Mengatasi ketidakseimbangan kelas dengan SMOTE.

4. **Evaluasi**
   - Menggunakan metrik evaluasi seperti:
     - Akurasi: **76%**
     - Recall: **69%**
     - F1-Score: **68%**
   - Visualisasi hasil dengan Confusion Matrix dan ROC-AUC Curve.

5. **Deployment**
   - Menyimpan model yang telah dioptimasi menggunakan Pickle.
   - Membuat prototipe API menggunakan Flask untuk prediksi real-time.
