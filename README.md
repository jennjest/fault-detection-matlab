# Fault Detection for Electric Motors Using Vibration Analysis

Proyek ini berfokus pada pengembangan simulasi dan analisis untuk mendeteksi kerusakan pada motor listrik menggunakan **vibration analysis** dengan bantuan **MATLAB dan Simulink**.

Melalui simulasi kondisi motor normal dan motor dengan gangguan, proyek ini bertujuan untuk mengamati karakteristik sinyal getaran, mengekstraksi fitur pada domain frekuensi menggunakan **Fast Fourier Transform (FFT)**, serta mengembangkan metode deteksi berbasis ambang batas (*threshold-based detection*).

Proyek ini dilaksanakan sebagai bagian dari program **Konversi Magang Fakultas**.

## Project Overview

| Information | Description |
|---|---|
| Project Title | Fault Detection for Electric Motors Using Vibration Analysis |
| Domain | Electrical Motor Fault Detection |
| Method | Vibration Analysis and Frequency Domain Analysis |
| Tools | MATLAB & Simulink |
| Project Duration | 26 December 2026 – 7 March 2027 |
| Duration | 10 Weeks |
| Team Size | 3 Members |

### Objectives

1. Memodelkan sistem motor listrik menggunakan MATLAB dan Simulink.
2. Menjalankan simulasi motor dalam kondisi normal (*healthy condition*) sebagai baseline.
3. Mensimulasikan beberapa jenis gangguan motor listrik melalui metode *fault injection*.
4. Merekam dan mengolah sinyal getaran serta arus motor dari hasil simulasi.
5. Menganalisis karakteristik sinyal pada domain frekuensi menggunakan FFT.
6. Mengidentifikasi puncak frekuensi karakteristik kerusakan (*fault frequency peaks*).
7. Mengembangkan kriteria deteksi kerusakan berdasarkan ambang batas (*thresholding*).

## Team Members & Responsibilities

Proyek ini dikerjakan oleh tiga anggota dengan pembagian tanggung jawab berdasarkan tiga fokus utama, yaitu pemodelan sistem, pengolahan sinyal, dan integrasi serta dokumentasi proyek.

| Member | Role | Main Responsibility |
|---|---|---|
| **Kael** | Simulink & Plant Modeling Specialist | Motor modeling, simulation, and fault injection |
| **Farel** | Signal Processing & MATLAB Scripter | Signal processing, FFT analysis, and threshold-based detection |
| **Jenni** | System Integrator, GitHub & Report Lead | Repository management, data integration, and final documentation |

### 1. Kael: Simulink & Plant Modeling Specialist

**Main Focus:** Pemodelan sistem fisik motor listrik dan eksekusi skenario simulasi menggunakan Simulink.

Responsibilities:
- Mempelajari blok diagram model motor listrik yang tersedia pada repositori resmi MathWorks.
- Menyiapkan dan menjalankan simulasi motor dalam kondisi normal (*baseline condition*).
- Mengaktifkan dan memodifikasi parameter gangguan melalui metode *fault injection*.
- Mensimulasikan gangguan berupa:
  - Bearing fault
  - Rotor eccentricity
- Memvariasikan tingkat keparahan kerusakan dan kondisi operasi motor.
- Mengekspor sinyal keluaran berupa getaran dan arus ke MATLAB Workspace.
- Menjalankan simulasi tambahan dengan variasi beban dan kecepatan putar motor.
- Memastikan model Simulink dapat dijalankan kembali tanpa galat.

### 2. Farel: Signal Processing & MATLAB Scripter

**Main Focus:** Pengolahan data sinyal mentah dan analisis matematika menggunakan skrip MATLAB (`.m`).

Responsibilities:
- Mempelajari skrip pemrosesan sinyal yang tersedia pada repositori proyek.
- Memahami struktur variabel dan format data masukan dari hasil simulasi.
- Melakukan analisis sinyal pada domain waktu (*time domain analysis*).
- Mengimplementasikan Fast Fourier Transform (FFT) untuk mengubah sinyal dari domain waktu ke domain frekuensi.
- Mengidentifikasi puncak frekuensi yang menjadi karakteristik masing-masing jenis kerusakan.
- Membandingkan karakteristik sinyal antara kondisi normal dan kondisi rusak.
- Merancang logika deteksi berdasarkan ambang batas (*thresholding*).
- Menghasilkan grafik visual untuk membandingkan hasil analisis setiap kondisi motor.

### 3. Jenni: System Integrator, GitHub & Report Lead

