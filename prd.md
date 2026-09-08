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
- **Nomor WhatsApp & CTA**: Menggunakan WhatsApp resmi `+6288989643555` yang mengatasnamakan `Vendor Hampers`.

---

## 6. Struktur Konten & Navigasi Internal (Content Structure & SEO On-Page)

### 6.1. Daftar Isi (Table of Contents / TOC)
- Setiap artikel wajib memiliki blok **Daftar Isi** (`.article-toc`) yang diletakkan setelah paragraf pembuka/pengantar.
- Setiap poin dalam daftar isi harus terhubung melalui *anchor link* (`#id-heading`) ke masing-masing subjudul (`<h2>`/`<h3>`) yang bersangkutan.
- Desain daftar isi mengikuti tema luxury website (*background champagne*, border aksen emas, font Playfair/Poppins).

### 6.2. Link Internal (Internal Linking Strategy)
Setiap artikel wajib memuat dua jenis tautan internal:
1. **Contextual Internal Links (Dalam Paragraf)**:
   - Menghubungkan kata kunci kontekstual ke halaman produk (`produk.html`, `Tumbler-Custom-Logo.html`), halaman artikel pilar/terkait lainnya (`artikel-rekomendasi-souvenir-day1.html`, dll.), serta halaman kontak (`kontak.html`).
   - Format styling tautan: warna emas tua (`var(--gold-dark)`), font tebal (`font-weight: 600`), dan bergaris bawah.
2. **Inline Banner "Baca Juga"**:
   - Menyisipkan kartu rujukan artikel (`.baca-juga-inline`) di antara paragraf pada bagian tengah artikel untuk meningkatkan *engagement* pembaca dan menurunkan *bounce rate*.

---

## 7. Prosedur Integrasi & Publikasi (Checklist Publikasi)

Sebelum artikel dinyatakan selesai, pastikan langkah-langkah berikut telah terpenuhi:

- [x] **File HTML Dibuat**: File tersimpan di *root* dengan struktur HTML valid dan responsif.
- [x] **Gambar Terpasang**: Format WebP, berwatermark, ukuran < 60 KB, path sesuai.
- [x] **Brand Resmi**: Menggunakan nama **Vendor Hampers** tanpa penyebutan `PT.` / `PT. Tim Souvenir Indonesia`.
- [x] **Daftar Isi & Anchor**: Berfungsi dengan baik saat diklik menuju section terkait.
- [x] **Link Internal Aktif**: Mengarah ke halaman internal yang relevan.
- [x] **Listing di `blog.html`**: Kartu artikel baru ditambahkan di urutan teratas grid blog dengan nama penulis **Reza Maulana Nehru**.
- [x] **Pembaruan `sitemap.xml`**: URL artikel dan gambar baru didaftarkan pada sitemap XML.
