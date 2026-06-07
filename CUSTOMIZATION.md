# 🎨 Panduan Kustomisasi

## Mengubah Warna

### Mengakses CSS Variables

1. Dashboard Blogger → **Theme** → **Edit HTML**
2. Tekan Ctrl+F untuk search
3. Cari `:root {`
4. Edit nilai variable sesuai keinginan

### Daftar CSS Variables

```css
:root {
  /* Primary Colors */
  --primary: #1565C0;           /* Warna utama (navy blue) */
  --primary-light: #1E88E5;     /* Warna utama terang */
  --primary-darker: #0D47A1;    /* Warna utama gelap */
  
  /* Accent Colors */
  --gold: #D4A017;              /* Warna accent (gold) */
  --teal: #00897B;              /* Warna accent sekunder (teal) */
  
  /* Background Colors */
  --bg-body: #F5F7FA;           /* Background body */
  --bg-primary: #FFFFFF;        /* Background cards */
  
  /* Text Colors */
  --text-primary: #1A202C;      /* Teks utama */
  --text-secondary: #4A5568;    /* Teks sekunder */
  
  /* Border & Shadow */
  --border: #E2E8F0;            /* Border color */
  --shadow-md: 0 4px 16px rgba(0,0,0,0.08); /* Shadow */
}
```

### Contoh Perubahan Warna

**Mengubah ke Warna Merah:**
```css
--primary: #C62828;           /* Red */
--primary-light: #E53935;
--primary-darker: #B71C1C;
```

**Mengubah ke Warna Hijau:**
```css
--primary: #00796B;           /* Teal Green */
--primary-light: #00897B;
--primary-darker: #004D40;
```

**Mengubah ke Warna Ungu:**
```css
--primary: #7B1FA2;           /* Purple */
--primary-light: #9C27B0;
--primary-darker: #6A1B9A;
```

---

## Mengubah Font

### Langkah 1: Buka Font Section
Cari di `<head>` bagian ini:
```xml
<link href='https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=Playfair+Display:wght@700;800&display=swap' rel='stylesheet'/>
```

