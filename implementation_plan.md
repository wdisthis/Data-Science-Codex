# Data Science Codex — Obsidian Vault Wiki

Transformasi file monolitik `kamus_sains_data.md` (530 baris) menjadi vault Obsidian bergaya Wikipedia dengan **200+ file atomik** yang saling terhubung.

## Status Saat Ini

- Sudah ada 1 file monolitik `kamus_sains_data.md` berisi ~50 istilah
- Vault `.obsidian/` sudah ada (graph view, core-plugins aktif)
- **Rencana:** File lama akan dipertahankan sebagai arsip, semua konten dipecah ke file-file baru

---

## Arsitektur Vault

### Prinsip Desain
1. **Atomic notes** — 1 konsep = 1 file
2. **MOC (Map of Content)** — setiap folder punya `_MOC *.md` sebagai halaman indeks
3. **YAML frontmatter** — tags, aliases, date, status
4. **Wikilinks `[[...]]`** — semua referensi antar konsep pakai backlink
5. **Tag taxonomy** — hierarkis (e.g. `#statistik/inferensial`, `#ml/supervised`)
6. **Stub files** — topik yang belum dikuasai dibuat sebagai file kosong bertanda `status: stub`

### Struktur Folder

```
Data-Science-Codex/
├── 00 Home.md                          ← Hub utama, pintu masuk ke semua MOC
├── _arsip/
│   └── kamus_sains_data.md             ← File lama dipindah ke sini
├── _templates/
│   ├── Template Istilah.md
│   └── Template MOC.md
│
├── 01 Statistika & Matematika/
│   ├── _MOC Statistika & Matematika.md
│   ├── P-Value.md
│   ├── Hipotesis.md
│   ├── Confidence Interval.md
│   ├── Type I dan Type II Error.md
│   ├── Korelasi vs Kausalitas.md
│   ├── Variance.md
│   ├── Standard Deviation.md
│   ├── Skewness.md
│   ├── Kurtosis.md
│   ├── Central Limit Theorem.md
│   ├── Law of Large Numbers.md
│   ├── ANOVA.md                        ← stub
│   ├── T-Test.md                       ← stub
│   ├── Chi-Square Test.md              ← stub
│   ├── Mann-Whitney U Test.md          ← stub
│   ├── Distribusi Normal.md
│   ├── Distribusi Binomial.md
│   ├── Distribusi Poisson.md
│   ├── Distribusi Uniform.md
│   ├── Distribusi Eksponensial.md
│   ├── Distribusi Bernoulli.md
│   ├── Distribusi t-Student.md
│   ├── Distribusi Chi-Square.md
│   ├── Distribusi Log-Normal.md        ← stub
│   ├── Distribusi Gamma.md             ← stub
│   ├── Probabilitas.md                 ← stub
│   ├── Teorema Bayes.md                ← stub
│   ├── Aljabar Linear.md              ← stub
│   ├── Eigenvalue dan Eigenvector.md   ← stub
│   ├── Matriks.md                      ← stub
│   ├── Turunan dan Gradien.md          ← stub
│   ├── Heteroskedastisitas.md
│   ├── Autocorrelation.md
│   └── Stationarity.md
│
├── 02 Machine Learning/
│   ├── _MOC Machine Learning.md
│   ├── Supervised Learning.md
│   ├── Unsupervised Learning.md
│   ├── Reinforcement Learning.md
│   ├── Semi-Supervised Learning.md     ← stub
│   ├── Bias-Variance Tradeoff.md
│   ├── Overfitting.md
│   ├── Underfitting.md
│   ├── Regularisasi.md
│   ├── Gradient Descent.md
│   ├── Loss Function.md               ← stub
│   ├── Learning Rate.md               ← stub
│   ├── Linear Regression.md
│   ├── Logistic Regression.md
│   ├── Decision Tree.md
│   ├── Random Forest.md
│   ├── Gradient Boosting.md
│   ├── XGBoost.md                      ← stub
│   ├── LightGBM.md                     ← stub
│   ├── CatBoost.md                     ← stub
│   ├── SVM.md
│   ├── KNN.md
│   ├── Naive Bayes.md                  ← stub
│   ├── K-Means.md
│   ├── DBSCAN.md                       ← stub
│   ├── Hierarchical Clustering.md      ← stub
│   ├── PCA.md
│   ├── t-SNE.md                        ← stub
│   ├── UMAP.md                         ← stub
│   ├── Ensemble Methods.md            ← stub
│   ├── Bagging.md                      ← stub
│   ├── Boosting.md                     ← stub
│   ├── Stacking.md                     ← stub
│   ├── Anomaly Detection.md           ← stub
│   └── Recommendation System.md       ← stub
│
├── 03 Evaluasi Model/
│   ├── _MOC Evaluasi Model.md
│   ├── Confusion Matrix.md
│   ├── Accuracy.md
│   ├── Precision.md
│   ├── Recall.md
│   ├── F1-Score.md
│   ├── AUC-ROC.md
│   ├── Specificity.md
│   ├── MAE.md
│   ├── MSE.md
│   ├── RMSE.md
│   ├── R-Squared.md
│   ├── MAPE.md
│   ├── Log Loss.md                     ← stub
│   ├── Silhouette Score.md             ← stub
│   ├── Cross Validation.md
│   ├── Train-Validation-Test Split.md
│   ├── Hyperparameter Tuning.md
│   ├── Learning Curve.md
│   ├── Grid Search.md                  ← stub
│   ├── Random Search.md                ← stub
│   └── Bayesian Optimization.md        ← stub
│
├── 04 Feature Engineering & Data Preprocessing/
│   ├── _MOC Feature Engineering.md
│   ├── Normalisasi vs Standarisasi.md
│   ├── Handling Missing Values.md
│   ├── Encoding Kategorikal.md
│   ├── One-Hot Encoding.md             ← stub
│   ├── Label Encoding.md              ← stub
│   ├── Target Encoding.md             ← stub
│   ├── Outlier.md
│   ├── Feature Selection.md
│   ├── Feature Extraction.md          ← stub
│   ├── Class Imbalance.md
│   ├── SMOTE.md                        ← stub
│   ├── Data Leakage.md
│   ├── Data Cleaning.md               ← stub
│   ├── Data Transformation.md         ← stub
│   ├── Binning.md                      ← stub
│   └── Feature Scaling.md             ← stub
│
├── 05 Deep Learning/
│   ├── _MOC Deep Learning.md
│   ├── Neural Network.md
│   ├── Activation Function.md
│   ├── Backpropagation.md
│   ├── Batch Normalization.md
│   ├── Dropout.md
│   ├── CNN.md
│   ├── RNN.md
│   ├── LSTM.md
│   ├── GRU.md
│   ├── Transformer.md
│   ├── Attention Mechanism.md
│   ├── GAN.md                          ← stub
│   ├── Autoencoder.md                  ← stub
│   ├── VAE.md                          ← stub
│   ├── Transfer Learning.md           ← stub
│   ├── Fine-Tuning.md                 ← stub
│   ├── Optimizer.md                    ← stub
│   ├── Adam.md                         ← stub
│   ├── Vanishing Gradient.md          ← stub
│   ├── Weight Initialization.md       ← stub
│   └── Epoch dan Batch Size.md
│
├── 06 NLP & Computer Vision/
│   ├── _MOC NLP & Computer Vision.md
│   ├── Tokenization.md                ← stub
│   ├── Word Embedding.md              ← stub
│   ├── Word2Vec.md                     ← stub
│   ├── TF-IDF.md                       ← stub
│   ├── Bag of Words.md                ← stub
│   ├── BERT.md                         ← stub
│   ├── GPT.md                          ← stub
│   ├── Sentiment Analysis.md          ← stub
│   ├── Named Entity Recognition.md    ← stub
│   ├── Image Classification.md        ← stub
│   ├── Object Detection.md            ← stub
│   ├── Image Segmentation.md          ← stub
│   ├── Data Augmentation.md           ← stub
│   └── LLM.md                         ← stub
│
├── 07 Python & Coding/
│   ├── _MOC Python.md
│   ├── Python Basics.md               ← stub
│   ├── Data Types Python.md           ← stub
│   ├── List Comprehension.md          ← stub
│   ├── Lambda Function.md             ← stub
│   ├── Decorator.md                    ← stub
│   ├── Generator.md                    ← stub
│   ├── OOP Python.md                  ← stub
│   ├── Exception Handling.md          ← stub
│   ├── Virtual Environment.md         ← stub
│   ├── Pip.md                          ← stub
│   ├── Conda.md                        ← stub
│   ├── Jupyter Notebook.md            ← stub
│   ├── Pandas.md                       ← stub
│   ├── NumPy.md                        ← stub
│   ├── Scikit-Learn.md                ← stub
│   ├── Matplotlib.md                  ← stub
│   ├── Seaborn.md                     ← stub
│   ├── TensorFlow.md                  ← stub
│   ├── PyTorch.md                     ← stub
│   ├── Keras.md                        ← stub
│   ├── SciPy.md                        ← stub
│   ├── Statsmodels.md                 ← stub
│   ├── XGBoost Library.md             ← stub
│   ├── Regex Python.md                ← stub
│   ├── File IO Python.md             ← stub
│   ├── JSON Handling.md               ← stub
│   ├── Web Scraping.md                ← stub
│   ├── Beautiful Soup.md              ← stub
│   ├── Requests Library.md            ← stub
│   └── Type Hints.md                  ← stub
│
├── 08 SQL & Database/
│   ├── _MOC SQL.md
│   ├── SELECT.md                       ← stub
│   ├── WHERE.md                        ← stub
│   ├── JOIN.md                         ← stub
│   ├── GROUP BY.md                     ← stub
│   ├── HAVING.md                       ← stub
│   ├── ORDER BY.md                     ← stub
│   ├── Subquery.md                     ← stub
│   ├── CTE.md                          ← stub
│   ├── Window Function.md             ← stub
│   ├── UNION.md                        ← stub
│   ├── INSERT UPDATE DELETE.md         ← stub
│   ├── CREATE TABLE.md                ← stub
│   ├── Index Database.md              ← stub
│   ├── Normalisasi Database.md        ← stub
│   ├── Primary Key dan Foreign Key.md ← stub
│   ├── ACID.md                         ← stub
│   ├── Transaction.md                 ← stub
│   ├── PostgreSQL.md                  ← stub
│   ├── MySQL.md                        ← stub
│   ├── SQLite.md                       ← stub
│   ├── NoSQL.md                        ← stub
│   ├── MongoDB.md                     ← stub
│   ├── Redis.md                        ← stub
│   ├── Data Warehouse.md              ← stub
│   ├── Data Lake.md                    ← stub
│   ├── ETL.md                          ← stub
│   ├── ELT.md                          ← stub
│   └── Star Schema vs Snowflake.md    ← stub
│
├── 09 Visualisasi Data/
│   ├── _MOC Visualisasi Data.md
│   ├── Prinsip Visualisasi.md         ← stub
│   ├── Bar Chart.md                    ← stub
│   ├── Line Chart.md                  ← stub
│   ├── Scatter Plot.md                ← stub
│   ├── Histogram.md                   ← stub
│   ├── Box Plot.md                    ← stub
│   ├── Heatmap.md                     ← stub
│   ├── Pie Chart.md                   ← stub
│   ├── Violin Plot.md                 ← stub
│   ├── Pair Plot.md                   ← stub
│   ├── Choropleth Map.md              ← stub
│   ├── Dashboard.md                   ← stub
│   ├── Tableau.md                      ← stub
│   ├── Power BI.md                    ← stub
│   ├── Plotly.md                       ← stub
│   ├── D3js.md                         ← stub
│   ├── Looker.md                       ← stub
│   ├── Metabase.md                    ← stub
│   └── Streamlit Visualisasi.md       ← stub
│
├── 10 Business Intelligence/
│   ├── _MOC Business Intelligence.md
│   ├── KPI.md                          ← stub
│   ├── A-B Testing.md                 ← stub
│   ├── Cohort Analysis.md             ← stub
│   ├── Funnel Analysis.md             ← stub
│   ├── Customer Segmentation.md       ← stub
│   ├── Churn Analysis.md              ← stub
│   ├── RFM Analysis.md                ← stub
│   ├── ROI.md                          ← stub
│   ├── CLV.md                          ← stub
│   ├── Data-Driven Decision.md        ← stub
│   ├── CRISP-DM.md
│   ├── Stakeholder Communication.md   ← stub
│   ├── Product Analytics.md           ← stub
│   ├── Market Basket Analysis.md      ← stub
│   └── Time Series Forecasting.md     ← stub
│
├── 11 MLOps & Deployment/
│   ├── _MOC MLOps.md
│   ├── Docker.md                       ← stub
│   ├── Kubernetes.md                  ← stub
│   ├── CI-CD.md                        ← stub
│   ├── Model Serving.md              ← stub
│   ├── Model Monitoring.md           ← stub
│   ├── Model Versioning.md           ← stub
│   ├── MLflow.md                       ← stub
│   ├── DVC.md                          ← stub
│   ├── Feature Store.md              ← stub
│   ├── API.md                          ← stub
│   ├── REST API.md                    ← stub
│   ├── Flask.md                        ← stub
│   ├── FastAPI.md                     ← stub
│   ├── Streamlit.md                   ← stub
│   ├── Gradio.md                       ← stub
│   ├── Cloud Computing.md            ← stub
│   ├── AWS Basics.md                  ← stub
│   ├── GCP Basics.md                  ← stub
│   └── Model Registry.md             ← stub
│
├── 12 Linux & DevOps/
│   ├── _MOC Linux.md
│   ├── Terminal Commands.md           ← stub
│   ├── Bash Scripting.md             ← stub
│   ├── File System Linux.md          ← stub
│   ├── SSH.md                          ← stub
│   ├── Package Manager.md            ← stub
│   ├── Apt.md                          ← stub
│   ├── Cron Job.md                    ← stub
│   ├── Nginx.md                        ← stub
│   ├── WSL.md                          ← stub
│   ├── Systemd.md                     ← stub
│   ├── Permissions Linux.md          ← stub
│   ├── Environment Variables.md      ← stub
│   ├── Vim Basics.md                  ← stub
│   └── Tmux.md                         ← stub
│
├── 13 Pengembangan Aplikasi/
│   ├── _MOC Pengembangan Aplikasi.md
│   ├── Git.md                          ← stub
│   ├── GitHub.md                       ← stub
│   ├── Git Branching.md               ← stub
│   ├── Frontend Basics.md            ← stub
│   ├── HTML.md                         ← stub
│   ├── CSS.md                          ← stub
│   ├── JavaScript Basics.md          ← stub
│   ├── Backend Basics.md             ← stub
│   ├── Markdown.md                    ← stub
│   ├── Agile.md                        ← stub
│   ├── Scrum.md                        ← stub
│   └── Design Patterns.md            ← stub
│
├── 14 Terminologi Umum/
│   ├── _MOC Terminologi Umum.md
│   ├── Feature.md
│   ├── Label.md
│   ├── Instance.md
│   ├── Dimensionality.md
│   ├── Multicollinearity.md
│   ├── Inference.md
│   ├── Hyperparameter.md
│   ├── Parameter.md
│   ├── Epoch dan Batch Size.md        (shared with Deep Learning)
│   └── Multivariate.md
│
└── .obsidian/
```

