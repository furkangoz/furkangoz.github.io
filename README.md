# Akademik Web Sitesi

Minimalist ve modern tasarıma sahip, profesyonel akademik web sitesi. GitHub Pages üzerinde yayınlanmak üzere tasarlanmıştır.

## 🎨 Özellikler

- **Responsive Tasarım**: Tüm cihazlarda mükemmel görünüm
- **Modern & Minimalist**: Temiz, profesyonel estetik
- **Hızlı Yükleme**: Optimize edilmiş performans
- **SEO Dostu**: Arama motorları için optimize edilmiş
- **Kolay Özelleştirme**: Basit HTML/CSS/JS yapısı

## 📋 Bölümler

1. **Ana Sayfa (Hero)**: Etkileyici karşılama bölümü
2. **Hakkımda**: Profil, CV, uzmanlık alanları
3. **Araştırmalar**: Yayınlar, makaleler, projeler
4. **Dersler**: Verdiğiniz dersler ve öğrenci danışmanlığı
5. **Blog**: Makaleler ve düşünceler
6. **Randevu**: Google Calendar entegrasyonu

## 🚀 Kurulum

### 1. GitHub Repository Oluşturma

```bash
# Yeni repository oluşturun (GitHub'da)
# Repository adı: kullaniciadi.github.io

# Yerel bilgisayarınızda
git init
git add .
git commit -m "İlk commit"
git branch -M main
git remote add origin https://github.com/kullaniciadi/kullaniciadi.github.io.git
git push -u origin main
```

### 2. GitHub Pages Aktifleştirme

1. Repository → Settings → Pages
2. Source: Deploy from a branch
3. Branch: main / (root)
4. Save

Web siteniz 2-3 dakika içinde `https://kullaniciadi.github.io` adresinde yayında olacak!

## ✏️ Özelleştirme

### Temel Bilgileri Değiştirme

**index.html** dosyasında şu yerleri güncelleyin:

```html
<!-- Adınızı değiştirin -->
<title>Dr. [Adınız] - Akademik Profil</title>
<a href="#home" class="nav-logo">Dr. [Adınız Soyadınız]</a>

<!-- Hero bölümünü düzenleyin -->
<span class="hero-label">Mühendislik Fakültesi</span>
<p class="hero-description">...</p>

<!-- İletişim bilgilerinizi ekleyin -->
<a href="mailto:email@university.edu" class="contact-item">
```

### Renkleri Değiştirme

**style.css** dosyasının başındaki CSS değişkenlerini düzenleyin:

```css
:root {
    --color-primary: #0a0a0a;      /* Ana renk */
    --color-accent: #4a90e2;        /* Vurgu rengi */
    --color-accent-dark: #2563eb;   /* Koyu vurgu */
    /* ... */
}
```

### Fotoğraf Ekleme

```bash
# images klasörü oluşturun
mkdir images

# Fotoğraflarınızı ekleyin:
images/
  ├── profile.jpg          # Profil fotoğrafı (önerilen: 400x400px)
  ├── blog-1.jpg           # Blog görselleri (önerilen: 800x600px)
  ├── blog-2.jpg
  └── blog-3.jpg
```

### Araştırmalar Ekleme

`index.html` içinde araştırma kartlarını kopyalayıp düzenleyin:

```html
<article class="research-card" data-category="journal">
    <div class="research-meta">
        <span class="research-type">Dergi Makalesi</span>
        <span class="research-year">2024</span>
    </div>
    <h3 class="research-title">Makale Başlığınız</h3>
    <p class="research-authors">
        <strong>Soyadınız, A.</strong>, Yazar, B.
    </p>
    <p class="research-journal">
        <em>Journal Name</em>, Vol. XX
    </p>
    <div class="research-links">
        <a href="paper.pdf" class="research-link">PDF</a>
        <a href="https://doi.org/..." class="research-link">DOI</a>
    </div>
</article>
```

### Blog Yazısı Ekleme

1. `blog` klasörü oluşturun
2. Her yazı için HTML dosyası oluşturun (örn: `blog/post-1.html`)
3. Ana sayfada blog kartını güncelleyin

## 📁 Dosya Yapısı

```
akademik-web-sitesi/
├── index.html           # Ana sayfa
├── style.css            # Stil dosyası
├── script.js            # JavaScript
├── README.md           # Bu dosya
├── images/             # Görseller
│   ├── profile.jpg
│   └── blog-*.jpg
├── files/              # İndirilebilir dosyalar
│   └── cv.pdf
└── blog/               # Blog yazıları
    ├── post-1.html
    └── post-2.html
```

## 🎯 İpuçları

### SEO Optimizasyonu

`index.html` head bölümüne ekleyin:

```html
<meta name="description" content="Dr. [Adınız] - [Alan] alanında araştırma ve öğretim">
<meta name="keywords" content="akademik, araştırma, [alanınız], [üniversite]">
<meta name="author" content="Dr. [Adınız Soyadınız]">
```

### Google Analytics (Opsiyonel)

```html
<!-- index.html head bölümüne ekleyin -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### CV Ekleme

1. CV'nizi PDF olarak kaydedin
2. `files/cv.pdf` olarak ekleyin
3. Link zaten mevcut: `<a href="files/cv.pdf" download>`

### Sosyal Medya Linkleri

Footer'da sosyal medya linklerini güncelleyin:

```html
<a href="https://linkedin.com/in/kullaniciadi">LinkedIn</a>
<a href="https://github.com/kullaniciadi">GitHub</a>
<a href="https://twitter.com/kullaniciadi">Twitter</a>
```

## 🔧 Teknik Detaylar

- **Framework**: Vanilla HTML/CSS/JS (bağımlılık yok)
- **Fontlar**: Google Fonts (Crimson Pro, JetBrains Mono)
- **Renk Paleti**: Minimalist siyah-beyaz-mavi
- **Responsive**: Mobile-first yaklaşım
- **Tarayıcı Desteği**: Modern tarayıcılar (Chrome, Firefox, Safari, Edge)

## 📱 Responsive Breakpoints

- Desktop: 1024px+
- Tablet: 768px - 1023px
- Mobile: < 768px

## 🎨 Renk Paleti

- **Primary**: #0a0a0a (Siyah)
- **Secondary**: #2d2d2d (Koyu Gri)
- **Accent**: #4a90e2 (Mavi)
- **Background**: #ffffff (Beyaz)
- **Alt Background**: #f8f9fa (Açık Gri)

## 🚀 Performans

- Hafif dosyalar (< 100KB toplam CSS/JS)
- Lazy loading görseller
- Optimize edilmiş animasyonlar
- Hızlı yükleme süreleri

## 📞 Destek

Sorularınız için:
- GitHub Issues açabilirsiniz
- E-posta: [email@domain.com]

## 📄 Lisans

Bu proje kişisel kullanım için ücretsizdir.

## ✨ Güncellemeler

### v1.0 (2024)
- ✅ İlk sürüm
- ✅ Responsive tasarım
- ✅ Google Calendar entegrasyonu
- ✅ Blog sistemi
- ✅ Araştırma filtreleme

---

**Not**: Tüm placeholder içerikleri kendi bilgilerinizle değiştirmeyi unutmayın!
