---
title: "Protokol SLR-RQ1"
subtitle: "Konseptualisasi, pengembangan, dan pengukuran Computational Thinking dalam pembelajaran fisika dan Earth Science (2016–2026)"
lang: id
---

# 1. Pertanyaan Penelitian

**SLR-RQ1.** Bagaimana *Computational Thinking* (CT) dikonseptualisasikan, dikembangkan, dan diukur dalam pembelajaran fisika dan Earth Science selama 10 tahun terakhir?

Supaya bisa dikodekan, RQ1 dipecah menjadi lima subpertanyaan:

| Sub-RQ | Pertanyaan | Data yang diekstrak | Fungsi untuk disertasi |
|---|---|---|---|
| **1a** | Bagaimana karakteristik publikasinya? | tahun, negara, jurnal, jenjang, **subjek (calon guru?)**, desain penelitian, ukuran sampel | Bukti "calon guru fisika jarang diteliti" |
| **1b** | Bagaimana CT dikonseptualisasikan? | definisi yang dikutip, **kerangka CT** (Wing, Brennan & Resnick, Weintrop dkk., Shute dkk., dll.), komponen CT | Dasar memilih kerangka CT |
| **1c** | Bagaimana CT dikembangkan? | model/pendekatan pembelajaran, **plugged/unplugged**, alat (Scratch, Python, simulasi, Arduino/IoT), **ada CM atau tidak**, materi fisika/kebumian, **masalah autentik atau soal terstruktur** | Bukti gap pertama: "CT lebih banyak lewat pemrograman, belum lewat masalah autentik" |
| **1d** | Bagaimana CT diukur? | jenis instrumen (tes, skala, rubrik kinerja, analisis artefak/kode), nama instrumen, komponen yang diukur, validitas dan reliabilitas | Dasar menyusun instrumen CT disertasi |
| **1e** | Apa hasil dan keterbatasannya? | temuan utama, keterbatasan, rekomendasi penelitian lanjutan | Celah penelitian dan arah lanjutan |

# 2. Kerangka PICOC

| Unsur | Definisi |
|---|---|
| **Population** | Peserta didik semua jenjang (sekolah menengah, mahasiswa, **calon guru**). Subjek calon guru dikodekan terpisah. |
| **Intervention / Phenomenon** | Pengembangan atau pengukuran CT |
| **Comparison** | Tidak diwajibkan |
| **Outcome** | CT (sebagai hasil, kerangka, atau praktik yang dianalisis) |
| **Context** | Pembelajaran **fisika** atau **Earth Science** (geofisika, meteorologi, hidrologi, sistem Bumi) |

# 3. Sumber Data

| Basis data | Peran | Akses |
|---|---|---|
| **Scopus** | **Utama** | Melalui langganan perpustakaan kampus (cek Perpustakaan Unila atau universitas tempat studi S3). Masuk dari jaringan kampus atau VPN/akun institusi. |
| **Web of Science** | *Cross-check* (bila tersedia) | Langganan institusi |
| **ERIC** (eric.ed.gov) | Pelengkap khusus pendidikan | **Gratis** |
| **Google Scholar** via aplikasi *Publish or Perish* (Harzing) | Pelengkap dan *grey literature* | **Gratis** |
| **Dimensions** (app.dimensions.ai) atau **Lens.org** | Alternatif gratis bila Scopus tidak tersedia | **Gratis** (fitur ekspor terbatas) |
| **Garuda / SINTA** | Opsional: studi Indonesia (Sinta 1–2) | **Gratis** |

**Teks lengkap (PDF):** langganan kampus, *open access*, ekstensi Unpaywall, repositori penulis/ResearchGate, atau permintaan langsung ke penulis melalui email. Hindari sumber ilegal karena metode SLR harus dapat dipertanggungjawabkan.

# 4. String Pencarian

## 4.1 Scopus (utama)

```
TITLE-ABS-KEY ( "computational thinking" )
AND TITLE-ABS-KEY ( physics OR "earth science*" OR geoscience* OR geophysic*
                    OR "earth system*" OR meteorolog* OR hydrolog* OR geolog* )
AND TITLE-ABS-KEY ( educat* OR learn* OR teach* OR student* OR course*
                    OR classroom* OR curricul* )
AND PUBYEAR > 2015 AND PUBYEAR < 2027
AND ( LIMIT-TO ( DOCTYPE , "ar" ) OR LIMIT-TO ( DOCTYPE , "cp" ) OR LIMIT-TO ( DOCTYPE , "re" ) )
AND ( LIMIT-TO ( LANGUAGE , "English" ) )
```

