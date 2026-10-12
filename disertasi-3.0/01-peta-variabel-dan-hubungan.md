# Peta Variabel dan Hubungan Antarvariabel — Disertasi 3.0

Dokumen kerja ini merangkum hasil penelusuran literatur awal untuk setiap variabel dalam rancangan Disertasi 3.0, sesuai keputusan terakhir pada dokumen *Rancang Ulang Disertasi* (hlm. 89–118). Isinya menjadi bahan baku penyusunan Latar Belakang (lihat `02-draf-latar-belakang.md`).

> **Status verifikasi.** Setiap rujukan diberi tanda:
> - ✅ **terverifikasi**: keberadaan artikel, penulis, dan jurnal sudah dicek melalui penelusuran web;
> - ⚠️ **perlu dicek**: artikel ditemukan, tetapi nama penulis atau detail bibliografisnya belum bisa dipastikan dari lingkungan kerja ini (situs penerbit tidak dapat diakses langsung). Cek di Scopus atau melalui DOI sebelum dikutip;
> - 📄 **dokumen Bapak**: bersumber dari file yang Bapak miliki (disertasi Amrizaldi, artikel Hendratmoko, Suryadi, Fitriah, Novitra, dan Kurikulum Unila 2025).

---

## 1. Struktur Konseptual yang Disepakati

