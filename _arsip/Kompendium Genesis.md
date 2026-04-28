# Kamus Istilah Sains Data
> *Memori kedua untuk referensi cepat — lengkap, rinci, dan praktis.*

---

## Daftar Isi
1. [Statistik & Probabilitas](#1-statistik--probabilitas)
2. [Machine Learning — Konsep Dasar](#2-machine-learning--konsep-dasar)
3. [Evaluasi Model](#3-evaluasi-model)
4. [Algoritma & Teknik](#4-algoritma--teknik)
5. [Distribusi Data](#5-distribusi-data)
6. [Feature Engineering & Data Preprocessing](#6-feature-engineering--data-preprocessing)
7. [Deep Learning](#7-deep-learning)
8. [Validasi & Seleksi Model](#8-validasi--seleksi-model)
9. [Terminologi Umum Sains Data](#9-terminologi-umum-sains-data)

---

## 1. Statistik & Probabilitas

### p-value
- **Definisi:** Probabilitas mendapatkan hasil yang sama ekstrem (atau lebih ekstrem) dengan data yang diamati, *jika hipotesis nol (H₀) benar*.
- **Interpretasi:**
  - `p < 0.05` → Tolak H₀ (hasil dianggap signifikan secara statistik)
  - `p ≥ 0.05` → Gagal tolak H₀ (tidak cukup bukti melawan H₀)
- **Peringatan:** p-value **BUKAN** probabilitas bahwa H₀ benar. Signifikansi statistik ≠ signifikansi praktis.
- **Contoh:** Uji apakah rata-rata tinggi badan pria dan wanita berbeda → p = 0.02 → ada perbedaan signifikan.

---

### Hipotesis Nol (H₀) & Hipotesis Alternatif (H₁)
- **H₀ (Null Hypothesis):** Asumsi awal yang ingin diuji — biasanya menyatakan "tidak ada efek" atau "tidak ada perbedaan".
- **H₁ (Alternative Hypothesis):** Pernyataan yang ingin dibuktikan — kebalikan dari H₀.
- **Contoh:** H₀: Obat tidak berpengaruh. H₁: Obat berpengaruh.

---

### Confidence Interval (CI) / Interval Kepercayaan
- **Definisi:** Rentang nilai yang dengan tingkat kepercayaan tertentu (mis. 95%) berisi parameter populasi yang sebenarnya.
- **Contoh:** CI 95% untuk rata-rata = [68, 72] artinya kita 95% yakin rata-rata populasi ada di antara 68 dan 72.
- **Hubungan dengan p-value:** Jika CI 95% tidak mencakup 0 → sama dengan p < 0.05.

---

### Type I & Type II Error
| Error | Nama Lain | Deskripsi |
|-------|-----------|-----------|
| **Type I (α)** | False Positive | Menolak H₀ padahal H₀ benar |
| **Type II (β)** | False Negative | Gagal menolak H₀ padahal H₀ salah |

- **Power of Test (1 - β):** Kemampuan uji mendeteksi efek nyata. Makin besar, makin baik.

---

### Korelasi vs Kausalitas
- **Korelasi:** Hubungan statistik antara dua variabel. Tidak berarti satu menyebabkan yang lain.
- **Kausalitas:** Satu variabel *menyebabkan* perubahan pada variabel lain.
- **Contoh klasik:** Es krim terjual dan kasus tenggelam berkorelasi → keduanya disebabkan oleh musim panas (variabel konfounding).

---

### Variance & Standard Deviation
- **Variance (σ²):** Rata-rata kuadrat selisih setiap titik data dari mean. Mengukur sebaran data.
- **Standard Deviation (σ):** Akar dari variance. Lebih intuitif karena satuannya sama dengan data asli.
- **Rumus:** `σ² = Σ(xᵢ - μ)² / N`

---

### Skewness & Kurtosis
- **Skewness (Kemiringan):** Mengukur asimetri distribusi.
  - Positif → ekor panjang ke kanan (right-skewed)
  - Negatif → ekor panjang ke kiri (left-skewed)
  - = 0 → distribusi simetris
- **Kurtosis:** Mengukur "ketebalan ekor" distribusi.
  - **Leptokurtik** (> 3): Ekor tebal, lebih banyak outlier
  - **Platikurtik** (< 3): Ekor tipis, sedikit outlier
  - **Mesokurtik** (= 3): Distribusi normal

---

## 2. Machine Learning — Konsep Dasar

### Bias-Variance Tradeoff
- **Bias:** Kesalahan akibat asumsi model yang terlalu sederhana. Model dengan bias tinggi → *underfitting*.
- **Variance:** Sensitivitas model terhadap fluktuasi kecil dalam data training. Variance tinggi → *overfitting*.
- **Tradeoff:** Mengurangi bias biasanya meningkatkan variance, dan sebaliknya.
- **Total Error:** `Total Error = Bias² + Variance + Irreducible Noise`
- **Tujuan:** Menemukan titik keseimbangan di mana total error minimum.

```
       Error
         |        Variance
         |       /
         |      /
         |     /
  Total  |----/------
  Error  |   / \
         |  /   \
         | /     Bias²
         |/
         +-------------------> Model Complexity
```

---

### Overfitting
- **Definisi:** Model terlalu "menghafal" data training, termasuk noise, sehingga performa buruk pada data baru.
- **Tanda-tanda:** Training error sangat rendah, test/validation error jauh lebih tinggi.
- **Penyebab:** Model terlalu kompleks, data training terlalu sedikit, fitur terlalu banyak.
- **Solusi:** Regularisasi (L1/L2), dropout, cross-validation, lebih banyak data, simplifikasi model.

---

### Underfitting
- **Definisi:** Model terlalu sederhana sehingga tidak mampu menangkap pola dalam data.
- **Tanda-tanda:** Training error dan test error sama-sama tinggi.
- **Solusi:** Gunakan model yang lebih kompleks, tambah fitur, kurangi regularisasi.

---

### Regularisasi
- **Tujuan:** Mencegah overfitting dengan menambahkan penalti pada kompleksitas model.
- **L1 (Lasso):** Penalti = `λ Σ|wᵢ|` → mendorong beberapa bobot menjadi nol (feature selection otomatis).
- **L2 (Ridge):** Penalti = `λ Σwᵢ²` → mengecilkan semua bobot, tidak menjadi nol.
- **Elastic Net:** Kombinasi L1 + L2.

---

### Supervised vs Unsupervised vs Reinforcement Learning
| Tipe | Data Label | Contoh Task | Algoritma |
|------|-----------|-------------|-----------|
| **Supervised** | Ada | Klasifikasi, Regresi | Linear Regression, SVM, Random Forest |
| **Unsupervised** | Tidak ada | Clustering, Dimensionality Reduction | K-Means, PCA, Autoencoders |
| **Reinforcement** | Reward/Punishment | Game AI, Robotika | Q-Learning, PPO, A3C |

---

### Gradient Descent
- **Definisi:** Algoritma optimasi yang secara iteratif menggerakkan parameter ke arah yang menurunkan loss function.
- **Update Rule:** `θ = θ - α * ∇J(θ)`  (α = learning rate)
- **Varian:**
  - **Batch GD:** Gunakan semua data per iterasi. Stabil tapi lambat.
  - **Stochastic GD (SGD):** Satu sampel per iterasi. Cepat tapi noisy.
  - **Mini-batch GD:** Subset data per iterasi. Keseimbangan terbaik.

---

## 3. Evaluasi Model

### Confusion Matrix
```
                  Predicted
                  Pos    Neg
Actual  Pos  |  TP   |  FN  |
        Neg  |  FP   |  TN  |
```
- **TP (True Positive):** Prediksi positif, aktual positif ✓
- **TN (True Negative):** Prediksi negatif, aktual negatif ✓
- **FP (False Positive):** Prediksi positif, aktual negatif ✗ (Type I Error)
- **FN (False Negative):** Prediksi negatif, aktual positif ✗ (Type II Error)

---

### Metrik Klasifikasi

| Metrik | Rumus | Kapan Digunakan |
|--------|-------|-----------------|
| **Accuracy** | (TP+TN) / Total | Data seimbang |
| **Precision** | TP / (TP+FP) | Minimalkan false positive (spam detection) |
| **Recall (Sensitivity)** | TP / (TP+FN) | Minimalkan false negative (deteksi kanker) |
| **F1-Score** | 2 × (P×R)/(P+R) | Data tidak seimbang |
| **Specificity** | TN / (TN+FP) | False positive penting |

---

### AUC-ROC
- **ROC Curve:** Plot True Positive Rate vs False Positive Rate pada berbagai threshold.
- **AUC (Area Under Curve):** Semakin mendekati 1.0, semakin baik model.
  - AUC = 1.0 → model sempurna
  - AUC = 0.5 → model setara tebak acak
  - AUC < 0.5 → model lebih buruk dari tebakan acak
- **Kegunaan:** Membandingkan model tanpa bergantung pada threshold tertentu.

---

### Metrik Regresi
| Metrik | Rumus | Keterangan |
|--------|-------|------------|
| **MAE** | `Σ|yᵢ - ŷᵢ| / n` | Lebih robust terhadap outlier |
| **MSE** | `Σ(yᵢ - ŷᵢ)² / n` | Menghukum error besar lebih berat |
| **RMSE** | `√MSE` | Satuan sama dengan target, populer |
| **R² (R-squared)** | `1 - SS_res/SS_tot` | Proporsi variansi yang dijelaskan model (0–1) |
| **MAPE** | `Σ|yᵢ - ŷᵢ|/yᵢ × 100%` | Error dalam persentase |

---

## 4. Algoritma & Teknik

### Linear Regression
- **Tujuan:** Memodelkan hubungan linier antara fitur dan target kontinu.
- **Asumsi:** Linearitas, independensi, homoskedastisitas, normalitas residual.
- **Rumus:** `y = β₀ + β₁x₁ + β₂x₂ + ... + ε`

---

### Logistic Regression
- **Tujuan:** Klasifikasi biner (output 0 atau 1) menggunakan fungsi sigmoid.
- **Fungsi Sigmoid:** `σ(z) = 1 / (1 + e⁻ᶻ)` → menghasilkan probabilitas 0–1.
- **Bukan regresi sebenarnya!** Namanya menyesatkan — ini adalah algoritma klasifikasi.

---

### Decision Tree
- **Cara kerja:** Membagi data secara rekursif berdasarkan fitur yang paling informatif (Gini Impurity / Information Gain).
- **Kelebihan:** Mudah diinterpretasi, tidak perlu normalisasi.
- **Kekurangan:** Sangat rentan overfitting.

---

### Random Forest
- **Cara kerja:** Ensemble dari banyak decision tree yang dilatih pada subset data dan fitur yang berbeda (bagging).
- **Output:** Voting mayoritas (klasifikasi) atau rata-rata (regresi).
- **Kelebihan:** Robust terhadap overfitting, handle missing values dengan baik.

---

### Gradient Boosting (XGBoost, LightGBM, CatBoost)
- **Cara kerja:** Membangun tree secara sekuensial — setiap tree memperbaiki kesalahan tree sebelumnya.
- **Berbeda dari Random Forest:** Random Forest = paralel (bagging). Boosting = sekuensial.
- **Hyperparameter penting:** learning_rate, n_estimators, max_depth, subsample.

---

### Support Vector Machine (SVM)
- **Cara kerja:** Mencari hyperplane dengan margin terbesar antara kelas.
- **Kernel Trick:** Memetakan data ke dimensi lebih tinggi agar bisa dipisahkan secara linier.
- **Kernel umum:** Linear, RBF (Gaussian), Polynomial.

---

### K-Nearest Neighbors (KNN)
- **Cara kerja:** Mengklasifikasikan titik baru berdasarkan K tetangga terdekatnya.
- **Hyperparameter utama:** K (jumlah tetangga). K kecil → high variance; K besar → high bias.
- **Kelemahan:** Lambat untuk dataset besar, sensitif terhadap skala fitur.

---

### K-Means Clustering
- **Cara kerja:** Membagi data ke K cluster dengan meminimalkan inertia (jarak dalam cluster).
- **Algoritma:**
  1. Inisialisasi K centroid secara acak
  2. Assign setiap titik ke centroid terdekat
  3. Update centroid ke rata-rata cluster
  4. Ulangi hingga konvergen
- **Cara pilih K:** Elbow Method, Silhouette Score.

---

### Principal Component Analysis (PCA)
- **Tujuan:** Dimensionality reduction dengan mempertahankan variansi maksimum.
- **Cara kerja:** Mencari arah (principal components) di mana data paling tersebar.
- **Kapan digunakan:** Visualisasi, mengurangi multikolinearitas, mempercepat training.
- **Peringatan:** Komponen PCA tidak bisa diinterpretasikan langsung.

---

## 5. Distribusi Data

### Distribusi Normal (Gaussian)
- **Definisi:** Distribusi simetris berbentuk lonceng, didefinisikan oleh mean (μ) dan standar deviasi (σ).
- **Aturan 68-95-99.7:**
  - 68% data dalam ±1σ
  - 95% data dalam ±2σ
  - 99.7% data dalam ±3σ
- **Notasi:** `X ~ N(μ, σ²)`

---

### Distribusi Binomial
- **Definisi:** Distribusi jumlah sukses dalam n percobaan independen dengan probabilitas sukses p.
- **Notasi:** `X ~ B(n, p)`
- **Mean:** `μ = np` | **Variance:** `σ² = np(1-p)`
- **Contoh:** Jumlah kepala dalam 10 kali lempar koin.

---

### Distribusi Poisson
- **Definisi:** Distribusi jumlah kejadian dalam interval waktu/ruang tertentu, dengan rata-rata λ.
- **Notasi:** `X ~ Poisson(λ)`
- **Ciri khas:** Mean = Variance = λ
- **Contoh:** Jumlah pelanggan yang datang per jam, jumlah email per hari.

---

### Distribusi Uniform
- **Definisi:** Setiap nilai dalam rentang [a, b] memiliki probabilitas yang sama.
- **Tipe:**
  - **Diskrit:** Semua nilai integer dalam rentang memiliki peluang sama.
  - **Kontinu:** `f(x) = 1/(b-a)` untuk a ≤ x ≤ b.

---

### Distribusi Eksponensial
- **Definisi:** Waktu antar kejadian dalam proses Poisson.
- **Notasi:** `X ~ Exp(λ)`
- **Mean:** `1/λ` | **Memoryless property:** P(X > s+t | X > s) = P(X > t)
- **Contoh:** Waktu tunggu antar pelanggan di kasir.

---

### Distribusi Bernoulli
- **Definisi:** Percobaan tunggal dengan dua kemungkinan: sukses (1) atau gagal (0) dengan probabilitas p.
- **Catatan:** Binomial = jumlah n percobaan Bernoulli.

---

### Distribusi t-Student
- **Definisi:** Digunakan ketika ukuran sampel kecil dan/atau variance populasi tidak diketahui.
- **Semakin besar degrees of freedom → mendekati distribusi normal.**
- **Digunakan dalam:** t-test, confidence interval untuk sampel kecil.

---

### Distribusi Chi-Square (χ²)
- **Definisi:** Distribusi jumlah kuadrat variabel normal standar independen.
- **Digunakan dalam:** Uji goodness-of-fit, uji independensi (tabel kontingensi).

---

## 6. Feature Engineering & Data Preprocessing

### Normalisasi vs Standarisasi
| Teknik | Rumus | Kapan Digunakan |
|--------|-------|-----------------|
| **Min-Max Normalization** | `(x - min) / (max - min)` → [0, 1] | KNN, Neural Network, algoritma berbasis jarak |
| **Standardization (Z-score)** | `(x - μ) / σ` → mean=0, std=1 | SVM, PCA, Logistic Regression |

- **Aturan umum:** Algoritma berbasis jarak **memerlukan** scaling. Tree-based methods **tidak** memerlukannya.

---

### Handling Missing Values
- **Deletion:** Hapus baris/kolom dengan missing value. Cocok jika < 5% data.
- **Mean/Median/Mode Imputation:** Isi dengan nilai statistik. Median lebih robust untuk data skewed.
- **KNN Imputation:** Isi berdasarkan nilai tetangga terdekat.
- **Model-based Imputation:** Prediksi nilai missing menggunakan model ML.

---

### Encoding Kategorikal
| Teknik | Kapan Digunakan |
|--------|-----------------|
| **One-Hot Encoding** | Kategori nominal tanpa urutan, jumlah kategori sedikit |
| **Label Encoding** | Kategori ordinal (ada urutan: rendah, sedang, tinggi) |
| **Target Encoding** | Kategori dengan banyak nilai unik (high cardinality) |
| **Binary Encoding** | Kompromi antara one-hot dan label encoding |

---

### Outlier
- **Definisi:** Titik data yang jauh berbeda dari mayoritas data.
- **Deteksi:**
  - **IQR Method:** Outlier = nilai di luar [Q1 - 1.5×IQR, Q3 + 1.5×IQR]
  - **Z-score:** Outlier = |z| > 3
  - **Isolation Forest:** Algoritma ML untuk deteksi anomali.
- **Penanganan:** Hapus, cap (winsorizing), transformasi log, atau pertahankan jika informasi penting.

---

### Feature Selection
- **Filter Methods:** Univariate statistical tests, Correlation matrix.
- **Wrapper Methods:** RFE (Recursive Feature Elimination) — iteratif, gunakan model.
- **Embedded Methods:** L1 regularization (Lasso), Feature importance dari Random Forest/XGBoost.

---

### Class Imbalance
- **Masalah:** Jika kelas mayoritas jauh lebih banyak, model cenderung mengabaikan kelas minoritas.
- **Solusi:**
  - **Oversampling:** SMOTE (Synthetic Minority Over-sampling Technique)
  - **Undersampling:** Kurangi kelas mayoritas
  - **Class Weights:** Beri bobot lebih besar pada kelas minoritas
  - **Ganti metrik:** Gunakan F1, AUC-ROC, bukan accuracy

---

## 7. Deep Learning

### Neural Network
- **Arsitektur dasar:** Input layer → Hidden layers → Output layer
- **Activation Functions:**
  | Fungsi | Rumus | Kegunaan |
  |--------|-------|----------|
  | **ReLU** | max(0, x) | Hidden layers (paling umum) |
  | **Sigmoid** | 1/(1+e⁻ˣ) | Output biner |
  | **Softmax** | eˣⁱ/Σeˣʲ | Output multi-kelas |
  | **Tanh** | (eˣ-e⁻ˣ)/(eˣ+e⁻ˣ) | Hidden layers, output [-1, 1] |

---

### Backpropagation
- **Definisi:** Algoritma untuk menghitung gradien loss terhadap setiap bobot dalam neural network menggunakan chain rule.
- **Proses:** Forward pass (hitung output) → Hitung loss → Backward pass (hitung gradien) → Update bobot.

---

### Batch Normalization
- **Tujuan:** Normalisasi input setiap layer selama training untuk stabilisasi dan mempercepat training.
- **Efek:** Mengurangi internal covariate shift, bertindak sebagai regularizer ringan.

---

### Dropout
- **Definisi:** Teknik regularisasi di mana neuron secara acak "dimatikan" selama training dengan probabilitas p.
- **Tujuan:** Mencegah overfitting, memaksa network belajar representasi yang lebih robust.
- **Catatan:** Dropout hanya aktif saat training, tidak saat inferensi.

---

### Convolutional Neural Network (CNN)
- **Digunakan untuk:** Pengolahan gambar, video, sinyal 1D.
- **Komponen:** Convolutional layer (ekstraksi fitur), Pooling layer (reduksi dimensi), Fully connected layer (klasifikasi).

---

### Recurrent Neural Network (RNN) / LSTM / GRU
- **Digunakan untuk:** Data sekuensial — teks, time series, audio.
- **Masalah RNN:** Vanishing gradient untuk sekuens panjang.
- **LSTM:** Mengatasi vanishing gradient dengan cell state dan gates (input, forget, output).
- **GRU:** Versi sederhana LSTM dengan performa serupa.

---

### Transformer & Attention Mechanism
- **Attention:** Memungkinkan model fokus pada bagian input yang relevan saat menghasilkan output.
- **Self-Attention:** Setiap token memperhatikan semua token lain dalam sekuens.
- **Transformer:** Arsitektur dasar model bahasa modern (BERT, GPT).

---

## 8. Validasi & Seleksi Model

### Cross-Validation
- **k-Fold CV:** Bagi data menjadi k subset; gunakan k-1 untuk training, 1 untuk validasi, rotasi k kali. Rata-rata performanya.
- **Stratified k-Fold:** Pastikan setiap fold memiliki proporsi kelas yang sama. Penting untuk data imbalanced.
- **Leave-One-Out (LOO):** k = n. Sangat akurat tapi lambat untuk dataset besar.

---

### Train / Validation / Test Split
- **Training set:** Data untuk melatih model.
- **Validation set:** Data untuk tuning hyperparameter dan pemilihan model.
- **Test set:** Data untuk evaluasi akhir — **HANYA DIGUNAKAN SEKALI!**
- **Aturan umum:** 70/15/15 atau 80/10/10.

---

### Hyperparameter Tuning
| Metode | Deskripsi | Kelebihan/Kekurangan |
|--------|-----------|----------------------|
| **Grid Search** | Coba semua kombinasi | Exhaustive tapi lambat |
| **Random Search** | Sampling acak | Lebih efisien dari grid search |
| **Bayesian Optimization** | Gunakan model probabilistik | Paling efisien, kompleks |

---

### Learning Curve
- **Definisi:** Plot training vs validation error terhadap ukuran training data atau iterasi.
- **Diagnosa:**
  - Keduanya tinggi → Underfitting
  - Training rendah, validation tinggi → Overfitting
  - Keduanya rendah & konvergen → Model baik

---

## 9. Terminologi Umum Sains Data

### Terminologi Data

| Istilah | Definisi |
|---------|----------|
| **Feature / Variabel Independen** | Kolom input yang digunakan model |
| **Label / Target / Variabel Dependen** | Kolom yang ingin diprediksi |
| **Instance / Sampel** | Satu baris data |
| **Dimensionality** | Jumlah fitur/kolom |
| **Multicollinearity** | Dua atau lebih fitur berkorelasi tinggi satu sama lain |
| **Data Leakage** | Informasi dari test set bocor ke proses training — hasil evaluasi jadi tidak valid |

---

### Terminologi Model

| Istilah | Definisi |
|---------|----------|
| **Inference** | Menggunakan model yang sudah dilatih untuk membuat prediksi |
| **Hyperparameter** | Parameter yang diset sebelum training (learning rate, depth) |
| **Parameter** | Nilai yang dipelajari model selama training (bobot) |
| **Loss Function** | Fungsi yang mengukur seberapa salah prediksi model |
| **Objective Function** | Fungsi yang dioptimalkan (biasanya meminimalkan loss) |
| **Epoch** | Satu kali pass lengkap seluruh data training |
| **Batch Size** | Jumlah sampel diproses sebelum update bobot |

---

### Terminologi Statistik Lanjutan

| Istilah | Definisi |
|---------|----------|
| **Central Limit Theorem** | Rata-rata sampel berdistribusi normal jika n cukup besar, terlepas dari distribusi populasi |
| **Law of Large Numbers** | Rata-rata sampel mendekati rata-rata populasi seiring bertambahnya n |
| **Multivariate** | Melibatkan lebih dari dua variabel |
| **Heteroskedastisitas** | Variance residual tidak konstan — melanggar asumsi regresi linier |
| **Autocorrelation** | Korelasi nilai dengan nilai sebelumnya dalam time series |
| **Stationarity** | Properti time series di mana mean & variance konstan sepanjang waktu |

---

### CRISP-DM (Proses Standar Sains Data)
```
1. Business Understanding  →  Apa yang ingin dicapai?
2. Data Understanding      →  Data apa yang tersedia?
3. Data Preparation        →  Cleaning, transformasi, feature engineering
4. Modeling                →  Pilih & latih algoritma
5. Evaluation              →  Apakah model memenuhi tujuan bisnis?
6. Deployment              →  Implementasi ke produksi
```

---

*Dokumen ini dibuat sebagai referensi cepat. Untuk pemahaman lebih dalam, selalu eksplorasi dengan data nyata.*

> **Terakhir diperbarui:** April 2026
