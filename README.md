# 📌 Title Project
**Perkembangan Roblox Berdasarkan Analisis Sentimen dan Tren Review Google Play Menggunakan IBM Granite AI**

Analisis ulasan & tren untuk memahami persepsi pengguna serta menyusun proyeksi pertumbuhan ekosistem Roblox.

---

# 🧭 Project Overview
Proyek ini mengeksplorasi data ulasan terkait Roblox untuk:
- melakukan eksplorasi data (EDA) singkat,
- mengekstraksi sentimen dan topik yang sering muncul,
- merumuskan *insight* yang relevan untuk produk/komunitas,
- serta menyusun gambaran awal prediksi perkembangan Roblox berbasis indikator dari ulasan & metrik pendukung.

Repositori ini berisi *notebook* Jupyter untuk eksperimen dan sebuah berkas dataset mentah (Excel).

> Catatan: Silakan jalankan notebook untuk mereproduksi grafik, tabel, dan ringkasan metrik.

---

# 🗂️ Raw Dataset Link
- 📥 **Dataset (Excel):** [`ROBLOX_REVIEWS.xls`](https://github.com/MitaAdhani/Prediksi-Perkembangan-Roblox-/blob/master/ROBLOX_REVIEWS.xls)
- 🔗 **Raw (direct download):** https://www.kaggle.com/datasets/bwandowando/322k-roblox-app-google-store-reviews?resource=download

> Perbarui tautan jika struktur folder/branch berubah.

---

# 🔎 Insight & Findings
Ringkasan berikut adalah draft *template* hasil. Perbarui dengan angka/temuan dari notebook kamu.

- ⭐ **Sentimen dominan:** _isi: proporsi positif/negatif/netral & contoh kutipan kunci_.
- 🧵 **Topik utama:** _isi: tema yang sering muncul—mis. kreativitas di Roblox Studio, komunitas, performa/bug, keamanan anak_.
- 📈 **Arah tren:** _isi: naik/turun berdasarkan volume ulasan & rerata rating per periode_.
- 🧩 **Implikasi produk:** _isi: peluang peningkatan—mis. moderasi, edukasi orang tua, stabilitas & UX_.

> Tips:
> - Tambahkan grafik distribusi rating & *word cloud*.
> - Buat tabel top keluhan & pujian.
        - Jika ada model sentimen, tampilkan metrik (akurasi/F1) dan contoh salah-klasifikasi.

---

# 🤖 AI Support Explanation
Bagaimana AI digunakan dalam proyek ini:

1. **Pra-proses NLP** 🧼  
   *Cleaning* teks (lowercasing, hapus tanda baca, stopword ID/EN), tokenization, dan stemming/lemmatization.

2. **Analisis Sentimen** 💬  
   - Opsi cepat: leksikon/rule-based.  
   - Opsi klasik: Logistic Regression/SVM + TF-IDF.  
   - Opsi lanjut: *Transformer* (IndoBERT/Multilingual) untuk akurasi lebih tinggi.

3. **Ekstraksi Topik** 🧠  
   LDA/NMF atau *keyphrase extraction* untuk menemukan tema yang berulang.

4. **Prediksi Perkembangan** 📊  
   Memakai indikator agregat (volume ulasan, rerata rating, rasio sentimen, sinyal topik) lalu regresi/time-series sederhana untuk proyeksi jangka pendek.

5. **Validasi & Interpretasi** 🔍  
   Tampilkan *confusion matrix*/classification report (jika ada model) dan contoh ulasan yang salah klasifikasi untuk insight perbaikan.

---

> 🙌 **Saran lanjut**: Tambahkan bagian *How to Run* (requirements + cara eksekusi notebook) bila repo siap dipublikasikan ke audiens yang lebih luas.