| Posisi | Konstruk | Kedudukan dalam desain |
|---|---|---|
| Variabel bebas (intervensi terpadu) | **Problem-Based Learning (PBL)** | *Pedagogical backbone*: mengorganisasi belajar melalui masalah autentik yang *ill-structured* |
| | **Integrated STEM** | Kerangka integrasi interdisipliner; STEM muncul karena masalah *menuntut* integrasi disiplin, bukan S-T-E-M di setiap sintaks |
| | **Computational Modeling (CM)** | Praktik ilmiah-komputasional: *define system → variables → relationships → construct → simulate → compare with data → validate → revise* |
| | **Scientific Argumentation Scaffolding (SAS)** | *Epistemic scaffold*: claim–evidence–reasoning–counterclaim/rebuttal untuk menilai output model dan solusi rekayasa |
| Variabel terikat utama | **Computational Thinking (CT)** | Kemampuan yang dikembangkan dan diukur |
| Domain | **Fisika Bumi** | Mata kuliah pilihan semester V–VI (Kurikulum Pendidikan Fisika Unila 2025) |
| Konteks | **Authentic Earth-system problem** | Kandidat utama: banjir/hidrometeorologi dan *environmental monitoring* (belum final) |
| Subjek | Mahasiswa calon guru fisika | |
| Lingkungan teknologi (opsional) | IoT/sensor, Python/*functional programming* | Alat akuisisi data dan platform CM, **bukan** sumber kebaruan |

**Catatan penting.** Keempat komponen intervensi diperlakukan sebagai **satu variabel bebas berupa desain pembelajaran terintegrasi**, bukan empat variabel bebas terpisah. Dengan begitu tidak diperlukan desain faktorial.

**Siklus mekanisme yang diajukan:**

```
Authentic Earth Problem → PBL → Integrated STEM + Engineering Design → Computational Model Construction
→ Real + Model-Generated Evidence → Scientific Argumentation Scaffolding (C–E–R–Rebuttal)
→ Critique → Model/Design Revision ⟲ → Computational Thinking
```

---

## 2. Profil Setiap Variabel

### 2.1 Computational Thinking (CT) — variabel terikat

**Definisi kunci**
- Wing (2006): CT adalah keterampilan berpikir fundamental bagi semua orang, bukan hanya ilmuwan komputer. ✅
- Grover & Pea (2013): CT melibatkan abstraksi, dekomposisi, berpikir algoritmik, dan generalisasi pola. ✅
- Shute, Sun, & Asbell-Clarke (2017): CT adalah fondasi konseptual untuk memecahkan masalah secara efektif dan efisien, dengan solusi yang dapat digunakan ulang dalam konteks lain. ✅
- **Weintrop et al. (2016)**: taksonomi CT untuk kelas matematika dan sains dengan empat kategori, yaitu *data practices*, *modeling & simulation practices*, *computational problem-solving practices*, dan *systems thinking practices*. Ini **kandidat kuat kerangka CT** karena praktik pemodelan dan simulasi menjadi bagian eksplisit dari CT, sehingga cocok dengan konteks CM. ✅

**Temuan empiris yang relevan**
- Review CT dalam pendidikan guru (*International Journal of Educational Research*, 2025) menelaah 43 artikel (2014–2024) dengan PRISMA. Penelitian terkonsentrasi pada calon guru dan bidang STEM, dengan aktivitas *plugged* dan *visual programming* yang dominan. ⚠️ (judul: *Integrating computational thinking into teacher education: A systematic literature review*; penulis perlu dicek)
- Dong et al. (2023) mereview pengembangan CT calon guru, *International Journal of Technology and Design Education*, DOI 10.1007/s10798-023-09811-3. ✅ (temuan rinci belum dibaca)
- Ogegbo & Ramnarain (2022) mereview 23 studi integrasi CT di kelas sains, *Studies in Science Education*. ✅
- Di Indonesia, SLR CT dalam pembelajaran fisika (JPPIPA, 2025) menemukan 20 dari 170 artikel relevan. Subjek dominan siswa SMA, materi dominan kinematika serta usaha–energi, dan media dominan Scratch. ✅ Review berbasis Scopus 2015–2025 (16 artikel, prosiding UNINDRA) mencatat pergeseran dari simulasi umum ke pemrograman Python, dengan tantangan utama pada kompetensi guru. ✅
- Amrizaldi (2025), disertasi UM: STEM-CT pada materi suhu dan kalor; studi pendahuluan pada 53 siswa menunjukkan *abstraction* (2,83) dan *algorithm* (2,37) sebagai aspek terlemah. 📄

**Implikasi untuk latar belakang:** CT di pendidikan fisika masih banyak dibangun melalui pemrograman, media visual, atau simulasi siap pakai, dan jarang melalui penyelesaian masalah ilmiah yang autentik. Calon guru fisika juga belum banyak menjadi subjek penelitian. Inilah **gap pertama**.

### 2.2 Problem-Based Learning (PBL) — komponen intervensi 1

- Hmelo-Silver (2004): PBL berpusat pada masalah kompleks yang tidak memiliki satu jawaban benar. Mahasiswa belajar dalam kelompok kolaboratif untuk mengidentifikasi apa yang perlu dipelajari, dan dosen berperan sebagai fasilitator. ✅
- Savery (2006): masalah PBL harus *ill-structured*. Mahasiswa bertanggung jawab atas pembelajarannya sendiri, dan pembelajaran diakhiri dengan refleksi. ✅
- **Pembeda PBL dan PjBL:** pada PBL, penggerak belajar adalah *masalah*. Produk atau prototipe muncul sebagai *konsekuensi* penyelesaian masalah, bukan tujuan yang ditetapkan sejak awal (hlm. 69–70 dokumen rancangan).
- Kurikulum Pendidikan Fisika Unila 2025 secara eksplisit memasukkan PBL dan PjBL sebagai pendekatan *student-centered*. 📄

### 2.3 Integrated STEM — komponen intervensi 2

- Kelley & Knowles (2016): kerangka konseptual integrated STEM melalui *situated learning*, dengan *engineering design* sebagai perekat antardisiplin. ✅
- **Roehrig, Dare, Ellis, & Ring-Whalen (2021)**, *Disciplinary and Interdisciplinary Science Education Research*, 3: tujuh karakteristik integrated STEM, dua di antaranya **digerakkan masalah autentik** dan **sentralitas engineering design**. ✅
- Suryadi et al. (STEM-TPD): integrasi STEM melibatkan lebih dari satu disiplin dan dapat diarahkan melalui *problem-based*, *inquiry-based*, atau *design-based learning*. 📄
- Arahan promotor: "masalah STEM biasanya tidak dapat diselesaikan dengan satu bidang."

### 2.4 Computational Modeling (CM) — komponen intervensi 3

- Review sistematis CM dalam pendidikan sains (*Interactive Learning Environments*, 2024; DOI 10.1080/10494820.2024.2372832) memakai Web of Science dan Scopus serta memperoleh **70 karya** terkait CM. Review ini menegaskan bahwa review CT di kelas sains berbeda definisi dari CM sehingga sering melewatkan studi CM yang relevan. Artinya, **CM berkaitan dengan CT tetapi tidak identik**. ⚠️ (judul: *Design and application of computational modeling in science education research: a systematic review*; penulis perlu dicek)
- Langbeheim & Bielik (2025), *Studies in Science Education*: review 53 studi (1998–2025) tentang siswa membangun model komputer. Mayoritas berada di konteks fisika dan biologi, dan CT menjadi salah satu outcome. ✅
- Sengupta, Kinnebrew, Basu, Biswas, & Clark (2013): kerangka teoretis integrasi CT dengan sains melalui komputasi berbasis agen. ✅
- Hutchins et al. (2020), *Journal of Science Education and Technology*, 29: C2STEM, sistem untuk pembelajaran sinergis fisika dan CT melalui pemodelan komputasional. ✅
- **Magana, Arigye, Udosen, Lyon, Joshi, & Pienaar (2024)**, *International Journal of STEM Education*, 11, DOI 10.1186/s40594-024-00494-3: 116 mahasiswa termodinamika dalam 24 tim mengerjakan proyek CM ter-*scaffold*. Penelitian ini mengkaji kompetensi representasional (interpretasi kode dan grafik output) serta keterampilan regulasi. ✅

**Implikasi:** CM menyediakan jembatan antara masalah sistem Bumi dan CT, karena memodelkan menuntut dekomposisi, abstraksi, algoritma, pengolahan data, pengujian, dan *debugging*. Namun **CM→CT bukan kebaruan**; hubungan ini sudah mapan.

### 2.5 Scientific Argumentation Scaffolding (SAS) — komponen intervensi 4

- Toulmin (1958/2003): pola argumen *claim–data–warrant–backing–qualifier–rebuttal*, landasan teoretis.
- McNeill, Lizotte, Krajcik, & Marx (2006): kerangka *claim–evidence–reasoning* (CER) dan *scaffold* yang dipudarkan (*fading*), operasionalisasi instruksional. ✅
- Osborne, Erduran, & Simon (2004): kualitas argumentasi diukur dari kehadiran *rebuttal*. ✅
- Belland, Walker, Kim, & Lefler (2017), *Review of Educational Research*: meta-analisis *computer-based scaffolding* di STEM menunjukkan efek positif yang konsisten. ✅
- **Lyon, Fennell, & Magana (2020)**, *Computer Applications in Engineering Education*, 28(4), 837–852, DOI 10.1002/cae.22256: mengkarakterisasi argumen dan penjelasan mahasiswa atas aktivitas CM berbasis disiplin. ✅ (keberadaan terverifikasi; temuan rinci perlu dibaca dari teks lengkap)
- **Wang, Huang, Zheng, Wu, & Zhao (2024/2025)**, *Journal of Research on Technology in Education*, 57(6), DOI 10.1080/15391523.2024.2398504: kuasi-eksperimen 2×2 pada 60 siswa kelas V. Argumentation scaffolding dalam aktivitas STEM **meningkatkan CT dan menurunkan cognitive load**. ✅ (catatan: sampel kecil dan jenjang SD, sehingga perlu dikutip dengan hati-hati)
- Lee, Liu, Pallant, Roohr, Pryputniewicz, & Buck (2014), *Journal of Research in Science Teaching*, 51(5): argumentasi ilmiah yang memuat ketidakpastian dalam modul **High-Adventure Science** (sistem Bumi, model komputasional, dan data nyata). ✅
- Hendratmoko et al.: argumentasi ilmiah tidak cukup berupa klaim; diperlukan evidence, reasoning, counterclaim, dan rebuttal yang di-*scaffold*. 📄

**Posisi SAS:** strategi pembelajaran (variabel bebas), **bukan** kemampuan argumentasi sebagai variabel terikat. SAS digunakan untuk mengubah output model menjadi *evidence* yang harus diuji, dijustifikasi, dipertahankan, dan direvisi.

### 2.6 Domain Fisika Bumi dan Konteks Masalah Autentik

- Møller, Kvarøy, & Hannisdal (2023), *Nordic Journal of STEM Education*: mata kuliah Earth science tingkat sarjana yang memperkenalkan praktik komputasional agar mahasiswa bekerja dengan data nyata dan masalah terbuka. Praktik komputasional bagi pemula menjadi sumber ketidakpastian yang dapat dikurangi melalui kerja kelompok. ✅
- Pallant, Lee, & Pryputniewicz (2019), *Journal of Geoscience Education*: modul "*Will there be enough fresh water?*" mendorong siswa mempertimbangkan ketidakpastian dalam argumen. ✅
- **Konteks Lampung:** banjir 22 Februari 2025 di Bandar Lampung dipicu hujan berintensitas tinggi dan menyebabkan 3 orang meninggal, 30.935 jiwa terdampak, serta lebih dari 9.425 rumah terendam (BNPB, *Buletin Info Bencana* Februari 2025). ✅ Angka "37 titik banjir" yang sering muncul berasal dari kejadian **6 Maret 2026**, bukan Februari 2025, sehingga jangan dicampur.
- Fisika Bumi tercantum sebagai mata kuliah pilihan semester V–VI pada Kurikulum Pendidikan Fisika Unila 2025. RPS rincinya belum dijadikan dasar. 📄

---

## 3. Matriks Hubungan Antarvariabel

| Hubungan | Bukti utama | Kekuatan bukti | Fungsi dalam argumen |
|---|---|---|---|
| Masalah sistem Bumi ↔ kebutuhan CT | Weintrop et al. (2016) memasukkan *systems thinking* serta *modeling & simulation* sebagai praktik CT; Møller et al. (2023) | Kuat (konseptual) | Mengapa Fisika Bumi |
| PBL ↔ Integrated STEM | Roehrig et al. (2021); Kelley & Knowles (2016); Suryadi 📄 | Kuat | Masalah autentik menuntut integrasi disiplin |
| Integrated STEM ↔ CT | Weintrop et al. (2016); Amrizaldi (2025) 📄; Hutchins et al. (2020) | Kuat | Kombinasi ini **bukan** kebaruan |
| CM ↔ CT | Sengupta et al. (2013); Hutchins et al. (2020); review CM ILE 2024 ⚠️ | Kuat | CM sebagai jembatan menuju CT; **bukan** kebaruan |
| CM ↔ Argumentasi | Lyon, Fennell, & Magana (2020); Lee et al. (2014) | Sedang–kuat | Output model belum otomatis menjadi *evidence* ilmiah |
| SAS ↔ CT | Wang et al. (2024/2025) | **Emerging** (satu studi kunci, jenjang SD) | Dasar empiris SAS → CT |
| SAS (scaffolding) di STEM | Belland et al. (2017) | Kuat (meta-analisis) | Scaffold efektif di STEM |
| PBL + STEM + CM + SAS → CT pada masalah sistem Bumi untuk calon guru fisika | Belum ditemukan desain yang sama persis | **Gap potensial** | Harus dibuktikan oleh SLR-RQ6 |

**Rumusan gap yang aman** (dipakai di latar belakang sebelum SLR selesai):
> Literatur telah menunjukkan hubungan A→B, B→C, dan C→D secara parsial, tetapi belum tersedia desain yang menghubungkan *evidence* hasil CM dengan revisi model yang digerakkan argumentasi (*argumentation-driven model revision*) dalam PBL–Integrated STEM pada masalah autentik sistem Bumi untuk mengembangkan CT calon guru fisika.

---

## 4. Daftar Tindak Lanjut

1. **Cek di Scopus** dua review bertanda ⚠️ (CM 70 studi, ILE 2024; CT pendidikan guru 43 artikel, IJER 2025), lalu lengkapi nama penulis di daftar pustaka.
2. **Baca teks lengkap** Lyon et al. (2020) dan Wang et al. (2024/2025) untuk mengambil angka atau temuan spesifik (*effect size*, jenis kesalahan argumen).
3. **Tetapkan kerangka CT**: Weintrop et al. (2016) atau kerangka lain, misalnya Shute et al. (2017), dan cocokkan dengan instrumen yang tersedia untuk mahasiswa.
4. **Ambil RPS Fisika Bumi** untuk menentukan submateri (hidrometeorologi, fluida dan hidrologi, mikroklimat, seismik).
5. **Data curah hujan resmi** banjir Februari 2025 (BMKG Stasiun Klimatologi Lampung) bila ingin memperkuat paragraf konteks.
6. Jalankan **SLR-RQ1 sampai RQ6** sesuai rancangan (hlm. 95–98) untuk memverifikasi semua klaim bertanda [SLR] pada draf latar belakang.