**Main Focus:** Manajemen repositori, integrasi data antaranggota, dan penyusunan laporan akhir konversi magang.

Responsibilities:
- Membuat dan mengelola repositori GitHub kelompok.
- Menyusun struktur direktori dan mengelola riwayat pembaruan proyek.
- Menetapkan standar format pertukaran data antara Kael dan Farel.
- Mengarsipkan dataset hasil simulasi ke dalam repositori.
- Mencatat hasil eksperimen dan perubahan parameter simulasi.
- Mendokumentasikan arsitektur sistem motor listrik.
- Menyusun laporan konversi magang secara bertahap.
- Mengintegrasikan hasil grafik dan analisis teknis ke dalam laporan.
- Mengelola dokumentasi `README.md` dan memastikan repositori siap digunakan untuk proses evaluasi akhir.

## Project Timeline

Pelaksanaan proyek dibagi menjadi lima fase selama sepuluh minggu.

| Period | Phase | Main Activities |
|---|---|---|
| 26 Dec 2026 – 8 Jan 2027 | Phase 1: Onboarding & Environment Setup | Menyelesaikan MATLAB Onramp dan Simulink Onramp, menyiapkan lingkungan kerja, memahami repositori MathWorks, serta membuat repositori GitHub. |
| 9 Jan – 22 Jan 2027 | Phase 2: Model Exploration & Baseline | Menjalankan simulasi motor normal, mengamati parameter RPM, arus stator, dan sinyal getaran, serta menyimpan data baseline. |
| 23 Jan – 5 Feb 2027 | Phase 3: Fault Injection | Mengaktifkan simulasi bearing fault dan rotor eccentricity, memvariasikan tingkat kerusakan, dan merekam dataset kondisi rusak. |
| 6 Feb – 19 Feb 2027 | Phase 4: FFT Analysis & Detection | Melakukan analisis FFT, mengidentifikasi puncak frekuensi kerusakan, menyusun kriteria threshold, dan menguji konsistensi respons getaran. |
| 20 Feb – 7 Mar 2027 | Phase 5: Final Validation & Reporting | Memvalidasi model dan skrip, menyelesaikan dokumentasi, menyusun kesimpulan, serta melakukan finalisasi laporan konversi magang. |

### Phase 1: Onboarding & Environment Setup

**26 December 2026 – 8 January 2027**

- Seluruh anggota menyelesaikan MATLAB Onramp dan Simulink Onramp.
- **Kael:** Mengunduh repositori resmi MathWorks, memasang toolbox pendukung yang diperlukan, dan memastikan model Simulink dapat dijalankan.
- **Farel:** Mengidentifikasi skrip MATLAB (`.m`) dan memahami struktur variabel masukan.
- **Jenni:** Membuat repositori GitHub privat dan menyiapkan struktur direktori proyek.

### Phase 2: Model Exploration & Baseline

**9 January – 22 January 2027**

- **Kael:** Menjalankan simulasi motor dalam kondisi normal dan merekam parameter RPM, arus stator, serta sinyal getaran.
- **Farel:** Membaca sinyal baseline pada domain waktu dan memverifikasi kestabilan amplitudo sinyal motor normal.
- **Jenni:** Mendokumentasikan arsitektur sistem dan mulai menyusun Bab 1 (Pendahuluan) serta Bab 2 (Tinjauan Pustaka).

### Phase 3: Fault Injection

**23 January – 5 February 2027**

- **Kael:** Mengaktifkan blok injeksi kerusakan pada Simulink untuk bearing fault dan rotor eccentricity, memvariasikan tingkat keparahan, serta merekam dataset.
- **Farel:** Membandingkan sinyal domain waktu antara kondisi normal dan rusak untuk mengidentifikasi anomali amplitudo.
- **Jenni:** Mengarsipkan dataset hasil simulasi dan mencatat parameter eksperimen untuk Bab 3 (Metodologi).

### Phase 4: FFT Analysis & Detection

**6 February – 19 February 2027**

- **Kael:** Menjalankan simulasi tambahan dengan variasi beban atau kecepatan putar motor untuk menguji konsistensi respons getaran.
- **Farel:** Menerapkan FFT pada dataset, memetakan puncak frekuensi karakteristik kerusakan, dan menyusun kriteria threshold untuk deteksi dini.
- **Jenni:** Mengintegrasikan grafik spektrum frekuensi dan menyusun pembahasan teknis untuk Bab 4 (Hasil dan Pembahasan).

### Phase 5: Final Validation & Reporting

**20 February – 7 March 2027**

