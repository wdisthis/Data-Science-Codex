# Data Science Codex — Obsidian Vault Wiki

Selamat datang di **Data Science Codex**, sebuah basis pengetahuan (*knowledge base*) komprehensif mengenai Data Science yang disusun menggunakan metode **Zettelkasten** dan **MOC (Map of Content)** di dalam **Obsidian**.

Proyek ini mentransformasi catatan monolitik menjadi jaringan konsep atomik yang saling terhubung, memudahkan navigasi dan pembelajaran terstruktur.

---

## Daftar Isi (MOC)

Vault ini dibagi menjadi 14 kategori utama yang mencakup seluruh spektrum Data Science:

| No | Kategori | Deskripsi |
|:---|:---|:---|
| 01 | **Statistika & Matematika** | Statistik, probabilitas, distribusi, aljabar linear |
| 02 | **Machine Learning** | Algoritma, konsep dasar, supervised/unsupervised |
| 03 | **Evaluasi Model** | Metrik, validasi, tuning, cross-validation |
| 04 | **Feature Engineering** | Preprocessing, encoding, scaling, outlier handling |
| 05 | **Deep Learning** | Neural network, CNN, RNN, Transformer |
| 06 | **NLP & Computer Vision** | Pemrosesan teks, gambar, LLM |
| 07 | **Python & Coding** | Python, library (Pandas, NumPy), coding patterns |
| 08 | **SQL & Database** | Query, database design, data warehouse |
| 09 | **Visualisasi Data** | Tipe chart, tools (Tableau, Power BI), dashboard |
| 10 | **Business Intelligence** | KPI, A/B testing, analitik bisnis |
| 11 | **MLOps & Deployment** | Deployment, Docker, CI/CD, monitoring |
| 12 | **Linux & DevOps** | Terminal, bash, konfigurasi server, WSL |
| 13 | **Pengembangan Aplikasi** | Git, web dev, metodologi agile |
| 14 | **Terminologi Umum** | Glosarium istilah-istilah umum sains data |
| 15 | **R & RStudio** | Statistika, RMarkdown, Tidyverse, ggplot2 |

---

## Struktur Direktori

```text
Data-Science-Codex/
├── 00 Home.md                          ← Hub utama, pintu masuk ke semua MOC
├── _arsip/
│   └── Kompendium Genesis.md           ← File monolitik asli
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
│   ├── SQL.md
│   ├── Data Definition Language.md
│   ├── Data Manipulation Language.md
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
│   ├── INSERT UPDATE DELETE.md
│   ├── CREATE TABLE.md
│   ├── ALTER.md
│   ├── DROP.md
│   ├── TRUNCATE.md
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
│   └── Multivariate.md
│
├── 15 R & RStudio/
│   ├── _MOC R & RStudio.md
│   ├── R Basics.md                    ← stub
│   ├── RStudio.md                     ← stub
│   ├── Tidyverse.md                   ← stub
│   ├── ggplot2.md                     ← stub
│   ├── dplyr.md                       ← stub
│   ├── R Markdown.md                  ← stub
│   ├── Data Types R.md                ← stub
│   └── Data Frame R.md                ← stub
│
└── .obsidian/
```

---

## Cara Membuka (Via Obsidian)

Untuk mendapatkan pengalaman terbaik (grafik koneksi, backlink, dan navigasi otomatis), sangat disarankan membuka folder ini menggunakan **Obsidian**.

1.  **Download & Install Obsidian**:
    Unduh aplikasinya di [obsidian.md](https://obsidian.md/).
2.  **Clone atau Download Repositori Ini**:
    Pastikan semua folder dan file `.md` berada dalam satu direktori.
3.  **Buka Vault**:
    - Jalankan Obsidian.
    - Pilih **"Open folder as vault"**.
    - Pilih folder `Data-Science-Codex`.
4.  **Mulai Navigasi**:
    Buka file `00 Home.md` sebagai titik awal navigasi Anda.

---

## Fitur Utama

-   **Atomic Notes**: Setiap konsep dijelaskan dalam satu file terpisah untuk fokus maksimal.
-   **Wikilinks**: Navigasi antar konsep menggunakan `[[Nama Konsep]]`.
-   **Graph View**: Visualisasikan hubungan antar ilmu secara interaktif untuk melihat "Big Picture".
-   **MOC (Map of Content)**: Struktur hierarkis yang memudahkan eksplorasi tanpa kehilangan konteks.
-   **Template Ready**: Gunakan folder `_templates` untuk membuat catatan baru dengan metadata (YAML frontmatter) yang konsisten.

---

## Taksonomi Tag

Proyek ini menggunakan tag hierarkis untuk mempermudah pencarian dan pengelompokan otomatis:

-   `#statistik`: `#statistik/deskriptif`, `#statistik/inferensial`, dll.
-   `#ml`: `#ml/supervised`, `#ml/unsupervised`, `#ml/ensemble`, dll.
-   `#python`: `#python/dasar`, `#python/library`, `#python/data`.
-   `#evaluasi`: `#evaluasi/klasifikasi`, `#evaluasi/regresi`.
-   `#bisnis`: `#bisnis/metrik`, `#bisnis/analisis`.

---

## Link Penting

-   **Official Website**: [Obsidian.md](https://obsidian.md/)
-   **Dokumentasi Obsidian**: [Obsidian Help](https://help.obsidian.md/)
-   **Metode Zettelkasten**: [Zettelkasten Method](https://zettelkasten.de/introduction/)

---
> *"The palest ink is better than the best memory."*
