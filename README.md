# Aktivitas Naive Bayes — Apakah Cocok Bermain Tenis Hari Ini?

Boilerplate aktivitas kelompok untuk mata kuliah **Machine Learning (DSB07)** — topik **Naive Bayes**.
Cocok untuk satu sesi kelas (~45 menit) bagi mahasiswa S-1 Teknik Informatika.

> Materi prasyarat: slide *PB11MAT_DSB07-P10_Naive Bayes* (Pengertian, Tahapan Klasifikasi, Analisa Data).

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

Repo ini dirancang sebagai **template GitHub Classroom**. Alur penggunaan:

1. Pastikan repo ini publik di organisasi Anda (mis. `UBM-ML/naive-bayes`) dan ditandai sebagai **Template repository** (Settings → Template repository).
2. Buat *assignment* di GitHub Classroom yang menggunakan repo ini sebagai template, dengan tipe **Group assignment**.
3. Sebelum membagikan invite, **pindahkan `notebooks/solusi.ipynb` ke branch privat** atau hapus dari template — agar kunci jawaban tidak ikut ter-clone ke repo tiap tim.
4. Bagikan invite link Classroom ke mahasiswa. Setiap tim akan otomatis mendapat repo sendiri (mis. `UBM-ML-Classroom/naive-bayes-tim-andi`).
5. Penilaian: lihat commit terakhir di branch `main` repo masing-masing tim sebelum deadline, gunakan rubrik di bawah.

> **Catatan data:** URL CSV di dalam notebook sudah di-pin ke `UBM-ML/naive-bayes` (repo template publik), sehingga semua tim memuat dataset yang sama tanpa perlu mengedit URL. Jangan rename atau privat-kan repo template selama semester berjalan.

## Untuk Tim Mahasiswa

Setelah klik invite GitHub Classroom dari dosen, ikuti alur berikut:

1. **Repo tim Anda otomatis dibuat** di organisasi kelas. Buka repo tersebut di GitHub.
2. **Buka notebook di Colab.** Ada dua cara:
   - Klik file `notebooks/template.ipynb` di GitHub → di atas preview notebook akan muncul tombol **"Open in Colab"**, **atau**
   - Buka [colab.research.google.com](https://colab.research.google.com) → menu *File → Open notebook → tab GitHub* → cari repo tim Anda → pilih `notebooks/template.ipynb`.
3. **Kerjakan TODO** di notebook. Tulis nama anggota tim di sel paling atas terlebih dahulu.
4. **Simpan kembali ke repo tim Anda.** Di Colab: *File → Save a copy in GitHub* → pilih repo tim → branch `main` → commit message singkat (mis. *"selesai tahap 2"*).
5. **Submission:** commit final sebelum deadline yang ditentukan dosen. Yang dinilai adalah commit terakhir di branch `main`.

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
    ├── template.ipynb         # Versi mahasiswa (berisi TODO)
    └── solusi.ipynb           # Kunci jawaban (untuk dosen)
```

## Lisensi
Lihat [LICENSE](LICENSE).
