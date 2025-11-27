# Analisis Keamanan Data dan Risiko Privasi pada Bank Marketing Dataset

#### 1. Deskripsi Proyek

Proyek ini bertujuan untuk mengevaluasi tingkat keamanan dan risiko privasi pada Bank Marketing Dataset (UCI/Kaggle) dengan menggunakan dua pendekatan utama: k-anonymity dan l-diversity. Dataset ini berisi informasi demografis dan perilaku nasabah dalam kampanye pemasaran bank, sehingga analisis privasi penting untuk memastikan bahwa data tidak rentan terhadap re-identifikasi dan kebocoran atribut sensitif.

#### 2. Dataset
Sumber: UCI Machine Learning Repository / Kaggle
Jumlah sampel: ±45.000 baris
Jumlah atribut: 17 kolom
Jenis atribut:
- Demografis (usia, pekerjaan, pendidikan, status pernikahan)
- Finansial (pinjaman, kredit, saldo bank)
- Perilaku kampanye (kontak, durasi, outcome)

#### 3. Tujuan Analisis
1. Menilai tingkat keamanan dan kerentanan privasi pada Bank Marketing Dataset.
2. Mengidentifikasi quasi-identifiers yang berpotensi menyebabkan re-identifikasi individu.
3. Mengukur tingkat anonimitas data menggunakan K-Anonymity.
4. Mengevaluasi keberagaman nilai sensitif menggunakan L-Diversity.
5. Menentukan risiko identity disclosure dan attribute disclosure berdasarkan hasil evaluasi

#### 4. Metodologi
1. Data Loading
2. Identifikasi Atribut
3. Perhitungan K-Anonymity
4. Perhitungan L-Diversity
5. Analisis Risiko Privasi

#### 5. Hasil Utama
- K-Anonymity:
Sebagian besar kombinasi QI memiliki nilai k = 1, yang berarti tiap baris memiliki kombinasi unik dan rawan re-identifikasi.
Hanya sedikit yang mencapai k = 2.

- L-Diversity:
Hampir semua grup memiliki l = 1, menandakan bahwa tiap grup hanya berisi satu nilai sensitif yang sama.
Hal ini menunjukkan bahwa dataset tidak memenuhi standar privasi yang baik.

- Risiko privasi:
Dataset memiliki risiko tinggi terhadap identity disclosure dan attribute disclosure.

#### 6. Cara Menjalankan
1. Install dependencies: `pip install pandas numpy matplotlib seaborn`
2. Download dataset
3. Jalankan notebook
4. Buka file analisis dan jalankan
