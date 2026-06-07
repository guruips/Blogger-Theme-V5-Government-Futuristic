# 📐 Penjelasan Struktur XML

## Anatomis File Blogger XML

```xml
<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html xmlns="..." xmlns:b="..." xmlns:data="...">
  <head>
    <!-- Meta Tags, Stylesheets, Scripts -->
  </head>
  <body>
    <!-- Content Sections -->
  </body>
</html>
```

---

## Meta Tags & SEO

### Meta Dasar
```xml
<meta charset='UTF-8'/>
<meta content='width=device-width, initial-scale=1.0' name='viewport'/>
<meta content='IE=edge' http-equiv='X-UA-Compatible'/>
<meta content='index, follow, max-snippet:-1, max-image-preview:large, max-video-preview:-1' name='robots'/>
```

### Open Graph (Social Media)
```xml
<meta content='article' property='og:type'/>
<meta expr:content='data:post.title' property='og:title'/>
<meta expr:content='data:post.snippet' property='og:description'/>
<meta expr:content='data:post.featuredImage.url' property='og:image'/>
```

### Twitter Cards
```xml
<meta content='summary_large_image' name='twitter:card'/>
<meta content='@kangtoer' name='twitter:site'/>
```

### Article Metadata
```xml
<meta expr:content='data:post.date' property='article:published_time'/>
<meta expr:content='data:post.author.name' property='article:author'/>
<meta expr:content='data:label.name' property='article:tag'/>
```

---

## Blogger Namespaces

### Namespace Declarations
```xml
<html 
  xmlns='http://www.w3.org/1999/xhtml'           <!-- Standard XHTML -->
  xmlns:b='http://www.google.com/blogger/2006/gadgets'  <!-- Blogger widgets -->
  xmlns:data='http://www.google.com/bloggerux/data/1.0'  <!-- Data access -->
  xmlns:expr='http://www.google.com/bloggerux/expr/1.0'  <!-- Expression evaluation -->
>
```

---

## Blogger Tags Penting

### Conditional Tags
```xml
<b:if cond='condition'>
  <!-- Content if true -->
<b:elseif cond='other_condition'/>
  <!-- Content if elseif true -->
<b:else/>
  <!-- Content if all false -->
</b:if>
```

### Loop Tags
```xml
<b:loop values='data:posts' var='post'>
  <!-- Repeat untuk setiap post -->
  <data:post.title/>
</b:loop>
```

### Section Tags (Widget Area)
```xml
<b:section class='main' id='main'>
  <b:widget id='Blog1' locked='true' title='Blog Posts' type='Blog'/>
</b:section>
```

---

## Data Variables

### Blog Data
```
data:blog.title                    - Judul blog
data:blog.metaDescription          - Deskripsi blog
data:blog.canonicalUrl             - URL canonical
data:blog.languageDirection        - Arah bahasa (LTR/RTL)
```

### Post Data
```
data:post.title                    - Judul post
data:post.snippet                  - Ringkasan post
data:post.body                     - Isi post
data:post.url                      - URL post
data:post.date                     - Tanggal posting
data:post.author.name              - Nama author
data:post.labels                   - Labels/kategori
data:post.featuredImage.url        - Featured image
data:post.firstImageUrl            - Gambar pertama
```

### View Data
```
data:view.isPost                   - Apakah halaman post
data:view.isPage                   - Apakah halaman page
data:view.isBlogPost               - Apakah halaman list posts
data:view.url                      - URL halaman saat ini
```

---

## CSS Variables (Custom Properties)

```css
:root {
  /* Primary Colors */
  --primary: #1565C0;
  --primary-light: #1E88E5;
  --primary-darker: #0D47A1;
  
  /* Backgrounds */
  --bg-body: #F5F7FA;
  --bg-primary: #FFFFFF;
  
  /* Text */
  --text-primary: #1A202C;
  --text-secondary: #4A5568;
  
  /* Others */
  --border: #E2E8F0;
  --shadow-md: 0 4px 16px rgba(0,0,0,0.08);
}
```

---

## Struktur Layout

### Header Section
```xml
<b:section class='header' id='header'>
  <b:widget id='Header1' type='Header'/>
</b:section>
```

### Main Content Section
```xml
<b:section class='main' id='main'>
  <b:widget id='Blog1' type='Blog'/>
</b:section>
```

### Sidebar Section
```xml
<b:section class='sidebar' id='sidebar'>
  <b:widget id='PopularPosts1' type='PopularPosts'/>
  <b:widget id='Labels1' type='Labels'/>
</b:section>
```

### Footer Section
```xml
<b:section class='footer' id='footer'>
  <b:widget id='Attribution1' type='Attribution'/>
</b:section>
```

---

## Widget Types

### Content Widgets
```
Blog              - Menampilkan blog posts
PageList          - Daftar halaman statis
Archive           - Daftar archive posting
Labels            - Daftar label/kategori
PopularPosts      - Post paling populer
RecentPosts       - Post terbaru
```

### Custom Widgets
```
HTML              - Custom HTML/JavaScript
Text              - Text content
Image             - Gambar
Video             - Video embeds
```

### Standard Widgets
```
Header            - Header blog
Profile           - Profil author
Followers         - Followers widget
Attribution       - Blogger attribution
```

---

## Expression Language (EL)

### Basic Syntax
```xml
<expr:text expr='expression'/>
<expr:attr name='attribute' binding='expression'/>
<expr:attr name='style' binding='"background: " + data:color'>
```

### String Concatenation
```xml
<expr:text expr='data:post.title + " by " + data:post.author.name'/>
```

### Conditional in Attributes
```xml
<expr:attr name='class' binding='data:isHome ? "active" : ""'/>
```

---

## Responsive Media Queries

```css
/* Desktop (default) */
body { /* desktop styles */ }

/* Tablet */
@media (max-width: 1024px) {
  body { /* tablet styles */ }
}

/* Mobile */
@media (max-width: 768px) {
  body { /* mobile styles */ }
}

/* Small Mobile */
@media (max-width: 480px) {
  body { /* small mobile styles */ }
}
```

---

## Best Practices

1. **Selalu gunakan `expr:`** untuk dynamic content
2. **Gunakan CSS variables** untuk warna & sizing
3. **Mobile-first approach** di media queries
4. **Optimize gambar** untuk faster loading
5. **Valid XHTML** - follow Blogger XML standards
6. **Accessible markup** - semantic HTML
7. **SEO-friendly** - proper meta tags
8. **Performance** - minimize render-blocking resources

---

## Debugging Tips

1. **Gunakan Blogger Dashboard Preview**
2. **Check Browser DevTools** (F12)
3. **Validate XML** di xmlvalidation.com
4. **Test berbagai devices**
5. **Check Console** untuk JavaScript errors
6. **Clear cache** browser sebelum test

---

**Referensi lengkap struktur Blogger XML theme** 📐