# Özelleştirme Rehberi

## 📝 Değiştirmeniz Gereken Yerler

### 1. index.html - Temel Bilgiler

#### Sayfa Başlığı (Satır 6)
```html
<title>Dr. [Adınız] - Akademik Profil</title>
```
→ `<title>Dr. Ahmet Yılmaz - Akademik Profil</title>`

#### Navigasyon Logo (Satır 16)
```html
<a href="#home" class="nav-logo">Dr. [Adınız Soyadınız]</a>
```
→ `<a href="#home" class="nav-logo">Dr. Ahmet Yılmaz</a>`

#### Hero Bölümü (Satır 30-50)
```html
<span class="hero-label">Mühendislik Fakültesi</span>
```
→ Kendi fakültenizi yazın

```html
<h1 class="hero-title">
    <span class="title-line">İnovasyon ve</span>
    <span class="title-line">Teknoloji</span>
</h1>
```
→ Kendi sloganınız veya araştırma odağınız

```html
<p class="hero-description">
    [Alan] alanında araştırma...
</p>
```
→ Kendinizi tanıtan 2-3 cümle

#### Profil Bilgileri (Satır 70-100)
```html
<h3>Dr. [Adınız Soyadınız]</h3>
<p class="profile-title">[Unvanınız]</p>
<p class="profile-dept">[Bölüm Adı]<br>[Üniversite Adı]</p>
```

#### İletişim (Satır 102-120)
```html
<a href="mailto:email@university.edu" class="contact-item">
    ...
    email@university.edu
</a>
```
→ Gerçek e-posta adresiniz

LinkedIn, GitHub, Google Scholar linklerinizi ekleyin

#### Biyografi (Satır 130-145)
İki paragraf şeklinde kendinizi tanıtın:
- Akademik geçmiş
- Araştırma ilgi alanları
- Mevcut projeler

#### Uzmanlık Alanları (Satır 150-160)
```html
<span class="tag">Makine Öğrenmesi</span>
<span class="tag">Yapay Zeka</span>
```
→ Kendi alanlarınızı ekleyin (5-8 adet)

#### Eğitim Bilgileri (Satır 170-200)
Her derece için:
```html
<div class="timeline-item">
    <span class="year">2020</span>
    <div class="timeline-content">
        <strong>Doktora</strong>
        <p>[Bölüm], [Üniversite]</p>
    </div>
</div>
```

#### Araştırmalar (Satır 230+)
Her yayın için kopyalayıp düzenleyin:
```html
<article class="research-card" data-category="journal">
    <div class="research-meta">
        <span class="research-type">Dergi Makalesi</span>
        <span class="research-year">2024</span>
    </div>
    <h3 class="research-title">Makale Başlığı</h3>
    <p class="research-authors">
        <strong>Soyadınız, A.</strong>, Yazar, B.
    </p>
    <p class="research-journal">
        <em>Journal Name</em>, Vol. XX
    </p>
    <div class="research-links">
        <a href="files/paper.pdf" class="research-link">PDF</a>
        <a href="https://doi.org/..." class="research-link">DOI</a>
    </div>
</article>
```

`data-category` değerleri:
- `journal` - Dergi makaleleri
- `conference` - Konferans bildirileri  
- `project` - Projeler

#### Dersler (Satır 330+)
```html
<div class="course-card">
    <div class="course-header">
        <h3>MUH301: Ders Adı</h3>
        <span class="semester">Güz 2024</span>
    </div>
    <p class="course-description">
        Ders açıklaması...
    </p>
    <div class="course-meta">
        <span class="course-level">Lisans</span>
        <span class="course-credits">3 Kredi</span>
    </div>
    <a href="files/syllabus.pdf" class="course-link">Ders Materyalleri →</a>
</div>
```

#### Danışmanlık İstatistikleri (Satır 380)
```html
<div class="stat-item">
    <span class="stat-number">5</span>
    <span class="stat-label">Doktora Öğrencisi</span>
</div>
```
→ Gerçek sayılarınızı girin

#### Blog Kartları (Satır 420+)
```html
<article class="blog-card">
    <div class="blog-image">
        <img src="images/blog-1.jpg" alt="Blog görseli">
        <span class="blog-category">Araştırma</span>
    </div>
    <div class="blog-content">
        <time class="blog-date">15 Ocak 2024</time>
        <h3 class="blog-title">Blog Başlığı</h3>
        <p class="blog-excerpt">Kısa özet...</p>
        <a href="blog/post-1.html" class="blog-link">Devamını Oku →</a>
    </div>
</article>
```

#### Google Calendar (Satır 450)
```html
<iframe src="https://calendar.google.com/calendar/appointments/schedules/AcZssZ2KrMnz6mwwTubFqBZMRJ-WlZIaJHsXgzU8cPz7KVLkdqjRvzJt_9B8_6aljDsEb0VcpNskiWX_?gv=true"
```
→ Kendi Google Calendar randevu URL'inizi kullanın

#### Footer (Satır 480+)
Tüm bilgileri, linkleri ve sosyal medya adreslerini güncelleyin

