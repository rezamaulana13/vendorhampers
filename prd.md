# Product Requirement Document (PRD) — Standar Pembuatan & Publikasi Artikel Website Vendor Hampers

## 1. Ikhtisar Dokumen (Overview)
Dokumen ini berfungsi sebagai panduan standar operasional dan spesifikasi teknis (PRD) dalam proses produksi, pemformatan, optimasi gambar, dan publikasi artikel blog baru pada website **Vendor Hampers** (`vendorhampers.web.id`). Panduan ini disusun berdasarkan serangkaian aturan dan perbaikan yang telah ditetapkan.

---

## 2. Struktur & Penamaan File (File & URL Conventions)

### 2.1. Penamaan File HTML
- Setiap artikel baru harus dibuatkan file `.html` mandiri di direktori utama (*root*) website.
- Nama file wajib mengikuti judul artikel dengan format *slug/kebab-case* (huruf kecil semua dipisahkan tanda hubung `-`) untuk menjamin URL yang rapi dan SEO-friendly.
- **Contoh Kasus**:
  - Judul: `Souvenir Pernikahan Mewah dan Berkesan untuk Wedding 2026`
  - File: `souvenir-pernikahan-mewah-dan-berkesan-untuk-wedding-2026.html`

### 2.2. Metadata & Tag Kanonikal
- Wajib menyertakan tag `<title>`, `<meta name="description">`, `<meta name="keywords">`, `<meta name="robots">`.
- Tag `<link rel="canonical">`, Open Graph (`og:url`, `og:image`), serta Twitter Cards harus merujuk ke URL file yang tepat.
- Menyertakan structured data Schema JSON-LD lengkap (*Article*, *LocalBusiness*, *Organization*, dan *BreadcrumbList*).

---

## 3. Spesifikasi & Optimasi Gambar Artikel (Featured Image)

| Kriteria | Ketentuan Standar |
| :--- | :--- |
| **Format File** | `.webp` *(Wajib format WebP modern)* |
| **Ukuran Maksimal** | **Maksimal 60 KB** (harus terkompresi dengan kualitas visual tetap tajam) |
| **Rasio & Resolusi** | Rasio `16:9` (Standar: `1200 x 675 px`) |
| **Watermark** | Wajib memiliki watermark brand (*Vendor Hampers / vendorhampers.web.id*) dengan badge elegan semi-transparan di sudut kanan bawah |
| **Lokasi Penyimpanan** | `assets/img/blog/[nama-gambar].webp` |
| **Alt Text** | Wajib deskriptif dan mengandung kata kunci utama artikel |

---

## 4. Standar Penulis (Author Standardization)

Mulai pembaruan ini, seluruh artikel baru dan kartu publikasi wajib menggunakan identitas penulis resmi berikut:
- **Nama Penulis**: `Reza Maulana Nehru`
- **Inisial Avatar**: `RN`
- **Avatar Generator URL**: `https://placehold.co/150x150/2b2622/ffffff?text=RN&font=raleway` (untuk halaman artikel) dan `https://placehold.co/48x48/2b2622/ffffff?text=RN&font=raleway` (untuk kartu blog).
- **Bio Penulis**: *Content Writer di Vendor Hampers, aktif menulis seputar souvenir pernikahan, hampers, dan inspirasi hadiah premium untuk berbagai momen spesial.*
- **Penerapan Identitas**:
  1. Header meta artikel (`Oleh: Reza Maulana Nehru`)
  2. Author box di akhir isi artikel
  3. Kartu listing artikel di halaman `blog.html`

---

## 5. Standar Penamaan Brand & Entitas Bisnis (Brand & Business Entity)

- **Ketentuan Brand**: Seluruh artikel, metadata, schema markup, dan CTA **TIDAK BOLEH** menggunakan sebutan badan usaha seperti **`PT.`** ataupun nama **`PT. Tim Souvenir Indonesia`**.
- **Nama Brand Resmi**: Wajib menggunakan nama brand resmi **`Vendor Hampers`** (website: `vendorhampers.web.id`).
- **Nomor WhatsApp & CTA**: Menggunakan WhatsApp resmi `+6288989643555` yang mengatasnamakan `Vendor Hampers`- **Tautan Website Jaringan (Footer)**: Bagian `footer-contact` wajib memuat tombol tautan jaringan/partner menuju `https://vendormerchandise.web.id/` dengan label `vendormerchandise.web.id`.
- **Lokasi yang Kami Layani (Footer 5-Kolom)**: Ditempatkan pada kolom ke-4 (sebelum kolom *Hubungi Kami*) dalam format daftar teks 2 kolom yang rapi dengan bullet emas, memuat 11 kota layanan resmi: *Jakarta, Surabaya, Bandung, Yogyakarta, Semarang, Malang, Denpasar, Makassar, Balikpapan, Samarinda, Palembang*.

---