- **Kael & Farel:** Memvalidasi seluruh model Simulink dan skrip MATLAB agar dapat dijalankan kembali dan direproduksi.
- **Jenni:** Menyelesaikan dokumentasi GitHub, melengkapi Bab 5 (Kesimpulan dan Saran), serta menyunting laporan akhir.
- **Seluruh Tim:** Melakukan pengecekan akhir dan menyerahkan laporan serta repositori proyek paling lambat 7 March 2027.

## Repository Structure

Struktur direktori repositori direncanakan sebagai berikut:

```text
fault-detection-electric-motors/
│
├── models/
│   └── motor_simulation.slx
│
├── scripts/
│   └── signal_processing.m
│
├── data/
│   ├── healthy/
│   └── faulty/
│
├── docs/
│   ├── experiments/
│   ├── figures/
│   └── report/
│
└── README.md
```

| Directory | Description |
|---|---|
| `models/` | Model simulasi motor listrik menggunakan Simulink (`.slx`). |
| `scripts/` | Skrip MATLAB untuk pengolahan dan analisis sinyal. |
| `data/` | Dataset hasil simulasi kondisi normal dan kondisi rusak. |
| `docs/` | Dokumentasi eksperimen, grafik hasil analisis, dan laporan proyek. |

## Data Management

Seluruh data hasil simulasi harus disimpan dalam format terstruktur agar dapat digunakan secara konsisten oleh anggota yang bertanggung jawab atas pemrosesan sinyal.

Format data yang digunakan:

- `.mat`
- `.csv`

Contoh penamaan file:

```text
data_sehat_1500rpm.mat
data_bearing_fault_1500rpm.mat
data_eccentricity_1500rpm.mat
```

Penamaan file harus mencerminkan kondisi motor dan parameter simulasi agar memudahkan identifikasi serta perbandingan dataset.

## Team Coordination & Development Guidelines

Untuk menjaga konsistensi pekerjaan dan menghindari konflik antaranggota, beberapa aturan koordinasi diterapkan selama pengerjaan proyek.

### 1. Simulink Model Editing

Perubahan langsung pada file Simulink (`.slx`) hanya dilakukan oleh **Kael**. Aturan ini diterapkan untuk menghindari konflik versi dan kerusakan struktur file akibat penggabungan perubahan secara otomatis.

### 2. Standardized Data Exchange

Kael bertanggung jawab menyediakan data hasil simulasi dalam format `.mat` atau `.csv`. Data tersebut kemudian digunakan oleh Farel untuk proses pengolahan dan analisis sinyal.

Format serta penamaan dataset harus konsisten untuk setiap eksperimen.

### 3. Experiment Documentation

Setiap eksperimen harus memiliki catatan mengenai:
- Kondisi motor yang disimulasikan.
- Jenis gangguan yang diberikan.
- Parameter kecepatan putar dan beban motor.
- Tingkat keparahan gangguan, jika diterapkan.
- Dataset hasil simulasi.
- Hasil pengamatan dan analisis.

### 4. Weekly Synchronization

Tim melakukan evaluasi singkat setiap akhir pekan, yaitu Jumat atau Sabtu, selama 15–30 menit.

Evaluasi bertujuan untuk:
- Memastikan target mingguan telah tercapai.
- Memeriksa hasil pekerjaan setiap anggota.
- Memastikan dataset dan dokumentasi telah diunggah ke GitHub.
- Mengidentifikasi kendala yang menghambat pekerjaan.
- Menyelaraskan kebutuhan data antaranggota untuk fase berikutnya.

## Expected Deliverables

Pada akhir periode proyek, tim menargetkan luaran berikut:

1. Model simulasi motor listrik menggunakan MATLAB dan Simulink.
2. Skenario simulasi kondisi normal dan kondisi rusak, meliputi bearing fault dan rotor eccentricity.
3. Dataset sinyal getaran dan arus dari berbagai kondisi simulasi.
4. Skrip MATLAB untuk pengolahan sinyal dan analisis FFT.
5. Grafik perbandingan sinyal pada domain waktu dan domain frekuensi.
6. Kriteria threshold untuk mendukung proses deteksi kerusakan.
7. Dokumentasi eksperimen dan repositori GitHub yang dapat direproduksi.
8. Laporan akhir konversi magang.

## Project Completion

**Final Deadline: 7 March 2027**

Seluruh model, skrip, dataset, dokumentasi, dan laporan akhir harus telah diperiksa serta disiapkan untuk proses penyerahan kepada dosen pembimbing atau penguji.

---

*This repository serves as the central workspace for the Fault Detection for Electric Motors Using Vibration Analysis project.*
