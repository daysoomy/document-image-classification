# Klasifikasi Gambar Dokumen (Document Image Classification)

Proyek Machine Learning untuk mengklasifikasikan gambar dokumen ke dalam 16 kategori menggunakan metode Deep Learning dan Transfer Learning dengan arsitektur EfficientNet-B2.

## 1. Gambaran Umum Proyek

Proyek ini bertujuan untuk mengembangkan model klasifikasi gambar yang mampu mengenali dan mengategorikan berbagai jenis dokumen secara otomatis berdasarkan karakteristik visualnya.

Proyek ini dikerjakan menggunakan dataset dari kompetisi Kaggle **Document Image Classification**.

## 2. Latar Belakang

Pengelolaan dokumen dalam jumlah besar membutuhkan proses identifikasi dan pengelompokan yang efisien. Proses klasifikasi secara manual dapat memerlukan waktu dan tenaga, terutama ketika jumlah dokumen semakin banyak.

Oleh karena itu, diperlukan pendekatan berbasis Machine Learning yang dapat membantu mengidentifikasi jenis dokumen secara otomatis melalui citra atau gambar dokumen.

## 3. Dataset

Dataset diperoleh dari kompetisi Kaggle:

[Document Image Classification](https://www.kaggle.com/competitions/document-image-classification-sd234504)

Informasi dataset:
- Jumlah data latih: 32.003 gambar
- Jumlah data uji: 7.994 gambar
- Jumlah kelas: 16 kategori

### Kategori Dokumen

Model dikembangkan untuk mengklasifikasikan dokumen ke dalam 16 kategori berikut:

1. Advertisement
2. Budget
3. Email
4. File Folder
5. Form
6. Handwritten
7. Invoice
8. Letter
9. Memo
10. News Article
11. Presentation
12. Questionnaire
13. Resume
14. Scientific Publication
15. Scientific Report
16. Specification

## 4. Metodologi

Tahapan pengerjaan proyek meliputi:

1. **Data Loading:** Memuat dataset gambar dan informasi label.
2. **Exploratory Data Analysis:** Memahami karakteristik dan distribusi data.
3. **Data Preprocessing:** Melakukan penyesuaian ukuran dan transformasi gambar.
4. **Data Splitting:** Membagi dataset menjadi data latih dan validasi.
5. **Model Development:** Mengembangkan model klasifikasi menggunakan EfficientNet-B2.
6. **Model Training:** Melatih model menggunakan data latih.
7. **Model Evaluation:** Mengevaluasi performa model menggunakan data validasi.
8. **Prediction:** Menghasilkan prediksi terhadap data uji.
9. **Submission:** Menyusun hasil prediksi dalam format submission Kaggle.

## 5. Arsitektur Model

Model utama yang digunakan adalah **EfficientNet-B2** dengan bobot pretrained dari ImageNet.

Pendekatan Transfer Learning digunakan untuk memanfaatkan pengetahuan yang telah diperoleh model dari dataset ImageNet, kemudian menyesuaikannya dengan permasalahan klasifikasi gambar dokumen.

### Konfigurasi Model

| Parameter | Konfigurasi |
|---|---|
| Arsitektur | EfficientNet-B2 |
| Pretrained Weights | ImageNet |
| Ukuran Input | 260 × 260 piksel |
| Optimizer | AdamW |
| Learning Rate | 0.0002 |
| Maksimum Epoch | 5 |
| Loss Function | Cross Entropy dengan Label Smoothing |
| Platform Training | Google Colab GPU |

## 6. Hasil dan Evaluasi

Berdasarkan hasil eksperimen dan pengujian pada kompetisi Kaggle, diperoleh hasil sebagai berikut:

| Metrik | Hasil |
|---|---:|
| Kaggle Public Score | **0.86198** |
| Peringkat Leaderboard | **28** |

Hasil tersebut merupakan performa pada public leaderboard saat submission dilakukan.

## 7. Teknologi yang Digunakan

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Scikit-learn
- Pillow (PIL)
- Google Colab
- Kaggle

## 8. Struktur Repository

```text
document-image-classification/
│
├── README.md
├── .gitignore
├── document_image_classification.ipynb
└── requirements.txt
```