## 6. Standar AEO, GEO, dan Local SEO Berbasis Kota Layanan

Untuk memaksimalkan visibilitas website pada mesin pencari tradisional (Google Search) maupun mesin pencari kecerdasan buatan (*AI Search Engines / Generative AI* seperti Google AI Overviews/SGE, ChatGPT Search, Perplexity, dan Copilot), setiap pembuatan halaman dan artikel wajib mengintegrasikan standar **AEO, GEO, dan Local SEO** berikut:

### 6.1. Daftar Resmi 11 Kota Layanan (Target Entity)
1. **Jakarta** (Jabodetabek / Pusat Bisnis Nasional)
2. **Surabaya** (Jawa Timur & Hub Indonesia Timur)
3. **Bandung** (Jawa Barat & Korporasi Kreatif)
4. **Yogyakarta** (DIY, Pendidikan, & Budaya)
5. **Semarang** (Jawa Tengah & Kawasan Industri)
6. **Malang** (Jawa Timur / Workshop & Pusat Produksi)
7. **Denpasar** (Bali, Pariwisata, & Event Internasional)
8. **Makassar** (Sulawesi Selatan & Pintu Masuk Indonesia Timur)
9. **Balikpapan** (Kalimantan Timur & Penunjang Korporasi IKN)
10. **Samarinda** (Kalimantan Timur & Sentra Pemerintahan)
11. **Palembang** (Sumatera Selatan & Bisnis Regional)

### 6.2. Strategi Answer Engine Optimization (AEO)
- **Direct Answer Format**: Setiap heading `<h2>` berbentuk pertanyaan wajib diikuti oleh **1–2 kalimat jawaban ringkas, tegas, dan berbobot (direct answer)** di awal paragraf sebelum pembahasan mendalam. Format ini memudahkan mesin AI mengambil kutipan instan (*snippet extraction*).
- **Target Query Berbasis Lokasi**: Menjawab pertanyaan umum pengguna seperti *"Bagaimana cara pesan hampers kantor untuk cabang Surabaya/Jakarta?"* atau *"Berapa lama estimasi pengiriman hampers corporate ke Makassar & Balikpapan?"*.

### 6.3. Strategi Generative Engine Optimization (GEO)
- **Semantic Entity Enrichment**: Menyebutkan nama-nama kota layanan dan kawasan industri/perkantoran secara alami di dalam konten (misal: area perkantoran Sudirman-Jakarta, Rungkut-Surabaya, hingga proyek IKN di Balikpapan-Samarinda) untuk memperkuat relevansi semantik brand di mata LLM (*Large Language Models*).
- **Knowledge Graph Association**: Mempertegas asosiasi brand **Vendor Hampers** sebagai vendor terpercaya untuk kategori *corporate gift*, *souvenir kantor*, dan *hampers custom* di 11 kota tersebut.

### 6.4. Strategi Local SEO & Schema Markup
- **Structured Data JSON-LD (`areaServed`)**:
  Setiap file halaman wajib menyertakan array `areaServed` lengkap pada skema `LocalBusiness` dan `Organization`:
  ```json
  "areaServed": [
    { "@type": "City", "name": "Malang" },
    { "@type": "City", "name": "Surabaya" },
    { "@type": "City", "name": "Jakarta" },
    { "@type": "City", "name": "Bandung" },
    { "@type": "City", "name": "Yogyakarta" },
    { "@type": "City", "name": "Semarang" },
    { "@type": "City", "name": "Denpasar" },
    { "@type": "City", "name": "Makassar" },
    { "@type": "City", "name": "Balikpapan" },
    { "@type": "City", "name": "Samarinda" },
    { "@type": "City", "name": "Palembang" },
    { "@type": "Country", "name": "Indonesia" }
  ]
  ```
- **Meta Tag GEO**: Menyertakan koordinat origin workshop dan geo-region resmi Jawa Timur/Indonesia pada header dokumen.

---

## 7. Struktur Konten & Navigasi Internal (Content Structure & SEO On-Page)

### 7.1. Format Judul Subheading (Wajib Berbentuk Pertanyaan)
- Seluruh tag `<h2>` (dan sub-heading utama) **WAJIB diubah ke dalam bentuk pertanyaan informatif dan ramah pencarian pengguna**.
  - *Contoh*: Dari `"Tahapan Produksi Box Souvenir Kayu"` diubah menjadi `"Berapa Lama Tahapan Produksi Box Souvenir Kayu?"` atau `"Bagaimana Tahapan Produksi Box Souvenir Kayu Custom?"`.
- **Integrasi FAQ ke Heading**: Pertanyaan-pertanyaan seputar kebutuhan konsumen disebarkan langsung sebagai sub-heading artikel (`<h2>`/`<h3>`) yang mengalir secara alami, bukan dikumpulkan dalam section FAQ accordion terpisah di bagian akhir.

