# Prediksi Harga Minyak Mentah Menggunakan LSTM

Repositori ini berisi skrip Python untuk melakukan analisis deret waktu dan prediksi harga minyak mentah global menggunakan model Deep Learning berbasis Long Short-Term Memory (LSTM). Dataset yang digunakan bersumber dari [Energy Institute Statistical Review](https://www.energyinst.org/statistical-review).

## Deskripsi Proyek

Proyek ini dilakukan sebagai bagian dari tugas akhir (skripsi) untuk:

* Melakukan pembersihan dan eksplorasi data harga minyak mentah (Dubai, Brent, Nigerian, WTI).
* Mendeteksi outlier dan menguji kestasioneran data.
* Melatih model LSTM untuk memprediksi harga minyak di masa depan.
* Membandingkan hasil prediksi dengan nilai aktual menggunakan metrik seperti MAE, RMSE, dan R².

## Instalasi

Untuk mereproduksi proyek ini, gunakan versi library berikut:

```bash
pip install numpy==1.23.5 tensorflow==2.12.0 keras==2.12.0 keras-tuner==1.3.5 pmdarima==2.0.3 statsmodels==0.14.0 openpyxl==3.1.2
```

## Dependencies

* pandas
* numpy
* seaborn
* matplotlib
* tensorflow / keras
* sklearn
* pmdarima
* statsmodels
* openpyxl

## Metodologi

1. **Preprocessing**: Imputasi missing values, deteksi outlier (Z-score), pengujian stasioneritas (ADF Test).
2. **Transformasi**: Scaling data dengan MinMaxScaler.
3. **Modeling**: LSTM dengan tuning hyperparameter menggunakan Keras Tuner.
4. **Evaluasi**: MAE, RMSE, dan R² score.