Catatan:
- *Review* (`re`) tetap diambil untuk ***snowballing***, yaitu menelusuri daftar pustakanya, tetapi tidak dimasukkan ke korpus analisis.
- Bila hasil terlalu sedikit (kurang dari 30), longgarkan dengan menambahkan `OR "computational model*" OR "computational practice*"` pada baris pertama dan catat versinya.
- Bila hasil terlalu banyak (lebih dari 600), batasi dengan `LIMIT-TO ( SUBJAREA , "SOCI" )`.

## 4.2 Web of Science

```
TS=("computational thinking")
AND TS=(physics OR "earth science*" OR geoscience* OR geophysic* OR "earth system*"
        OR meteorolog* OR hydrolog* OR geolog*)
AND TS=(educat* OR learn* OR teach* OR student* OR course* OR classroom* OR curricul*)
Timespan: 2016-2026 · Document types: Article, Proceedings Paper, Review · Language: English
```

## 4.3 ERIC

```
"computational thinking" AND (physics OR "earth science" OR geoscience)
Filter: Peer reviewed only · 2016–2026
```

## 4.4 Publish or Perish (Google Scholar)

- *All of the words*: `computational thinking physics`
- Lakukan juga dengan `computational thinking "earth science"`.
- Tahun 2016–2026; maksimum 500 hasil per pencarian.

> **Wajib dicatat setiap pencarian:** tanggal, basis data, string persis, dan jumlah hasil. Catatan ini masuk ke lembar `Log_Pencarian` di Excel dan ke diagram PRISMA.

# 5. Kriteria Inklusi dan Eksklusi

| Kode | Inklusi | Kode | Eksklusi |
|---|---|---|---|
| I1 | Terbit 2016–2026 | E1 | CT hanya disebut sekilas (tidak dikembangkan, diukur, atau dianalisis) |
| I2 | Artikel jurnal atau prosiding *peer-reviewed* | E2 | Konteks bukan fisika atau Earth Science (mis. murni ilmu komputer, matematika, biologi) |
| I3 | Konteks pembelajaran fisika atau Earth Science | E3 | Bukan konteks pendidikan |
| I4 | CT dikembangkan, diukur, atau dianalisis secara eksplisit | E4 | Review, editorial, atau opini (dipakai hanya untuk *snowballing*) |
| I5 | Studi empiris (kuantitatif, kualitatif, campuran, atau D&D/EDR) | E5 | Teks lengkap tidak dapat diperoleh |
| I6 | Bahasa Inggris (opsional: Indonesia, Sinta 1–2) | E6 | Duplikat |

# 6. Prosedur (PRISMA 2020)

1. **Identifikasi:** jalankan pencarian, ekspor, lalu gabungkan semua hasil.
2. **Hapus duplikat** berdasarkan DOI dan judul.
3. **Screening judul dan abstrak** dengan kriteria I/E. Keputusan: *Include / Exclude (kode) / Ragu*.
4. **Screening teks lengkap** untuk artikel *Include* dan *Ragu*.
5. ***Snowballing*** (backward dan forward) dari artikel inklusi dan review terkait.
6. **Ekstraksi data** ke lembar `Ekstraksi_RQ1`.
7. **Reliabilitas antar-penilai:** penilai kedua (rekan atau promotor) mengkode ulang sekitar 20% artikel; hitung **Cohen's κ** (target ≥ 0,70; Suryadi dkk. melaporkan κ = 0,75).
8. **Sintesis:** statistik deskriptif (1a, 1c, 1d) dan sintesis tematik (1b, 1e).

# 7. Pembagian Peran: Bapak dan Claude

| Langkah | Bapak | Claude |
|---|---|---|
| Protokol, string, templat | Mereview dan menyesuaikan | **Sudah disiapkan (dokumen ini dan Excel)** |
| Pencarian di Scopus/WoS | **Menjalankan** (perlu login institusi) | Tidak bisa login ke Scopus dari sesi ini |
| Ekspor | Ekspor **CSV** dengan semua kolom (*citation information, bibliographical information, abstract & keywords*) + **RIS/BibTeX**; unggah ke chat atau folder `slr/rq1/raw/` | Menggabungkan file dan **menghapus duplikat** |
| Screening judul–abstrak | **Memverifikasi** keputusan | **Screening tahap pertama** dengan alasan per artikel (Include/Exclude-kode/Ragu) |
| PDF teks lengkap | **Mengunduh** dan mengunggah | Membaca PDF dan **mengekstrak data** ke Excel, dengan kutipan halaman sebagai bukti |
| Verifikasi | Mengecek sampel hasil ekstraksi | Menghitung κ bila ada penilai kedua |
| Analisis dan penulisan | Menginterpretasi dan memutuskan | Tabel, grafik, diagram PRISMA, file siap VOSviewer, draf narasi hasil RQ1 |

**Catatan etika metodologi:** penggunaan AI untuk membantu screening dan ekstraksi perlu **diungkapkan di bagian metode**. Keputusan akhir inklusi dan pengkodean tetap dibuat dan diverifikasi oleh peneliti.
