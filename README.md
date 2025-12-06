# NanoCam Website

NanoCam - Kameralar va tarmoq qurilmalari do'koni uchun landing page.

## 🚀 GitHub Pages'ga joylashtirish

### 1-qadam: Repository yaratish
```bash
# Yangi repository yarating: nanocam.github.io yoki nanocam-website
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/nanocam-website.git
git push -u origin main
```

### 2-qadam: GitHub Pages'ni yoqish
1. GitHub'da repository'ga kiring
2. **Settings** → **Pages** bo'limiga o'ting
3. **Source** bo'limida `main` branch va `/ (root)` tanlang
4. **Save** bosing

### 3-qadam: nanocam.uz domenni ulash

#### GitHub'da:
1. **Settings** → **Pages** → **Custom domain**
2. `nanocam.uz` kiriting va **Save** bosing

#### Domen provayderingizda (DNS sozlamalari):

**A records qo'shing:**
```
Type: A
Name: @
Value: 185.199.108.153

Type: A
Name: @
Value: 185.199.109.153

Type: A
Name: @
Value: 185.199.110.153

Type: A
Name: @
Value: 185.199.111.153
```

**CNAME record (www uchun):**
```
Type: CNAME
Name: www
Value: YOUR_USERNAME.github.io
```

#### HTTPS yoqish:
DNS tarqalganidan keyin (24-48 soat), GitHub Pages'da **Enforce HTTPS** ni belgilang.

## 📁 Kerakli rasmlar

`images/` papkasiga quyidagi rasmlarni qo'shing:

| Fayl nomi | O'lcham | Tavsif |
|-----------|---------|--------|
| `logo.png` | 100x100 px | App logosi |
| `favicon.png` | 32x32 px | Brauzer ikonkasi |
| `app-mockup.png` | 350x700 px | Telefon mockup rasmi |
| `og-image.png` | 1200x630 px | Social media uchun rasm |

## 🎨 Ranglar

```css
--primary: #1E3A5F;      /* Asosiy ko'k */
--accent: #4CAF50;       /* Yashil accent */
--background: #F8FAFC;   /* Fon */
```

## 📱 App Store va Google Play linklari

`index.html` faylida quyidagi joylarni o'zgartiring:

```html
<!-- App Store link -->
<a href="https://apps.apple.com/app/nanocam/id..." class="store-btn">

<!-- Google Play link -->
<a href="https://play.google.com/store/apps/details?id=dev.nanocam.nanocam" class="store-btn">
```

## 📞 Aloqa formasi

Hozircha forma `alert()` ko'rsatadi. Quyidagi variantlarni qo'shish mumkin:

1. **Telegram Bot** - Formani Telegram'ga yuborish
2. **Formspree** - Bepul form backend
3. **EmailJS** - Email orqali yuborish
4. **Firebase** - Ma'lumotlarni saqlash

### Formspree bilan misol:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

## 🔧 Texnik talablar

- Brauzer: Chrome, Firefox, Safari, Edge (so'nggi versiyalar)
- Mobile: iOS 12+, Android 8+
- Responsive: 320px dan 1920px gacha

## 📄 Litsenziya

© 2025 NanoCam. Barcha huquqlar himoyalangan.
