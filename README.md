# 🎓 Catatan Guru IPS — Blogger XML Theme V5

**Catatan Guru IPS V5 Government-Futuristic Edition**

Tema Blogger XML yang telah di-redesign dengan gaya **governmental-institutional** yang modern dan futuristik. Warna cerah, bersih, profesional — terinspirasi dari situs resmi pemerintah dan dinas.

---

## ✨ Fitur Utama

- ✅ **Responsive Design** — Mobile-first, tampil sempurna di semua ukuran layar
- ✅ **Bright & Clean Color Scheme** — Navy blue primary, gold accent, white background
- ✅ **Futuristic UI** — Glassmorphism, gradient accents, clean geometric cards
- ✅ **Dark/Light Mode Toggle** — Otomatis tersimpan di localStorage
- ✅ **Reading Progress Bar** — Indikator progres baca di bagian atas
- ✅ **Smooth Scroll Animations** — IntersectionObserver-based reveal effects
- ✅ **Hero Section** — Landing area dengan featured cards
- ✅ **CPNS SKD Section** — Area khusus latihan SKD CPNS
- ✅ **Sponsor/Mitra Section** — Partnership showcase
- ✅ **Sidebar Widgets** — Popular Posts, Labels, Statistics
- ✅ **Search Overlay** — Pencarian dengan keyboard shortcut (Ctrl+K)
- ✅ **Back-to-Top Button** — Navigasi cepat ke atas
- ✅ **Mobile Navigation** — Hamburger menu dengan dropdown support
- ✅ **Copy Link Button** — Salin URL artikel dengan satu klik
- ✅ **SEO Optimized** — JSON-LD structured data, Open Graph, Twitter Cards
- ✅ **Font Awesome 6.5** — Ikon modern dan lengkap
- ✅ **Google Fonts** — Plus Jakarta Sans + Playfair Display

---

## 🎨 Palet Warna

| Elemen | Warna | Kode |
|--------|-------|------|
| Primary | Navy Blue | `#0C4A6E` |
| Primary Light | Sky Blue | `#0EA5E9` |
| Accent | Gold/Amber | `#D97706` |
| Background | White | `#FFFFFF` |
| Surface | Light Gray | `#F1F5F9` |
| Text Primary | Dark Slate | `#0F172A` |
| Text Secondary | Slate | `#475569` |
| Gradient | Blue → Teal | `#0C4A6E → #0D9488` |

---

## 📁 Struktur File

```
Blogger-Theme-V5-Government-Futuristic/
├── catatanguruips-v5-government-futuristic.xml    # Template Blogger XML lengkap
├── README.md                                       # Dokumentasi utama
├── INSTALLATION.md                                 # Panduan instalasi detail
├── CUSTOMIZATION.md                                # Panduan kustomisasi
├── LICENSE                                         # Lisensi open source
└── docs/
    ├── COLOR_PALETTE.md                           # Referensi warna lengkap
    ├── STRUCTURE.md                               # Penjelasan struktur XML
    └── TROUBLESHOOTING.md                         # FAQ & solusi masalah
```

---

## 🚀 Cara Install

### Metode 1: Direct Import

1. Buka [Blogger Dashboard](https://www.blogger.com/) → **Theme** → **Edit HTML**
2. Hapus semua kode yang ada
3. **Copy** seluruh isi file `catatanguruips-v5-government-futuristic.xml`
4. **Paste** ke editor HTML Blogger
5. Klik **Save**
6. Selesai! ✅

### Metode 2: Download & Upload

1. Download file `catatanguruips-v5-government-futuristic.xml`
2. Buka Blogger Dashboard → **Theme** → **Backup/Restore**
3. Klik **Choose File** dan pilih file XML yang telah didownload
4. Klik **Upload**
5. Selesai! ✅

---

## ⚙️ Konfigurasi

### Mengubah Warna Primary

Cari di dalam CSS:
```css
:root {
  --primary: #1565C0;  /* Ubah kode warna di sini */
  --primary-light: #1E88E5;
  --primary-darker: #0D47A1;
}
```

### Mengubah Font

Cari di bagian `<head>`:
```xml
<link href='https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=Playfair+Display:wght@700;800&display=swap' rel='stylesheet'/>
```

Ganti dengan font pilihan Anda dari Google Fonts.

---

## 📝 Catatan Penting

- ✓ Semua tag Blogger XML (`b:if`, `b:loop`, `b:section`, `b:widget`, `data:`, `expr:`) dipertahankan utuh
- ✓ Struktur dan fungsionalitas identik dengan versi asli
- ✓ Perubahan hanya pada CSS (warna, styling, layout visual)
- ✓ Kompatibel dengan Blogger Widget v2
- ✓ Responsive dan mobile-friendly
- ✓ SEO-optimized dengan Open Graph & Twitter Cards

---

## 🛠️ Browser Support

| Browser | Support | Catatan |
|---------|---------|----------|
| Chrome | ✅ | Full support |
| Firefox | ✅ | Full support |
| Safari | ✅ | Full support |
| Edge | ✅ | Full support |
| IE 11 | ⚠️ | Partial support |

---

## 🤝 Kontribusi

Anda dapat berkontribusi dengan:
- Melaporkan bug
- Mengusulkan fitur baru
- Membuat pull request dengan improvement
- Berbagi feedback dan saran

---

## 👤 Author

**Catatan Guru IPS** — Portal edukasi IPS, Bank Soal, CPNS SKD, dan EdTech Tools

🌐 Website: [catatanguruips.com](https://catatanguruips.com)  
📧 Email: contact@catatanguruips.com  
🐙 GitHub: [@guruips](https://github.com/guruips)

---

## 📄 Lisensi

Template ini dirilis di bawah lisensi **MIT** dan bebas digunakan untuk keperluan pribadi, komersial, dan edukasi. Silakan sesuaikan konten sesuai kebutuhan Anda.

Baca lengkap di file [LICENSE](./LICENSE).

---

## 📚 Dokumentasi Tambahan

- [Panduan Instalasi Detail](./INSTALLATION.md)
- [Panduan Kustomisasi](./CUSTOMIZATION.md)
- [Referensi Palet Warna](./docs/COLOR_PALETTE.md)
- [Penjelasan Struktur XML](./docs/STRUCTURE.md)
- [FAQ & Troubleshooting](./docs/TROUBLESHOOTING.md)

---

## 📊 Statistik

- **Lines of Code**: ~1200+
- **CSS Variables**: 20+
- **Responsive Breakpoints**: 4
- **SEO Meta Tags**: 15+
- **Supported Languages**: Blogger multi-language

---

**Last Updated**: June 7, 2026  
**Version**: 5.0.0  
**Status**: Active & Maintained ✅