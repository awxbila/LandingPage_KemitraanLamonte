# 🎯 Lamonte Partnership Landing Page

Landing page modern dan responsif untuk platform kemitraan bisnis baju anak **Lamonte** dengan pengalaman pengguna yang optimal di semua perangkat.

---

## ✨ Fitur Utama

### 🎨 **Desain & Animasi**

- **Intro Screen Premium** - Halaman pembuka visual dengan gradien hijau-kuning yang eye-catching
- **Smooth Scroll Animations** - Animasi entrance/exit otomatis saat scroll ke section
- **Dark Mode Support** - Toggle tema terang/gelap yang persist di browser
- **Gradient Typography** - Text dengan gradient warna brand untuk visual impact

### 📱 **Responsif Sempurna**

- Mobile-first design untuk HP (≤480px, ≤640px)
- Tablet portrait & landscape optimized (≤768px, 769px-1024px)
- Desktop full experience (≥1025px)
- Fluid typography dengan `clamp()` CSS

### 🚀 **Showcase & Interaksi**

- **Hero Section** - Presentasi utama dengan key benefits & statistics
- **Module Ecosystem** - Slider 3-kolom untuk fitur produk dengan hover effects
- **Partnership Flow** - Step-by-step business process dengan card design
- **Testimonial Marquee** - Carousel otomatis dengan fade-out rules
- **Product Catalog** - Grid/list toggle, sorting by relevance/price, order CTA
- **Contact Form** - WhatsApp integration untuk seamless inquiry

### 🎛️ **Teknologi**

- **Vanilla JavaScript** - Tanpa framework, pure DOM manipulation
- **IntersectionObserver API** - Efficient scroll-based visibility tracking
- **CSS3 Features** - Gradients, animations, media queries, clamp()
- **localStorage/sessionStorage** - Persistent user preferences
- **Responsive Images** - Lazy loading support

---

## 📁 Struktur Project

```
LandingPage_KemitraanLamonte/
├── index.html                 # Halaman landing utama
├── katalog.html               # Halaman katalog produk
├── README.md                  # File dokumentasi ini
├── assets/
│   ├── styles.css             # Stylesheet utama (desktop-first base)
│   ├── media-queries.css      # Media queries mobile & tablet
│   ├── img/
│   │   ├── logo.png           # Logo Lamonte
│   │   ├── sun.svg            # Icon mode terang
│   │   ├── moon.svg           # Icon mode gelap
│   │   ├── herosection.jpg    # Hero visual
│   │   ├── katalog 1-6.jpg    # Produk images
│   │   └── [other assets]     # Aset lainnya
```

---

## 🎬 Fitur Halaman Utama (index.html)

### Intro Screen

```
Durasi: 3.2 detik otomatis (pertama kali saja, disimpan di localStorage)
Desain: Gradient hijau-kuning dengan decorative circles
Text: "Apakah kamu tertarik bergabung bersama kami?"
```

### Hero Section

- Headline menarik + sub-headline dengan emphasis text
- 4 key benefits dalam grid
- 3 statistik omzet/rating/penjualan
- Visual image responsive

### Module Ecosystem

- Slider horizontal 3-item per view
- Card hover: lift, border highlight, shadow glow
- Image: grayscale→saturated saat hover
- Dimming saat scroll luar viewport

### Partnership (Kemitraan) Section

- Copy + business flow steps
- 5 step cards dengan hover effect
- Alert box dengan info penting
- CTA button dengan WhatsApp link

### Testimonial Section

- Auto-scrolling marquee (60s loop)
- Fade-in saat section visible
- Hide saat footer muncul (footer precedence)
- Multiple cards dengan ratings

### Footer

- Social media links (Instagram, TikTok, Facebook, YouTube, WhatsApp)
- Company info (alamat, telepon, email, website)
- Feedback form dengan WhatsApp integration

---

## 📋 Fitur Halaman Katalog (katalog.html)

### Hero + Catalog Info

- Matching animations dengan halaman utama
- Deskripsi singkat paket kemitraan
- Panel informatif dengan checklist

### Product Grid & Controls

- **View Toggle**: Grid (3 kolom) ↔ List view
- **Sort By**: Relevance / Price Ascending / Price Descending
- **Order Button**: Hover image zoom + WhatsApp order link
- **Best Seller Badge**: Highlight untuk 3 top products

### Responsive Products

- Grid: 3 kolom (desktop) → 2 kolom (tablet) → 1 kolom (mobile)
- Reveal: Saat section center mencapai viewport center
- Hide: Saat footer sepenuhnya visible (precedence)

---

## 🎨 Tema Warna (CSS Variables)

### Mode Terang (Default)

```css
--green-900: #0f3f12 --green-700: #2f6a1d --green-500: #4e8b2a
  --yellow-500: #f0d53f --cream-50: #fffdf3 --cream-100: #f8f3df;
```

### Mode Gelap

```css
--bg-page: #0f1713 --text-main: #e7f1e4 --accent: #86b85b;
```

---

## 🚀 Cara Menggunakan

### 1. **Buka Halaman**

```
Browser: Chrome, Firefox, Safari, Edge (modern versions)
Desktop: http://localhost/LandingPage_KemitraanLamonte/index.html
Katalog: http://localhost/LandingPage_KemitraanLamonte/katalog.html
```

### 2. **Fitur Toggle Tema**