### 7.2. Daftar Isi (Table of Contents / TOC)
- Setiap artikel wajib memiliki blok **Daftar Isi** (`.article-toc`) yang diletakkan setelah paragraf pembuka/pengantar.
- Setiap poin dalam daftar isi harus terhubung melalui *anchor link* (`#id-heading`) ke masing-masing subjudul pertanyaan (`<h2>`/`<h3>`) yang bersangkutan.
- Desain daftar isi mengikuti tema luxury website (*background champagne*, border aksen emas, font Playfair/Poppins).

### 7.3. Tabel Data & Transparansi Harga Produk
- **Minimal 1 Tabel Data per Artikel**: Wajib menyertakan minimal satu tabel data responsif (`<table>` dengan styling premium emas/charcoal).
- **Isi Tabel**: Tabel dapat memuat perbandingan spesifikasi material/finishing, kisaran biaya berdasarkan jumlah pemesanan (kuantitas), atau paket kombinasi isi.
- **Pencantuman Harga Produk**: Wajib mencantumkan harga atau estimasi kisaran harga produk Vendor Hampers sendiri secara transparan dan masuk akal sesuai pasar.

### 7.4. Kutipan Sumber Eksternal yang Valid
- Jika artikel mengutip data angka, statistik pasar, atau referensi industri, **wajib menggunakan sumber eksternal yang benar-benar valid dan kredibel** (seperti data Kemenparekraf, asosiasi resmi, atau referensi riset nyata).
- Dilarang keras menaruh nama media sembarangan semata-mata untuk menciptakan kesan kredibel tanpa referensi klaim yang nyata.

### 7.5. Link Internal Alami (Natural Internal Linking Strategy)
Setiap artikel wajib memuat dua jenis tautan internal:
1. **Contextual Internal Links (Dalam Paragraf)**:
   - Menghubungkan kata kunci kontekstual secara mengalir dan natural ke halaman produk (`produk.html`, `Tumbler-Custom-Logo.html`), artikel pilar/terkait lainnya (`artikel-rekomendasi-souvenir-day1.html`, dll.), serta halaman kontak (`kontak.html`).
   - Format styling tautan: warna emas tua (`var(--gold-dark)`), font tebal (`font-weight: 600`), dan bergaris bawah.
2. **Inline Banner "Baca Juga"**:
   - Menyisipkan kartu rujukan artikel (`.baca-juga-inline`) di antara paragraf pada bagian tengah artikel untuk meningkatkan *engagement* pembaca dan menurunkan *bounce rate*.

### 7.6. Checklist Ringkas / Bagian Referensi Penutup
- Sebelum tombol CTA penutup, artikel **wajib ditutup dengan blok Checklist Ringkas** (misal: daftar periksa persiapan pemesanan) atau **Bagian Referensi Panduan** (`.article-checklist-box`) agar pembaca memperoleh kesimpulan praktis yang dapat langsung dieksekusi.

---

## 8. Prosedur Integrasi & Publikasi (Checklist Publikasi)

Sebelum artikel dinyatakan selesai, pastikan langkah-langkah berikut telah terpenuhi:

- [x] **File HTML Dibuat**: File tersimpan di *root* dengan struktur HTML valid dan responsif.
- [x] **Gambar Terpasang**: Format WebP, berwatermark, ukuran < 60 KB, path sesuai.
- [x] **Brand Resmi**: Menggunakan nama **Vendor Hampers** tanpa penyebutan `PT.` / `PT. Tim Souvenir Indonesia`.
- [x] **Sub-heading Pertanyaan (H2)**: Seluruh `<h2>` diformat dalam bentuk kalimat tanya yang jelas dan kontekstual.
- [x] **Daftar Isi & Anchor**: Berfungsi dengan baik saat diklik menuju section pertanyaan terkait.
- [x] **Tabel Data & Harga**: Memuat minimal 1 tabel data perbandingan/spesifikasi dan kisaran harga produk.
- [x] **Sumber Valid**: Kutipan data eksternal berasal dari sumber yang nyata dan relevan.
- [x] **AEO & GEO Ready**: Memuat direct answer ringkas di bawah H2 dan konteks wilayah kota layanan.
- [x] **Link Internal Natural**: Tautan kontekstual dan kartu *Baca Juga* terpasang rapi.
- [x] **Checklist Penutup**: Terdapat checklist ringkas atau bagian referensi sebelum CTA penutup.
- [x] **Footer Partner Link & Kota Layanan**: Tautan redirect ke `vendormerchandise.web.id` dan 11 kota layanan terpasang di kolom ke-4 footer.
- [x] **Listing di `blog.html`**: Kartu artikel baru ditambahkan di urutan teratas grid blog dengan nama penulis **Reza Maulana Nehru**.
- [x] **Pembaruan `sitemap.xml`**: URL artikel dan gambar baru didaftarkan pada sitemap XML.
