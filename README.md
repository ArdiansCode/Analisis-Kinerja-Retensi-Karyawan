# Analisis Kinerja & Retensi Karyawan (HR & Workforce Analytics)

Proyek portofolio ini berisi analisis data sumber daya manusia (HR) untuk mengevaluasi kinerja karyawan, tingkat kepuasan (*satisfaction level*), durasi lembur (*overtime*), serta risiko 
resign (*resign risk*) di dalam perusahaan.

---

## 📁 Struktur Direktori & File
- **`HR_&_WORKFORCE_ANALYTICS.ipynb`**: Notebook Jupyter yang berisi eksplorasi data, pembersihan data (*data cleaning*), manipulasi data, dan visualisasi analitik workforce.
- **`database.db`**: Basis data SQLite yang menyimpan tabel bersih hasil pemrosesan data karyawan (`hr_employees`).
- **`hr_dataset_extended.csv` & `hr_dataset_extended_1.csv`**: File dataset mentah/ekstensi dalam format CSV yang digunakan sebagai sumber data utama.

---

## 📊 Ringkasan & Temuan Utama (Key Findings)

Berdasarkan analisis terhadap 50 data karyawan dalam basis data:

1. **Distribusi Departemen & Jumlah Karyawan**:
   - Total Karyawan Dianalisis: **50 orang**
   - **Engineering**: 19 karyawan (Departemen terbesar dengan tingkat kepuasan rata-rata **3.58**)
   - **Sales**: 10 karyawan (Menunjukkan tingkat kepuasan terendah rata-rata **1.90**)
   - **Marketing**: 8 karyawan (Kepuasan rata-rata **3.25**)
   - **Finance**: 8 karyawan (Kepuasan rata-rata **3.75**)
   - **HR**: 5 karyawan (Kepuasan tertinggi rata-rata **4.00**)

2. **Analisis Risiko Resign (*Resign Risk*)**:
   - **High Risk**: **13 karyawan** terdeteksi memiliki indikasi atau risiko tinggi untuk keluar dari perusahaan (biasanya berkorelasi dengan tingkat kepuasan yang rendah dan jam lembur yang tinggi).
   - **Safe**: **37 karyawan** berada dalam kategori aman dan stabil.

3. **Kompensasi & Kinerja**:
   - Rata-rata Gaji Bulanan (*Monthly Salary*): **Rp 11.266.000**
   - Gaji tertinggi dipegang oleh peran **Data Scientist** (rata-rata ~Rp 17.500.000) dan **DevOps Engineer** (~Rp 15.875.000).
   - Jam lembur (*Overtime Hours*) tertinggi terdapat pada peran **Data Scientist** (~29.8 jam) dan **Account Executive** (~26.3 jam).

---

## 🛠️ Teknologi & Tools yang Digunakan
- **Python**: Pemrosesan dan analisis data (`pandas`, `numpy`)
- **Visualisasi**: `matplotlib`, `seaborn`
- **Database**: SQLite (`database.db`)
- **Environment**: Jupyter Notebook

---

## 🚀 Cara Menjalankan Proyek
1. Pastikan lingkungan Python terinstal beserta pustaka yang dibutuhkan (`pandas`, `numpy`, `matplotlib`, `seaborn`).
2. Buka file notebook menggunakan Jupyter:
   ```bash
   jupyter notebook "HR_&_WORKFORCE_ANALYTICS.ipynb"
   ```
3. Atau lakukan kueri langsung pada file `database.db` menggunakan SQLite viewer/CLI.
