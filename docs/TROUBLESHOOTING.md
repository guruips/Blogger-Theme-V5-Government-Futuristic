# 🔧 FAQ & Troubleshooting

## Instalasi

### Q: Kode XML tidak bisa di-paste di Blogger
A:
- Gunakan browser Chrome, Firefox, atau Safari
- Jangan gunakan IE 11 atau browser lawas
- Disable extensions yang mungkin mengganggu
- Clear cache browser (Ctrl+Shift+Delete)
- Copy paste ulang dengan hati-hati

### Q: Error "XML Parsing Error" saat save
A:
- Kemungkinan ada karakter special yang rusak
- Download ulang file XML yang bersih
- Gunakan Notepad++ untuk edit (bukan Word/Pages)
- Pastikan encoding adalah UTF-8
- Jangan hapus tag HTML pembuka/penutup

### Q: Save theme tapi halaman tetap blank
A:
- Refresh halaman (Ctrl+F5)
- Tunggu 5-10 menit untuk full propagation
- Buka blog di tab/browser baru
- Check di halaman berbeda (home, archive, post)
- Coba logout dan login kembali

---

## Display & Styling

### Q: Tema tidak tampil dengan benar di mobile
A:
- Pastikan meta viewport tag ada: `<meta content='width=device-width' name='viewport'/>`
- Clear browser cache: Ctrl+Shift+Delete
- Test di browser mobile yang berbeda
- Check media queries di CSS
- Zoom out browser untuk lihat full layout

### Q: Warna tidak berubah setelah edit CSS
A:
- Pastikan mengubah di tempat yang benar (`:root` section)
- Save theme setelah edit
- Clear cache browser: Ctrl+Shift+Delete
- Refresh page: Ctrl+F5 (hard refresh)
- Tunggu 5 menit untuk propagation
- Buka di browser/tab baru

### Q: Font tidak berubah
A:
- Pastikan URL Google Fonts valid
- Check `<link>` tag di `<head>`
- Update nama font di CSS `font-family`
- Clear cache dan refresh
- Pilih font weights yang benar (400, 700, dll)

### Q: Widget tidak muncul di sidebar
A:
- Dashboard → **Layout** → check widgets listed
- Klik "Add widget" untuk menambah
- Pastikan widget tidak tersembunyi
- Check bagian `<b:section>` di XML
- Refresh halaman layout
- Save arrangement

---

## Performance

### Q: Blog lambat loading
A:
- Optimize gambar (compress ukuran)
- Minify CSS & JavaScript
- Enable browser caching
- Reduce external resources
- Use CDN untuk media files
- Check PageSpeed Insights: pagespeed.web.dev

### Q: Banyak unused CSS
A:
- Remove unused styles dari `<b:skin>`
- Use Critical CSS tools
- Lazy load images
- Defer non-critical JavaScript
- Use CSS-in-JS untuk component styles

---

## SEO

### Q: Meta tags tidak terdeteksi
A:
- Pastikan conditional tags (`b:if`) benar
- Check `expr:` attributes valid
- Validate di Google Search Console
- Test dengan Google's Rich Results Test
- Wait 24-48 jam untuk Google crawl

### Q: Open Graph tidak work di social media
A:
- Pastikan meta tags ada di `<head>`
- Use Social Media Debugger tools
- Check featured image URL valid
- Wait untuk social platform cache refresh
- Test di Facebook/LinkedIn debugger tools

---

## Dark/Light Mode

### Q: Dark mode tidak toggle
A:
- Check JavaScript untuk toggle function
- localStorage mungkin disabled
- Buka DevTools → Application → localStorage
- Pastikan CSS variables di-support browser
- Test di browser modern (Chrome, Firefox, Safari)

### Q: Dark mode mengacaukan warna
A:
- Add `@media (prefers-color-scheme: dark)` rules
- Test contrast ratios untuk accessibility
- Use CSS custom properties untuk dark colors
- Test di macOS dark mode & Windows dark mode

---

## Mobile Optimization

### Q: Menu hamburger tidak work
A:
- Check JavaScript event listeners
- Test di mobile device (bukan just resize desktop)
- Enable mobile-specific CSS
- Check touch event handlers
- Verify viewport meta tag

### Q: Konten terpotong di mobile
A:
- Check `max-width` di container
- Ensure padding/margin cocok untuk mobile
- Test di berbagai screen sizes
- Use responsive units (%, vw, em)
- Don't use fixed widths

### Q: Font terlalu kecil/besar di mobile
A:
- Adjust font-size di media queries
- Use rem units (relative to root)
- Test readability di actual device
- Follow WCAG minimum 16px untuk body text
- Add font scaling di `<head>`: `-webkit-text-size-adjust: 100%`

---

## Browser Compatibility

### Q: Tidak work di IE 11
A:
- IE 11 limited support untuk CSS Grid/Flexbox
- Use fallback styles
- Add vendor prefixes (-ms-, -webkit-)
- Test di Edge (newer version)
- Consider dropping IE 11 support

### Q: Tidak work di Safari
A:
- Check `-webkit-` vendor prefixes
- Test backdrop-filter property
- Verify CSS custom properties support
- Use `-webkit-appearance` untuk form elements
- Test di actual Safari (bukan just Chrome)

---

## Backup & Recovery

### Q: Bagaimana rollback ke theme lama?
A:
1. Dashboard → **Theme** → **⋮** → **Backup/Restore**
2. Klik **Restore**
3. Pilih tema dari list
4. Klik **Restore this version**
5. Tunggu proses selesai

### Q: Mau export theme current?
A:
1. Dashboard → **Theme** → **⋮** → **Backup/Restore**
2. Klik **Download tema lengkap**
3. File XML akan di-download
4. Save untuk reference/sharing

---

## Advanced Issues

### Q: Post template tidak render dengan benar
A:
- Check `data:post` variables valid
- Verify `expr:` expressions syntax
- Test di single post page
- Check browser console untuk errors
- Validate XML structure

### Q: Custom JavaScript tidak execute
A:
- Add script di akhir `</body>`
- Check script async/defer attributes
- Verify no syntax errors
- Test di browser console
- Use Blogger's `<b:include>` jika perlu

### Q: AJAX search tidak work
A:
- Check API endpoints
- Verify CORS headers
- Test di browser console
- Check network tab untuk requests
- Ensure jQuery/vanilla JS loaded

---

## Contact & Support

### Jika masalah tidak teratasi:

1. **GitHub Issues**
   - https://github.com/guruips/Blogger-Theme-V5-Government-Futuristic/issues
   - Berikan detail lengkap tentang masalah
   - Sertakan screenshots/video

2. **Email Support**
   - contact@catatanguruips.com
   - Describe issue dengan detail
   - Include browser/device info

3. **Community Forum**
   - Blogger official forum: https://support.google.com/blogger
   - Stack Overflow: tag `blogger` & `blogger-template`

---

## Common Error Messages

### "XML Parsing Error: no element found"
- Kemungkinan ada tag HTML yang tidak closed
- Check opening/closing tags balance
- Remove extra/invalid characters

### "The gadget with id=X is not defined"
- Widget ID mungkin duplicate
- Rename widget IDs unique
- Clear browser cache

### "Your template has errors: The HTML is not valid"
- Validate XML di xmlvalidation.com
- Check closing tags
- Ensure proper nesting

---

**Semoga FAQ ini membantu! Jika ada pertanyaan lain, silakan hubungi support.** 💡