---

### 2. style.css - Tasarım Değişiklikleri

#### Renk Paleti (Satır 1-15)
```css
:root {
    --color-primary: #0a0a0a;      /* Ana renk (siyah) */
    --color-accent: #4a90e2;        /* Vurgu rengi (mavi) */
    --color-accent-dark: #2563eb;   /* Koyu vurgu */
}
```

Popüler renk önerileri:
- Mavi: `#4a90e2`, `#2563eb`
- Yeşil: `#10b981`, `#059669`
- Mor: `#8b5cf6`, `#7c3aed`
- Turuncu: `#f59e0b`, `#d97706`
- Kırmızı: `#ef4444`, `#dc2626`

#### Font Değiştirme (Satır 18-20)
Başka fontlar için Google Fonts'u ziyaret edin:
https://fonts.google.com

Örnek alternatifler:
```css
/* Klasik & Akademik */
--font-display: 'Playfair Display', serif;
--font-body: 'Source Serif Pro', serif;

/* Modern & Minimal */
--font-display: 'Manrope', sans-serif;
--font-body: 'Inter', sans-serif;

/* Teknik & Profesyonel */
--font-display: 'IBM Plex Sans', sans-serif;
--font-body: 'IBM Plex Sans', sans-serif;
```

Font linkini `index.html` head bölümünde değiştirmeyi unutmayın!

---

### 3. _config.yml - Site Ayarları

```yaml
title: Dr. Ahmet Yılmaz
description: Bilgisayar Mühendisliği - Araştırma ve Öğretim
author: Dr. Ahmet Yılmaz
email: ayilmaz@university.edu

social:
  linkedin: ahmet-yilmaz
  github: ahmetyilmaz
  twitter: drahmetyilmaz
  scholar: abc123xyz
```

---

### 4. Dosya Yapısı

```
website/
├── index.html              # Ana sayfa
├── style.css               # Stiller
├── script.js               # JavaScript
├── README.md               # Dokümantasyon
├── QUICKSTART.md          # Hızlı başlangıç
├── _config.yml            # GitHub Pages config
├── .gitignore             # Git ignore
│
├── images/                # Görseller
│   ├── profile.jpg        # 400x400px profil fotoğrafı
│   ├── blog-1.jpg         # 800x600px blog görseli
│   ├── blog-2.jpg
│   └── blog-3.jpg
│
├── files/                 # İndirilebilir dosyalar
│   ├── cv.pdf            # CV'niz
│   └── syllabus.pdf      # Ders programları
│
└── blog/                  # Blog yazıları
    ├── post-template.html # Şablon
    ├── post-1.html       # İlk yazı
    └── post-2.html       # İkinci yazı
```

---

## 🎨 Tasarım Önerileri

### Minimalist Tema
```css
--color-primary: #1a1a1a;
--color-accent: #666666;
--color-bg: #ffffff;
```

### Mavi Tonlar (Teknoloji)
```css
--color-primary: #0f172a;
--color-accent: #3b82f6;
--color-bg: #f8fafc;
```

### Yeşil Tonlar (Çevre/Bio)
```css
--color-primary: #14532d;
--color-accent: #10b981;
--color-bg: #f0fdf4;
```

### Mor Tonlar (Sanat/Sosyal)
```css
--color-primary: #581c87;
--color-accent: #a855f7;
--color-bg: #faf5ff;
```

---

## 📸 Görsel Boyutları

- **Profil fotoğrafı**: 400x400px (kare)
- **Blog görselleri**: 1200x630px (16:9)
- **Dosya boyutu**: Her görsel < 500KB

---

## ✅ Yayınlamadan Önce Kontrol Listesi

- [ ] Tüm `[...]` placeholder'ları değiştirildi
- [ ] E-posta adresleri güncellendi
- [ ] Sosyal medya linkleri eklendi
- [ ] Profil fotoğrafı yüklendi
- [ ] En az 1 yayın bilgisi eklendi
- [ ] En az 1 ders bilgisi eklendi
- [ ] Google Calendar linki güncellendi
- [ ] CV dosyası yüklendi
- [ ] Renk paleti seçildi
- [ ] Tüm dosyalar GitHub'a yüklendi
- [ ] GitHub Pages aktifleştirildi
- [ ] Site canlıda test edildi

---

## 🆘 Sorun mu Yaşıyorsunuz?

### Site açılmıyor
1. Repository adı `kullaniciadi.github.io` mi?
2. Settings → Pages → Source: main/(root) seçili mi?
3. 5 dakika beklediniz mi?

### Görseller görünmüyor
1. Dosya adları doğru mu? (büyük/küçük harf)
2. `images/` klasöründe mi?
3. Tarayıcı önbelleğini temizleyin (Ctrl+F5)

### Mobilde bozuk
1. Tüm dosyalar yüklendi mi?
2. `style.css` ve `script.js` yüklenmiş mi?
3. Konsol hatalarını kontrol edin (F12)

---

**Başarılar! 🎉**
