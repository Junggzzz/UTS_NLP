# UTS Natural Language Processing - Text Similarity Search
**Nama:** Anak Agung Anantavirya Sadhaka
**NIM:** 2301020079
**Program Studi:** Teknik Informatika
**Universitas:** Primakara University

---

## Deskripsi Proyek
Proyek ini merupakan tugas Ujian Tengah Semester (UTS) untuk mata kuliah **Natural Language Processing (NLP)**. Fokus utama dari proyek ini adalah mengimplementasikan pencarian kemiripan teks (*text similarity*) menggunakan dataset **20 Newsgroups** dari Scikit-Learn.

Sistem ini membandingkan dua metode ekstraksi fitur teks yang umum digunakan:
1. **Bag of Words (BoW)**: Menggunakan `CountVectorizer` untuk menghitung frekuensi kemunculan kata.
2. **TF-IDF (Term Frequency-Inverse Document Frequency)**: Menggunakan `TfidfVectorizer` untuk menghitung bobot kata berdasarkan kepentingan relatifnya dalam dokumen dan seluruh korpus.

## Fitur Utama
- **Data Preprocessing**: Melakukan pembersihan dataset dengan menghapus header, footer, dan kutipan untuk memastikan kualitas data.
- **Text Cleaning**: Tokenisasi, penghapusan stop words, dan normalisasi teks menggunakan library NLTK dan Gensim.
- **Cosine Similarity**: Menghitung skor kemiripan antara input query pengguna dengan ribuan dokumen di dalam dataset.
- **Comparison Analysis**: Menampilkan perbandingan hasil antara metode BoW dan TF-IDF untuk menunjukkan efektivitas TF-IDF dalam menangani kata-kata umum.

## Dataset
Dataset yang digunakan adalah **20 Newsgroups**, yang merupakan kumpulan sekitar 20.000 dokumen newsgroup, yang tersebar di 20 newsgroup berbeda.

## Cara Penggunaan
1. Buka file `UTS.ipynb` di Google Colab atau Jupyter Notebook.
2. Jalankan semua cell untuk memuat data dan melatih vectorizer.
3. Masukkan query pada bagian pencarian untuk melihat hasil perbandingan.

## Hasil Analisis
Berdasarkan hasil pengujian, metode **TF-IDF** secara konsisten memberikan hasil pencarian yang lebih relevan dibandingkan **Bag of Words**. Hal ini dikarenakan TF-IDF mampu memberikan bobot rendah pada kata-kata yang terlalu sering muncul (seperti 'the', 'is', 'and') sehingga pencarian lebih fokus pada kata kunci unik.

---
© 2026 Anak Agung Anantavirya Sadhaka