**Total file: ~230 file** (termasuk 14 MOC + 2 template + 1 home)

---

## Format Standar Setiap File

### Template Istilah (file berisi konten)

```markdown
---
tags:
  - statistik/inferensial
  - evaluasi
aliases:
  - nilai-p
  - p value
date: 2026-04-28
status: complete
---

# P-Value

> **Ringkasan:** Probabilitas mendapatkan hasil yang sama ekstrem jika H₀ benar.

## Definisi
(penjelasan rinci)

## Interpretasi
(cara baca, threshold, konteks)

## Contoh
(contoh praktis)

## Hubungan dengan Konsep Lain
- Terkait: [[Hipotesis]], [[Confidence Interval]], [[Type I dan Type II Error]]
- Digunakan di: [[T-Test]], [[ANOVA]], [[Chi-Square Test]]

## Referensi
- (opsional)
```

### Template Istilah (stub / file kosong)

```markdown
---
tags:
  - ml/unsupervised
aliases: []
date: 2026-04-28
status: stub
---

# DBSCAN

> **Ringkasan:** *(belum diisi)*

## Definisi

*(topik ini belum ditulis — akan diisi nanti)*

## Hubungan dengan Konsep Lain
- Terkait: [[K-Means]], [[Anomaly Detection]], [[Clustering]]
```

