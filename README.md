# UTS Natural Language Processing - Information Retrieval System

| Informasi Mahasiswa | |
|---|---|
| **Nama** | Anak Agung Anantavirya Sadhaka |
| **NIM** | 2301020079 |
| **Program Studi** | Teknik Informatika |
| **Universitas** | Primakara University |

---

## 📋 Tema Proyek
**Sistem Pencarian Dokumen (Information Retrieval)** *Membangun sistem untuk menemukan dokumen paling relevan berdasarkan query pengguna menggunakan teknik pembobotan kata (TF-IDF).*

## 📖 Deskripsi Proyek
Proyek ini merupakan tugas **Ujian Tengah Semester (UTS)** mata kuliah **Natural Language Processing (NLP)**. Implementasi ini bertujuan untuk mensimulasikan bagaimana mesin pencari bekerja dalam menentukan relevansi sebuah dokumen terhadap kueri tertentu menggunakan dataset **20 Newsgroups**.

Proyek ini membandingkan dua pendekatan ekstraksi fitur teks:
1. **Bag of Words (BoW)**: Representasi teks berbasis frekuensi kemunculan kata mentah.
2. **TF-IDF (Term Frequency-Inverse Document Frequency)**: Representasi teks berbasis bobot statistik yang mempertimbangkan kepentingan kata dalam seluruh korpus.

## ✨ Fitur Utama
- **Data Preprocessing**: Memuat dataset dengan filter `remove=('headers', 'footers', 'quotes')` untuk memastikan hasil pencarian murni berdasarkan konten berita, bukan metadata email.
- **Advanced Text Cleaning**: Implementasi tokenisasi, penghapusan *stop words*, dan normalisasi teks menggunakan library **NLTK** dan **Gensim**.
- **Similarity Scoring**: Menggunakan **Cosine Similarity** untuk menghitung kedekatan vektor antara kueri pengguna dengan ribuan dokumen dalam dataset.
- **Performance Comparison**: Analisis komparatif yang membuktikan keunggulan TF-IDF dalam menyaring informasi yang relevan secara semantik.

## 📊 Dataset
Dataset yang digunakan adalah **20 Newsgroups** via Scikit-Learn. Dataset ini berisi koleksi dokumen berita yang mencakup berbagai topik seperti sains, politik, teknologi, dan hobi, yang sangat ideal untuk pengujian sistem *Information Retrieval*.

## 🚀 Cara Penggunaan
1. Unggah file `UTS.ipynb` ke **Google Colab** atau jalankan di Jupyter Notebook lokal.
2. Pastikan dependensi berikut sudah terpasang:
   ```bash
   pip install scikit-learn nltk gensim
3. Jalankan seluruh sel kode (Run All).
4. Masukkan kueri (contoh: "space mission" atau "computer graphics") pada kolom input untuk melihat peringkat dokumen yang paling relevan.

💡 Hasil Analisis & Kesimpulan
Berdasarkan hasil pengujian pada sistem ini, ditemukan bahwa:

TF-IDF memberikan hasil yang jauh lebih akurat karena mampu memberikan penalti pada kata-kata umum (common words) dan memberikan nilai lebih tinggi pada kata kunci unik yang mencerminkan topik dokumen secara spesifik.

BoW cenderung menghasilkan skor kemiripan yang tinggi pada dokumen yang hanya mengandung banyak kata sambung yang sama dengan kueri, sehingga kurang efektif untuk sistem pencarian dokumen yang presisi.

© 2026 Anak Agung Anantavirya Sadhaka
