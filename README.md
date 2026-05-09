# Aktivitas Naive Bayes — Apakah Cocok Bermain Tenis Hari Ini?

Aktivitas kelompok untuk mata kuliah **Machine Learning** — topik **Naive Bayes**.
Cocok untuk satu sesi kelas (~45 menit) bagi mahasiswa S-1 Teknik Informatika.

## Tujuan Pembelajaran (Sub-CPMK C3, A3)
Setelah aktivitas ini, mahasiswa mampu:
1. **Menghitung** probabilitas prior, kondisional, dan posterior secara manual untuk satu kasus klasifikasi Naive Bayes.
2. **Mengimplementasikan** Naive Bayes menggunakan `scikit-learn` di Google Colab.
3. **Membandingkan** hasil manual dengan hasil sklearn dan menjelaskan penyebab perbedaannya (Laplace smoothing).

## Format Aktivitas
- **Durasi:** 45 menit di kelas
- **Kelompok:** 3–4 mahasiswa
- **Platform:** Google Colab
- **Dataset:** `play_tennis.csv` (14 baris klasik — Quinlan/Mitchell)

| Tahap | Durasi | Kegiatan |
|-------|--------|----------|
| 1. Memahami data | 5 menit | Load CSV, lihat distribusi label |
| 2. Hitung manual | 15 menit | Prior, kondisional, posterior untuk 1 kasus uji |
| 3. Implementasi sklearn | 15 menit | `CategoricalNB`, prediksi kasus uji yang sama |
| 4. Diskusi kelompok | 7 menit | Bandingkan hasil, jawab 4 pertanyaan diskusi |
| 5. Refleksi | 3 menit | 3 kalimat refleksi pribadi |

## Cara Menggunakan (untuk Dosen)
1. **Fork / clone** repo ini ke GitHub Anda.
2. Edit placeholder `USERNAME` di [notebooks/template.ipynb](notebooks/template.ipynb) dan tombol *Open in Colab* di bawah agar mengarah ke repo Anda.
3. Bagikan link *Open in Colab* template ke mahasiswa. Minta tiap kelompok membuat **copy** ke Drive masing-masing.
4. Simpan [notebooks/solusi.ipynb](notebooks/solusi.ipynb) untuk Anda sendiri (atau pindahkan ke branch privat sebelum repo di-publish).

### Tombol Open in Colab (ganti `USERNAME`)
```markdown
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/USERNAME/naive-bayes/blob/main/notebooks/template.ipynb)
```

## Rubrik Penilaian Kelompok (100 poin)

| Aspek | Bobot | Indikator |
|-------|-------|-----------|
| Perhitungan manual | 30 | Prior, kondisional, dan posterior dihitung benar; prediksi kelas tepat |
| Implementasi sklearn | 30 | Encoding fitur benar, model terlatih, prediksi & probabilitas ditampilkan |
| Analisis perbandingan | 20 | Mampu menjelaskan perbedaan numerik manual vs sklearn (Laplace smoothing) |
| Diskusi & refleksi | 20 | 4 pertanyaan diskusi terjawab dengan beralasan; refleksi jujur |

## Struktur Repo
```
.
├── README.md                  # Anda di sini
├── data/
│   └── play_tennis.csv        # Dataset 14 baris
└── notebooks/
    └── template.ipynb         # berisi TODO
```

## Lisensi
Lihat [LICENSE](LICENSE).