### Template MOC

```markdown
---
tags:
  - moc
  - statistik
date: 2026-04-28
---

# 📊 Statistika & Matematika

> Map of Content untuk semua konsep statistika dan matematika.

## 🔑 Konsep Utama
- [[P-Value]]
- [[Hipotesis]]
- ...

## 📐 Distribusi
- [[Distribusi Normal]]
- ...

## 🧮 Matematika Dasar
- [[Aljabar Linear]]
- ...

## Status
| Konsep | Status |
|--------|--------|
| [[P-Value]] | ✅ complete |
| [[ANOVA]] | 📝 stub |
```

---

## Proposed Changes

### Fase 1: Infrastruktur

#### [NEW] `00 Home.md`
Hub utama vault. Links ke semua 14 MOC. Statistik total file, panduan navigasi.

#### [NEW] `_templates/Template Istilah.md`
Template standar untuk semua note istilah.

#### [NEW] `_templates/Template MOC.md`
Template standar untuk semua MOC.

#### [MOVE] `kamus_sains_data.md` → `_arsip/kamus_sains_data.md`
File lama dipindah ke arsip sebagai referensi.

---

### Fase 2: MOC Files (14 file)

Satu MOC per folder, berisi daftar lengkap semua file di folder tersebut dengan status (complete/stub).

