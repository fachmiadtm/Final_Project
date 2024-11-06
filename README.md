# Prediksi Harga Mobil Bekas di UK

Proyek ini bertujuan untuk mengembangkan model machine learning yang dapat memprediksi harga mobil bekas di Inggris berdasarkan berbagai fitur seperti jarak tempuh (mileage), ukuran mesin, jenis bahan bakar, dan lainnya. Proyek ini menggunakan beberapa teknik regresi untuk menghasilkan prediksi harga yang akurat dan mencakup analisis data eksploratif (EDA), rekayasa fitur, serta evaluasi model dengan metrik seperti MAE dan MAPE untuk menilai kinerja model.

## Deskripsi Data

Dataset ini terdiri dari beberapa fitur penting yang mempengaruhi harga mobil di Inggris, termasuk:

- **year**: Tahun pembuatan mobil.
- **mileage**: Jarak tempuh mobil.
- **tax**: Pajak mobil.
- **mpg**: Miles per gallon (efisiensi bahan bakar).
- **engineSize**: Ukuran mesin mobil.
- **price**: Variabel target yang menunjukkan harga mobil.

## Alur Kerja Proyek

1. **Analisis Data Eksploratif (EDA)**:
   - Visualisasi distribusi, deteksi outlier, dan memahami hubungan antar fitur.
   - Evaluasi multikolinieritas antara fitur numerik menggunakan VIF.

2. **Rekayasa Fitur**:
   - Menambahkan fitur turunan seperti `age` dan `mileage_per_year`.
   - One-hot encoding untuk variabel kategorikal (misalnya, merek, transmisi, jenis bahan bakar).

3. **Pemodelan**:
   - Melatih beberapa model regresi (misalnya, Random Forest, XGBoost).
   - Evaluasi kinerja model menggunakan metrik seperti MAE dan MAPE.

4. **Evaluasi Model**:
   - Menghitung MAE, MAPE, dan R² untuk menilai akurasi model.
   - Menggunakan nilai SHAP dan feature importances untuk interpretasi model.

## Hasil

- **Mean Absolute Error (MAE)**: Model mencapai rata-rata error absolut sekitar 1006.04, menunjukkan rata-rata deviasi harga dalam dollar dari harga aktual.
- **Mean Absolute Percentage Error (MAPE)**: Model mencapai error persentase rata-rata sebesar 6.47%, menunjukkan kinerja yang dapat diandalkan dalam memprediksi harga mobil.

## Kesimpulan

Model ini menyediakan estimasi yang andal untuk memprediksi harga mobil bekas di pasar UK. Dengan MAE sebesar 1006.04 dan MAPE sebesar 6.47%, model ini menunjukkan keseimbangan antara akurasi dan interpretasi. Penggunaan model machine learning secara signifikan mengurangi error prediksi dibandingkan dengan metode berbasis aturan (rule-based).

## Rekomendasi

Peningkatan lebih lanjut dapat dilakukan dengan mengeksplorasi teknik rekayasa fitur yang lebih canggih, menggabungkan data eksternal tambahan (seperti tren pasar), dan menggunakan tuning hiperparameter untuk mengoptimalkan kinerja model.
