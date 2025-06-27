# 🚀 DBSCAN Clustering Project

## 📚 Deskripsi
Proyek ini adalah implementasi **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** untuk mengelompokkan data simulasi menggunakan Python.  
DBSCAN efektif untuk:
- 📦 Mengelompokkan data tanpa perlu menentukan jumlah cluster di awal
- 🎯 Mendeteksi outlier atau noise secara otomatis

---

## 🗂️ Dataset
Dataset dibuat menggunakan `make_blobs` dengan rincian:
- 🔢 **750 sampel data**
- 🎯 **3 pusat cluster**
- ⚙️ Data dinormalisasi dengan `StandardScaler` agar distribusinya standar

---

## 🛠️ Tools & Teknologi
- 🐍 Python
- 📦 scikit-learn
- 📊 Matplotlib
- 🔢 NumPy

---

## ⚙️ Alur Proses
1. 🚚 Mengimpor library yang dibutuhkan
2. 🏗️ Membuat dataset dengan `make_blobs`
3. 🧹 Menormalisasi data
4. 🔍 Visualisasi data awal
5. 🧩 Clustering dengan **DBSCAN** (`eps=0.3`, `min_samples=10`)
6. 📝 Evaluasi model dengan:
   - ✅ Homogeneity
   - ✅ Completeness
   - ✅ V-Measure
   - ✅ Adjusted Rand Index (ARI)
   - ✅ Adjusted Mutual Information (AMI)
   - ✅ Silhouette Coefficient
7. 🎨 Visualisasi hasil clustering (core points, border points, noise)

---

## 📈 Hasil Evaluasi
| Metrik                       | Nilai     |
|------------------------------|-----------|
| Estimated Clusters           | 3         |
| Estimated Noise Points       | 18        |
| Homogeneity                  | 0.887     |
| Completeness                 | 0.880     |
| V-Measure                    | 0.883     |
| Adjusted Rand Index          | 0.935     |
| Adjusted Mutual Information  | 0.880     |
| Silhouette Coefficient       | 0.571     |

---

## 🎯 Visualisasi
- 🟢 **Core Points** → Titik besar
- 🟡 **Border Points** → Titik kecil
- ⚫ **Noise** → Titik hitam (data di luar cluster)

---

## ✅ Kesimpulan
Algoritma **DBSCAN**:
- 🎉 Berhasil membentuk 3 cluster sesuai dengan data asli
- 🕵️‍♂️ Berhasil mendeteksi 18 data *noise*
- 🔍 Memberikan evaluasi clustering yang **sangat baik**
- 🚀 Cocok digunakan untuk dataset yang tidak beraturan dan mengandung outlier

---

## 🔗 Referensi
- 📄 [Scikit-Learn DBSCAN Example](https://scikit-learn.org/stable/auto_examples/cluster/plot_dbscan.html)
- 🗂️ Dataset: `make_blobs` dari `sklearn.datasets`

---

> 💡 *"Clustering is not just grouping data, it’s about finding structure in the chaos."* ✨