---

### Fase 3: Complete Notes (~60 file)

Konten dari `kamus_sains_data.md` dipecah menjadi file atomik + konten diperkaya dengan backlinks dan tags. Setiap file yang sudah ada kontennya di kamus lama akan berstatus `complete`.

---

### Fase 4: Stub Notes (~160 file)

File kosong dengan frontmatter, ringkasan kosong, dan backlink yang sudah diisi. Berstatus `stub`.

---

## Tag Taxonomy

```
#statistik
  #statistik/deskriptif
  #statistik/inferensial
  #statistik/distribusi
  #statistik/lanjutan
#matematika
  #matematika/aljabar-linear
  #matematika/kalkulus
#ml
  #ml/supervised
  #ml/unsupervised
  #ml/reinforcement
  #ml/ensemble
  #ml/clustering
  #ml/dimensionality-reduction
#evaluasi
  #evaluasi/klasifikasi
  #evaluasi/regresi
  #evaluasi/validasi
#feature-engineering
  #feature-engineering/scaling
  #feature-engineering/encoding
  #feature-engineering/selection
#deep-learning
  #deep-learning/arsitektur
  #deep-learning/teknik
  #deep-learning/optimasi
#nlp
#computer-vision
#python
  #python/dasar
  #python/library
  #python/data
#sql
  #sql/query
  #sql/ddl
  #sql/database
  #sql/data-warehouse
#visualisasi
  #visualisasi/tipe-chart
  #visualisasi/tools
#bisnis
  #bisnis/metrik
  #bisnis/analisis
  #bisnis/proses
#mlops
  #mlops/deployment
  #mlops/monitoring
  #mlops/tools
#linux
  #linux/command
  #linux/konfigurasi
  #linux/tools
#dev
  #dev/version-control
  #dev/web
  #dev/metodologi
#terminologi
```

---

## User Review Required

> [!IMPORTANT]


---

## Verification Plan

### Automated Tests
- Cek semua wikilinks `[[...]]` mengarah ke file yang ada
- Cek semua file punya valid YAML frontmatter
- Cek tidak ada file duplikat

### Manual Verification
- Buka vault di Obsidian → pastikan graph view menampilkan koneksi yang benar
- Navigasi dari `00 Home.md` → MOC → file individual → backlink → file lain
- Verifikasi template berfungsi untuk membuat note baru
