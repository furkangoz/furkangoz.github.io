# Hızlı Başlangıç Kılavuzu

## 5 Dakikada GitHub Pages'e Yükleyin

### Adım 1: Dosyaları İndirin
Bu klasördeki tüm dosyaları bilgisayarınıza indirin.

### Adım 2: Kişiselleştirin
En az şu dosyaları düzenleyin:

**index.html**
- Satır 6: `<title>Dr. [Adınız] - Akademik Profil</title>`
- Satır 16: `<a href="#home" class="nav-logo">Dr. [Adınız Soyadınız]</a>`
- Satır 35-50: Hero bölümündeki tüm metinleri
- Satır 70-150: Hakkımda bölümü
- Satır 102-110: İletişim bilgileri
- Satır 160+: Araştırmalar, dersler, blog kartları

**_config.yml**
- Satır 4-7: Tüm bilgileri güncelleyin

### Adım 3: Görseller Ekleyin
`images/` klasörüne:
- `profile.jpg` - Profil fotoğrafınız (400x400px önerilir)
- `blog-1.jpg`, `blog-2.jpg`, `blog-3.jpg` - Blog görselleri

### Adım 4: GitHub'a Yükleyin

#### 4a. GitHub Desktop ile (Kolay)
1. GitHub Desktop'ı indirin: https://desktop.github.com
2. File → New Repository
3. Name: `kullaniciadi.github.io` (kullanıcı adınızla)
4. Local Path: Bu dosyaların olduğu klasör
5. Create Repository
6. Publish Repository (Public olarak işaretleyin)

#### 4b. Komut satırı ile
```bash
cd /projenizin/yolu
git init
git add .
git commit -m "İlk commit: Akademik web sitesi"
git branch -M main
git remote add origin https://github.com/kullaniciadi/kullaniciadi.github.io.git
git push -u origin main
```

### Adım 5: GitHub Pages'i Aktifleştirin
1. GitHub'da repository'nize gidin
2. Settings → Pages
3. Source: "Deploy from a branch"
4. Branch: "main" / "(root)"
5. Save

### Adım 6: Bekleyin ve Ziyaret Edin
2-3 dakika sonra siteniz hazır!
Adres: `https://kullaniciadi.github.io`

## Hızlı Özelleştirme İpuçları

### Renkleri Değiştirme
`style.css` dosyasının başındaki `:root` bölümünde:
```css
--color-accent: #4a90e2;  /* Mavi yerine istediğiniz renk */
```

### Google Calendar'ı Değiştirme
`index.html` satır 450'deki iframe URL'ini kendi randevu bağlantınızla değiştirin.

### Yeni Blog Yazısı Ekleme
1. `blog/post-template.html` dosyasını kopyalayın
2. `blog/post-2.html` olarak kaydedin
3. İçeriği düzenleyin
4. `index.html`'de blog kartı ekleyin

## Sorun Giderme

### Site görünmüyor
- Repository adının `kullaniciadi.github.io` olduğundan emin olun
- Settings → Pages'de "Deploy from a branch" seçili olmalı
- 5 dakika bekleyin

### Görseller görünmüyor
- Dosya adlarının doğru olduğundan emin olun (büyük/küçük harf)
- Görsellerin `images/` klasöründe olduğunu kontrol edin

### Mobilde bozuk görünüyor
- Tüm dosyaları doğru yüklediğinizden emin olun
- Tarayıcı önbelleğini temizleyin

## Gelişmiş Özelleştirme

### Custom Domain Kullanma
1. Domain sağlayıcınızda CNAME kaydı oluşturun
2. GitHub Settings → Pages → Custom domain
3. Domain adınızı girin (örn: `www.sitenim.com`)

### Google Analytics Ekleme
`index.html` head bölümüne Google Analytics kodunu ekleyin.

### SEO İyileştirme
- Meta description ekleyin
- Alt text'leri tüm görsellere ekleyin
- Sitemap oluşturun

## Güncelleme Yapma

Değişiklik yaptıktan sonra:
```bash
git add .
git commit -m "Güncelleme açıklaması"
git push
```

2-3 dakika içinde değişiklikler yayında!

---

**Yardıma mı ihtiyacınız var?**
GitHub Issues'da soru sorabilirsiniz veya
README.md dosyasındaki detaylı kılavuzu okuyun.
