# 📊 Model Regresi Linear untuk Prediksi Pelanggan

## 📌 Ringkasan Proyek
Proyek ini menerapkan **model Regresi Linear** menggunakan **Scikit-Learn** untuk memprediksi jumlah pelanggan berdasarkan anggaran iklan yang dikeluarkan untuk **TV, Radio, dan Media Sosial**. Dataset yang digunakan berisi data pengeluaran pemasaran dan jumlah pelanggan yang diperoleh.

## 🛠 Teknologi yang Digunakan
- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib & Seaborn

## 📂 Informasi Dataset
Dataset ini memiliki kolom sebagai berikut:
- `TV_Ads_Budget`: Anggaran iklan yang dikeluarkan untuk TV (dalam USD)
- `Radio_Ads_Budget`: Anggaran iklan yang dikeluarkan untuk Radio (dalam USD)
- `Social_Media_Ads_Budget`: Anggaran iklan yang dikeluarkan untuk Media Sosial (dalam USD)
- `Number_of_Customers`: Jumlah pelanggan yang diperoleh (**Variabel Target**)

## 📊 Pelatihan & Evaluasi Model
Model ini melalui beberapa tahapan berikut:
1. Memuat dan mengeksplorasi dataset.
2. Melakukan praproses data (mengatasi nilai kosong, normalisasi jika diperlukan).
3. Membagi data menjadi **data latih** dan **data uji**.
4. Melatih **model Regresi Linear** menggunakan Scikit-Learn.
5. Mengevaluasi performa model menggunakan metrik berikut:
   - **Mean Absolute Error (MAE)**
   - **Mean Squared Error (MSE)**
   - **Root Mean Squared Error (RMSE)**
   - **R² Score**

## 🚀 Cara Menjalankan Proyek
1. Clone repositori ini:
   ```bash
   git clone https://github.com/baloerrr04/sklearn-linear-regression-ads.git
   cd your-repo-name
   ```
2. Instal dependensi yang diperlukan:
   ```bash
   pip install -r requirements.txt
   ```
3. Jalankan skrip:
   ```bash
   python main.py
   ```

## 🔬 Pengujian dengan Data Baru
Untuk menguji model dengan data baru, perbarui DataFrame `new_data` dalam skrip:
```python
new_data = pd.DataFrame({
    'TV_Ads_Budget': [1200, 300, 850],
    'Radio_Ads_Budget': [250, 90, 200],
    'Social_Media_Ads_Budget': [180, 50, 140]
})
```
Jalankan prediksi dan lihat hasilnya:
```python
predictions = model.predict(new_data)
print(predictions)
```

## 📈 Contoh Hasil Evaluasi
| Metrik  | Skor |
|---------|-------|
| MAE     | 24.73 |
| R² Score | 0.97 |

![Deskripsi Gambar](path/gambar.png)


## 📜 Lisensi
Proyek ini bersifat open-source dan tersedia di bawah lisensi **MIT**.

---
**Penulis:** Nama Anda  
**GitHub:** [Profil Anda](https://github.com/baloerrr04)
