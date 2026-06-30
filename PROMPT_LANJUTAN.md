# PROMPT LANJUTAN, ONE HCMS LEARNING (MODULE 09 / LMS)

Salin seluruh blok di bawah ini ke chat baru untuk melanjutkan pekerjaan.

---

Kamu melanjutkan pembangunan ONE HCMS Learning (Module 09, LMS) untuk Nabati Group. Aku Kang Rangga (Rangga Irawan Prasetyo), HR consultant dan Digital HR Architect, panggil aku Kang Rangga. Jawab dalam Bahasa Indonesia, istilah teknis tetap dalam Bahasa Inggris.

ATURAN WAJIB
- Tidak ada em dash dan en dash sama sekali. Pakai koma atau hyphen biasa.
- Output dibuat humanized, tanpa penanda yang membuatnya terbaca sebagai hasil AI.
- Sebelum mengeksekusi tugas, rekomendasikan Sonnet atau Opus berdasarkan kompleksitas.
- Jika aku bilang presentasi, deck, atau pitch, tanya dulu mau pakai Prompt A (Patrick Winston) atau struktur lain.
- Jangan masukkan CHRM BNSP dan Tazkia MEI ke output apa pun. Referensi file permanen ranggairawan.com.
- ONE HCMS (Nabati) dan Nusva People adalah dua produk berbeda, jangan dicampur.

KONTEKS PRODUK
LMS ini portal multi-persona berupa file HTML standalone (self-contained), satu file per persona, meniru pola Module 05 OrgDesign yang sudah dikirim. AI-native global HRMS untuk 32 ribu karyawan lintas 15+ negara, menggantikan HC Portal 1.0. Agent AI tampil sebagai HC AI (branding tunggal, tidak pernah pakai nama Smith atau nama agent individual).

FILE YANG SUDAH JADI (semua live, lolos QA)
1. index.html, launcher login tunggal, 6 kartu persona, toggle ID/EN. Kredensial, username lms_onehcms atau onehcms, password nabatiHC-123!
2. lms_p_learner.html, persona Learner bergaya Coursera (top nav plus search di tengah, hero, carousel kursus, kalender). Identitas Sari Dewi, Operator Produksi fungsi Genba. Surface, Beranda, Katalog, Matriks Skill (tab Standar vs Aktual, Aktual vs N+1, Pindah Job Family 30 fungsi, Kamus Kompetensi Genba), Perjalanan dan Badge, IDP, Kepatuhan, plus Ruang Belajar (video yang berhenti di menit tertentu untuk kuis) yang dibuka lewat tombol.
3. lms_p_linemanager.html, side nav. Identitas Budi Santoso. Surface team, assign, approve (maker-checker termasuk training eksternal), comp, skill.
4. lms_p_instructor.html, side nav. Identitas Hendra Kusuma. Surface studio (module management), scorm (SCORM 1.2/2004, xAPI, AICC, cmi5, plus standar file video optimal), assess (editor checkpoint kuis video), ilt (waktu, trainer, tempat), perf.
5. lms_p_ldadmin.html, side nav. Identitas Dewi Lestari. Surface overview, catalog, enroll, approvals (checker), compliance (Console multi-negara), budget dan vendor.
6. lms_p_hcbp.html, side nav. Identitas Andi Pratama, Manufacturing BU. Surface overview, capability (heatmap fungsi KSNI x klaster kompetensi), succession (bench agregat), learning, compliance, priorities.
7. lms_p_exec.html, side nav. Identitas Ratna Wijaya. Surface overview, capability (plus acuan eksternal WEF, McKinsey, Deloitte), roi (Learning ROI), trends, risk, strategy.
8. kamus_kompetensi_ksni.html, kamus master 30 fungsi KSNI, 346 kompetensi, pencarian, definisi, deskriptor Level 1 sampai 5.

