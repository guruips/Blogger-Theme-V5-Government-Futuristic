# 📦 Panduan Instalasi

## Prasyarat

- Akun Blogger aktif
- Browser modern (Chrome, Firefox, Safari, Edge)
- Koneksi internet stabil

---

## Metode 1: Import Langsung (Rekomendasi)

### Langkah Demi Langkah

1. **Buka Dashboard Blogger**
   - Kunjungi [blogger.com](https://www.blogger.com)
   - Login dengan akun Google Anda
   - Pilih blog yang ingin di-update

2. **Akses Pengaturan Theme**
   - Di sidebar kiri, klik **Theme**
   - Klik icon **⋮** (tiga titik) → **Edit HTML**

3. **Backup Theme Lama (Opsional tapi Direkomendasikan)**
   - Klik **⋮** → **Backup/Restore**
   - Klik **Download tema lengkap**
   - Simpan file XML di komputer Anda

4. **Copy Kode Baru**
   - Buka file `catatanguruips-v5-government-futuristic.xml` di editor teks
   - Select All (Ctrl+A) dan Copy (Ctrl+C)

5. **Paste ke Blogger**
   - Di editor HTML Blogger, pilih semua kode (Ctrl+A)
   - Hapus (Delete)
   - Paste kode baru (Ctrl+V)

6. **Simpan Theme**
   - Klik tombol **Save theme** di kanan atas
   - Tunggu hingga proses selesai (2-3 detik)
   - Anda akan melihat notifikasi sukses

7. **Preview & Test**
   - Klik **View blog** untuk melihat hasilnya
   - Refresh page (F5) jika belum terlihat perubahan

---

## Metode 2: Upload File (Alternatif)

### Untuk Pengguna Mobile atau Browser Terbatas

1. **Buka Backup/Restore**
   - Dashboard Blogger → **Theme** → **⋮** → **Backup/Restore**

2. **Upload File**
   - Klik tombol **Choose File**
   - Cari dan pilih `catatanguruips-v5-government-futuristic.xml`
   - Klik **Upload**

3. **Konfirmasi**
   - Klik **OK** pada dialog konfirmasi
   - Tunggu proses upload selesai

4. **Verifikasi**
   - Refresh halaman blog Anda
   - Pastikan theme telah terbentuk dengan baik

---

## 🔧 Troubleshooting Instalasi

### Masalah: Kode XML Tidak Bisa di-Paste

**Solusi:**
- Gunakan browser Chrome atau Firefox
- Hapus extension browser yang mungkin mengganggu
- Clear cache browser (Ctrl+Shift+Delete)
- Coba di browser berbeda

### Masalah: Error saat Save Theme

**Solusi:**
- Pastikan internet connection stabil
- Refresh halaman dan coba lagi
- Periksa apakah ada karakter khusus yang rusak
- Download ulang file `catatanguruips-v5-government-futuristic.xml`

### Masalah: Theme Tidak Tampil dengan Benar

**Solusi:**
- Bersihkan cache browser (Ctrl+Shift+Delete)
- Refresh halaman blog (Ctrl+F5)
- Tunggu 5-10 menit untuk propagasi penuh
- Coba di browser/device lain

### Masalah: Widgets Tidak Tampil

**Solusi:**
- Klik **Layout** di sidebar Blogger
- Pastikan widgets sudah ditambahkan ke area yang tepat
- Refresh halaman layout
- Klik **Save arrangement**

---

## ✅ Verifikasi Instalasi Berhasil

Setelah instalasi, pastikan hal berikut:

- [ ] Header terlihat dengan logo dan navigasi
- [ ] Footer terlihat dengan informasi blog
- [ ] Sidebar widgets terdaftar (Popular Posts, Labels, dll)
- [ ] Posting terlihat dengan formatting yang benar
- [ ] Warna mengikuti palet government-futuristic (navy blue, gold, teal)
- [ ] Mobile view responsive dan tidak berantakan
- [ ] Search/Navigation berfungsi normal

---

## 🎨 Konfigurasi Awal (Setelah Instalasi)

### 1. Update Blog Title & Description
- Dashboard → **Settings** → **Basic**
- Update judul dan deskripsi blog
- Klik **Save Settings**

### 2. Upload Logo/Header Image (Opsional)
- Dashboard → **Theme** → **Customize**
- Cari bagian **Header Image**
- Upload logo atau banner Anda

### 3. Tambah Widget Penting
- Dashboard → **Layout**
- Tambahkan widget: About Me, Popular Posts, Labels
- Atur posisi dan judul widget
- Klik **Save Arrangement**

### 4. Kustomisasi Warna (Opsional)
- Dashboard → **Theme** → **Edit HTML**
- Cari bagian CSS `:root` variables
- Ubah nilai `--primary`, `--gold`, dll sesuai keinginan
- Klik **Save Theme**

---

## 📱 Test di Multiple Devices

### Desktop
- [ ] Chrome
- [ ] Firefox
- [ ] Safari
- [ ] Edge

### Mobile
- [ ] iOS Safari
- [ ] Android Chrome
- [ ] Android Firefox

### Testing Tools
- Google Mobile-Friendly Test: [test.webpagetest.org](https://test.webpagetest.org)
- Google PageSpeed Insights: [pagespeed.web.dev](https://pagespeed.web.dev)

---

## 🚨 Rollback (Kembalikan ke Theme Lama)

Jika ada masalah dengan theme baru:

1. Dashboard → **Theme** → **⋮** → **Backup/Restore**
2. Klik **Restore**
3. Pilih backup theme lama dari daftar
4. Klik **Restore this version**
5. Tunggu proses selesai

---

## 📞 Bantuan & Support

Jika masih ada masalah:

1. **Baca FAQ**: [docs/TROUBLESHOOTING.md](./docs/TROUBLESHOOTING.md)
2. **Lihat Customization Guide**: [CUSTOMIZATION.md](./CUSTOMIZATION.md)
3. **Hubungi Support**: contact@catatanguruips.com
4. **GitHub Issues**: [github.com/guruips/issues](https://github.com/guruips/Blogger-Theme-V5-Government-Futuristic/issues)

---

**Selamat! Theme berhasil diinstal.** 🎉