# 'ONE' GLOBAL HCMS — Learning & Development (LMS Docs App)

Aplikasi dokumentasi interaktif modul **Learning & Development** pada
**'ONE' GLOBAL HCMS** (Nabati). Satu file statis (`index.html`) berisi 62 kartu
Functional Requirement (FR-LD) + matriks cakupan PRD, masing-masing dengan demo
interaktif. Bilingual Indonesia/English, AI bernama **HC AI**.

## Jalankan lokal
Buka `index.html` di browser — tanpa build, tanpa dependensi.

## Login demo
- User: `Nabati-LMS`
- Password: `Semangat!`

## Deploy ke Vercel
Situs statis murni, tidak perlu build step.

**Dashboard:** Import repo di vercel.com -> Framework Preset **Other**
(Build Command & Output Directory dikosongkan) -> **Deploy**.

**CLI:**
```bash
npm i -g vercel
vercel --prod
```

## Cakupan
64 Functional Requirement PRD di 10 famili (HC AI/SMITH, Delivery, Analytics,
LXP, Social, LCMS, Compliance, Admin, Integration, Mobile) terpetakan 100% —
lihat section **Cakupan PRD** di dalam aplikasi.