DESIGN SYSTEM (token kanonik)
Google Fonts, Schibsted Grotesk (display), Geist (ui), Geist Mono atau JetBrains Mono (num). Warna, ink #1F242C, ink-2 #525a67, ink-3 #8a93a0, border #e4e8ee, surface-2 #f7f8fa, brand merah #E1231B, role-tint #fdeceb, role-tint2 #f9dad7, green #1f9d57, amber #c47d10, info #2563c9. Topbar dengan aksen merah 3px di atas. Tanpa Bricolage, tanpa Plus Jakarta Sans, tanpa biru Coursera. Learner pakai chrome top-nav ala Coursera, persona operasional dan strategis pakai side nav.

KONVENSI TEKNIS
- Satu file HTML standalone per persona, bilingual ID/EN via setLang, data-lang, dan paintChrome yang me-render ulang seluruh surface.
- JavaScript hanya pakai string concatenation, tidak ada template literal, tidak ada backtick, tidak ada dollar-brace.
- Tidak ada kode FR atau decision code yang tampil di layar (internal saja).
- Persona switcher pakai array REG berisi 6 entri, navigasi jika value bukan SELF.
- Governance terkunci, analitik agregat dengan k-anonymity (minimal 5, lintas-tabel sensitif minimal 10), tidak ada skor risiko, peringkat, atau prediksi individu, prediksi turnover individu (FR-ANALYTICS-004) di-drop. Maker-checker, Line Manager dan Instructor sebagai maker, L&D Admin sebagai checker, checker tidak bisa menyetujui pengajuannya sendiri.
- Kompetensi mengikuti Kerangka Leveling Competency KSNI, disinkronkan dari modul Performance sebagai satu sumber kebenaran. Data karyawan dari ECA, jalur karier dari Career.

INTEGRASI KOMPETENSI KSNI
Matriks skill Learner memakai kompetensi Genba nyata. Simulator Pindah Job Family memuat 30 fungsi, kolom kiri kompetensi yang dikuasai di fungsi asal, kolom kanan kompetensi yang dibutuhkan di fungsi tujuan, penanda hijau untuk yang langsung transferable. Heatmap HRBP memakai fungsi KSNI nyata (Genba, HSE, Manufacture, QA, Maintenance, Warehouse) terhadap klaster kompetensi.

CARA BUILD DAN QA
Tiap file dihasilkan oleh Python builder yang menyuntik shared CSS dan logo, lalu menulis HTML standalone. QA pakai qa.js (jsdom), cek sintaks, integritas getElementById, scan em dash dan en dash, render smoke setiap surface di ID dan EN, dan switcher 6 opsi.

SUMBER PRD
Google Drive doc id 1K-mjk7hZAIXxego9EmSbdbPcXGT-U1uCs5bKCtFJBJU (07. PRD Learning Management System v1.0). Keluarga FR, FR-LCMS, FR-DELIVERY, FR-LXP, FR-ADMIN, FR-ANALYTICS, FR-SMITH (di-rebrand HC AI), FR-INTEGRATION, FR-COMPLIANCE.

CATATAN PENTING UNTUK MELANJUTKAN
File di container tidak ikut berpindah antar sesi. Untuk membangun lagi, aku akan upload ulang ke-8 file HTML dan dua ZIP kompetensi (Kompetensi_KSNI_Manufacture.zip dan Kompetensi_KSNI_Non_Manufacture.zip).

KEMUNGKINAN LANGKAH LANJUTAN
- Halaman detail kursus bergaya Coursera (tab About, Outcomes, Reviews, distribusi rating).
- Matriks traceability final yang memetakan keenam persona ke seluruh FR PRD.
- Normalisasi Corporate HC menjadi kompetensi induk (sekitar 12 sampai 16) agar setara fungsi lain.
- Pembersihan baris klaster gabungan di Channel Development GT.
- Pemetaan leveling per posisi nyata dari workbook ke matriks dan succession.

Konfirmasi kamu paham konteksnya, rekomendasikan model, lalu tunggu instruksiku.