- Klik icon matahari/bulan di navbar (kanan atas)
- Tema tersimpan otomatis di browser
- Berlaku untuk kedua halaman

### 3. **Navigasi Smooth Scroll**

- Klik menu (Home/Module/Kemitraan/Contact) → auto scroll ke section
- Header offset 84px untuk sticky header
- Behavior: smooth

### 4. **Interaksi Produk**

- **Grid/List**: Toggle di atas grid
- **Sort**: Pilih relevansi atau harga (ascending/descending)
- **Order**: Hover card → klik tombol yellow → WhatsApp admin penjualan

### 5. **Form Feedback**

- Tulis pesan di textarea
- Klik "Send" → automatic WhatsApp window
- WhatsApp number configurable via `data-wa-number` attribute

---

## 📊 Performance & Accessibility

### Optimasi

- ✅ Lazy loading untuk images
- ✅ CSS transitions & animations (smooth 60fps)
- ✅ Efficient event listeners (passive scroll)
- ✅ Minimal JS bundle (vanilla, no frameworks)

### Accessibility

- ✅ Semantic HTML (header, main, footer, article, section)
- ✅ ARIA labels & roles (dialog, navigation, status)
- ✅ Keyboard navigation support
- ✅ Color contrast compliance
- ✅ `prefers-reduced-motion` fallbacks

---

## 🔧 Responsive Breakpoints

| Device           | Width      | Breakpoint          | Layout      |
| ---------------- | ---------- | ------------------- | ----------- |
| Mobile Small     | ≤480px     | Custom font scaling | 1 column    |
| Mobile Medium    | ≤640px     | Improved spacing    | 1-2 columns |
| Mobile/Tablet    | ≤768px     | Full navigation     | 2 columns   |
| Tablet Landscape | 769-1024px | Semi-desktop        | 2-3 columns |
| Desktop          | ≥1025px    | Full experience     | 3+ columns  |

### Media Query Files

- **styles.css** - Base desktop styles + existing breakpoints (980px, 680px)
- **media-queries.css** - New mobile-first breakpoints (480px, 640px, 768px, 1024px)

---

## 📞 Integrasi WhatsApp

### Format Pesan Otomatis

```
Order: "Halo admin Lamonte, saya ingin order [Nama Paket]..."
Feedback: "Halo layanan Lamonte, saya ingin menyampaikan: [Pesan]"
```

### Konfigurasi Nomor

Edit di HTML:

```html
<!-- Untuk order produk -->
const salesWaNumber = "6281234567891";

<!-- Untuk feedback -->
data-wa-number="6281234567890"
```

---

## 🔐 Browser Storage

### localStorage (Persist Across Sessions)

- `lamonte-theme` - Dark/light mode preference
- `lamonte-intro-seen` - Intro screen status

### Cara Clear

```javascript
localStorage.removeItem("lamonte-theme");
localStorage.removeItem("lamonte-intro-seen");
localStorage.clear(); // Clear semua
```

---

## 🎯 User Behavior

### First Visit Flow

1. Intro screen muncul (3.2 detik) → auto fade out
2. Landing page fully visible
3. Sticky header dengan smooth nav
4. Scroll reveals sections dengan animation
5. Dark mode preference saved

### Return Visits

1. Intro screen TIDAK tampil (stored in localStorage)
2. Preferensi tema dimuat instant
3. Page fully interactive

---

## 📧 Kontak & Social Media

| Platform  | Link                                 |
| --------- | ------------------------------------ |
| Instagram | https://instagram.com/lamonte        |
| TikTok    | https://tiktok.com/@lamonte          |
| Facebook  | https://facebook.com/lamonte         |
| YouTube   | https://youtube.com/lamonte          |
| WhatsApp  | https://whatsapp.com/channel/lamonte |
| Website   | https://lamonte.id                   |

---

## 📝 Catatan Teknis

### IntersectionObserver Rules

- **Hero**: Show ≥45%, Hide ≤20%
- **Module**: Show ≥45%, Hide ≤28%
- **Mitra**: Show left→right stagger, Hide when out of viewport, Replay on re-entry
- **Testimonial**: Show ≥45%, But hide if footer ≥95% visible (precedence)
- **Products**: Show saat center mencapai viewport center, Hide if footer ≥95%

### Animation Timings

```
Hero enter: 1.08s (0.14s delay) → 0.9s → 0.88s → 0.9s
Module stagger: per card dengan delays
Testimonial marquee: 60s linear infinite (paused until visible)
Intro fade: 0.8s ease-out
```

---

## ✅ Testing Checklist

- [ ] Light mode displays correctly
- [ ] Dark mode toggle works & persists
- [ ] Intro screen appears once, then hidden
- [ ] All scroll animations trigger on viewport enter
- [ ] Testimonial marquee loops smoothly
- [ ] Product sort (all 3 options) works
- [ ] Product grid/list toggle works
- [ ] Order button opens WhatsApp correctly
- [ ] Form feedback sends WhatsApp message
- [ ] Mobile responsive ≤480px, ≤640px, ≤768px
- [ ] Tablet landscape 769-1024px smooth
- [ ] No console errors
- [ ] No layout shifts

---

## 📄 License

© 2026 Kemitraan Lamonte. Seluruh hak cipta dilindungi.

---

**Last Updated**: April 17, 2026  
**Version**: 1.0  
**Status**: Production Ready ✅
