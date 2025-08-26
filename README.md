# Capstone Project: Sentiment Analysis & Insights dari Ulasan Produk Indonesia

## 📌 Project Overview
Proyek ini bertujuan menganalisis ulasan pelanggan e-commerce berbahasa Indonesia untuk memperoleh insight bermakna terkait **sentimen (positif, negatif, netral)** serta **tema utama** dari ulasan pelanggan.  
Analisis ini mendukung pemahaman mendalam terkait persepsi pelanggan dan area perbaikan yang diperlukan oleh penjual.

## 📊 Raw Dataset
Dataset berasal dari Kaggle: [Indonesian Marketplace Product Reviews](https://www.kaggle.com/datasets/taqiyyaghazi/indonesian-marketplace-product-reviews).  
Salinan dataset mentah juga tersedia di repo ini: [`data/raw_dataset/reviews.csv`](https://github.com/MegaGloria/Sentiment-Analysis-Insights-dari-Ulasan-Produk-Indonesia/blob/main/data/raw_dataset/reviews.csv).

## 🔎 Analysis Process
1. Load dataset & preprocessing (pembersihan teks, normalisasi label).
2. Exploratory Data Analysis (EDA) → distribusi sentimen, word cloud.
3. Model AI Granite (via Replicate API) → klasifikasi sentimen otomatis.
4. Theme Mining → menggali tema utama dari ulasan positif & negatif.
5. Evaluasi performa model → confusion matrix, akurasi, precision, recall.

## 💡 Insight & Findings
- **Mayoritas ulasan bersentimen positif (±70%)**, diikuti negatif dan netral.  
- **Pujian utama**: kualitas produk, harga terjangkau, pengiriman cepat.  
- **Keluhan utama**: warna tidak sesuai, ukuran salah, bahan tipis, kemasan jelek.  
- Granite cukup baik membedakan **positif vs negatif**, namun kadang keliru di **netral**.  

## ✅ Recommendations
1. **Perbaikan kualitas**: pastikan warna & ukuran sesuai deskripsi produk.  
2. **Pengemasan**: tingkatkan proteksi saat pengiriman.  
3. **Manfaatkan insight AI**: gunakan otomatisasi untuk memonitor keluhan baru secara real-time.  

## 🤖 AI Support Explanation
Proyek ini menggunakan **IBM Granite Models** melalui Replicate API untuk:  
- **Sentiment Classification** → mengklasifikasikan review ke negatif/netral/positif.  
- **Theme Mining** → menemukan tema utama dari ulasan.  

Notebook analisis: [`notebook/capstone project_megagloria.ipynb`](https://colab.research.google.com/drive/1MVupPRCSR-UG2j6R7EBV_zfPNRoXmg8K?usp=sharing)