### Langkah 2: Pilih Font dari Google Fonts
1. Kunjungi [fonts.google.com](https://fonts.google.com)
2. Cari font yang diinginkan
3. Klik font, pilih weights yang dibutuhkan
4. Copy link `<link>` atau `@import`

### Langkah 3: Ganti di Template
```xml
<!-- LAMA -->
<link href='https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=Playfair+Display:wght@700;800&display=swap' rel='stylesheet'/>

<!-- BARU (Contoh: Poppins + Merriweather) -->
<link href='https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800&family=Merriweather:wght@700;800&display=swap' rel='stylesheet'/>
```

### Langkah 4: Update CSS Font Family
Cari di CSS dan ubah:
```css
/* LAMA */
body { font-family: 'Plus Jakarta Sans', -apple-system, BlinkMacSystemFont, sans-serif; }
h1, h2, h3, h4, h5, h6 { font-family: 'Playfair Display', serif; }

/* BARU */
body { font-family: 'Poppins', -apple-system, BlinkMacSystemFont, sans-serif; }
h1, h2, h3, h4, h5, h6 { font-family: 'Merriweather', serif; }
```

---

## Mengubah Layout

### Mengubah Lebar Container
```css
.container { max-width: 1280px; } /* Ubah nilai ini */
```

**Rekomendasi:**
- Layar besar: `1280px` (desktop)
- Layar medium: `1024px` (tablet besar)
- Layar kecil: `768px` (tablet kecil)

### Mengubah Padding/Margin
```css
.container { padding: 0 24px; } /* Ubah nilai ini */
```

---

## Mengubah Header

### Mengubah Tinggi Header
Cari di CSS:
```css
--header-h: 68px; /* Ubah nilai ini */
```

### Mengubah Logo
1. Dashboard → **Theme** → **Customize**
2. Cari bagian **Header Image**
3. Upload image baru

---

## Menambah Custom CSS

### Metode 1: Tambah di Dalam `<b:skin>`

1. Buka Theme HTML Editor
2. Cari `</b:skin>` (bagian akhir CSS)
3. Tambah CSS baru sebelum tag penutup:

```css
/* Custom Styles */
.my-custom-class {
  background: #1565C0;
  padding: 20px;
  border-radius: 8px;
  color: white;
}
```

### Metode 2: Override Existing Styles

```css
/* Override warna link */
a { color: #D4A017 !important; }

/* Override background card */
.post-card { background: #f0f4f8 !important; }
```

---

## Menambah Widget Custom

### Langkah 1: Buka Layout
Dashboard → **Layout**

### Langkah 2: Tambah Widget
Klik **+ Add a Gadget**

### Langkah 3: Pilih Jenis Widget
- **HTML/JavaScript** - Untuk kode custom
- **Image** - Untuk banner/logo
- **Text** - Untuk konten statis
- **Followers** - Untuk followers widget
- **Labels** - Untuk daftar label/kategori

### Contoh: Tambah Subscribe Button
```html
<div style="text-align: center; padding: 20px;">
  <h3>Daftar Newsletter</h3>
  <p>Dapatkan artikel terbaru langsung ke email Anda</p>
  <!-- Ganti dengan form Anda -->
  <input type="email" placeholder="Email Anda" style="width: 100%; padding: 10px;">
  <button style="width: 100%; padding: 10px; background: #1565C0; color: white; border: none; border-radius: 5px; cursor: pointer; margin-top: 10px;">
    Subscribe
  </button>
</div>
```

---

## Mengubah Mobile Menu

### Ubah Responsive Breakpoint

Cari di CSS:
```css
@media (max-width: 768px) { /* Ubah nilai ini */ }
```

Nilai umum:
- `768px` - Tablet & mobile
- `1024px` - Tablet besar
- `1280px` - Desktop kecil

---

## Menambah Social Media Links

### Di Footer atau Sidebar

Tambah HTML ini:
```html
<div class="social-links">
  <a href="https://facebook.com/yourpage" title="Facebook"><i class="fab fa-facebook"></i></a>
  <a href="https://twitter.com/yourhandle" title="Twitter"><i class="fab fa-twitter"></i></a>
  <a href="https://instagram.com/yourhandle" title="Instagram"><i class="fab fa-instagram"></i></a>
  <a href="https://youtube.com/yourchannel" title="YouTube"><i class="fab fa-youtube"></i></a>
</div>
```

Tambah CSS:
```css
.social-links {
  display: flex;
  gap: 10px;
  justify-content: center;
}

.social-links a {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 40px;
  height: 40px;
  background: var(--primary);
  color: white;
  border-radius: 50%;
  transition: all 0.3s ease;
}

.social-links a:hover {
  background: var(--primary-darker);
  transform: scale(1.1);
}
```

---

## Advanced: Mengubah Post Card Style

### Lebih Banyak Shadow
```css
.post-card {
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15) !important;
}
```

### Lebih Banyak Border Radius
```css
.post-card {
  border-radius: 16px !important;
}
```

### Hover Effect
```css
.post-card:hover {
  transform: translateY(-8px) !important;
  box-shadow: 0 15px 40px rgba(0, 0, 0, 0.2) !important;
}
```

---

## Tips & Trik

### 1. Backup Sebelum Edit
Selalu backup theme sebelum melakukan perubahan besar:
- Dashboard → **Theme** → **⋮** → **Backup/Restore** → **Download tema lengkap**

### 2. Test di Multiple Devices
Jangan lupa test perubahan di:
- Desktop
- Tablet
- Mobile

### 3. Clear Cache
Jika perubahan tidak terlihat:
- Browser: Ctrl+Shift+Delete (clear cache)
- Blog: Tunggu 5-10 menit

### 4. Gunakan Developer Tools
- Tekan F12 di browser
- Gunakan Inspector untuk test CSS langsung
- Lihat element mana yang perlu diubah

### 5. Dokumentasikan Perubahan
Catat semua perubahan yang Anda buat untuk referensi di masa depan.

---

## Resources

- [Google Fonts](https://fonts.google.com)
- [Color Palette Generator](https://coolors.co)
- [CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [Font Awesome Icons](https://fontawesome.com/icons)
- [Blogger XML Reference](https://support.google.com/blogger/answer/46995)

---

**Selamat kustomisasi! Jika ada pertanyaan, silakan buat issue di GitHub.** 🚀