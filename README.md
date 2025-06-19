# Portfolio Pribadi

Website portfolio pribadi yang modern, responsif, dan interaktif. Dibuat dengan HTML, CSS, dan JavaScript vanilla.

## 🚀 Fitur

- **Design Modern**: Interface yang clean dan profesional dengan gradien warna yang menarik
- **Responsif**: Optimal di semua perangkat (desktop, tablet, mobile)
- **Animasi Smooth**: Transisi dan animasi yang halus untuk pengalaman yang lebih baik
- **Mobile Menu**: Menu hamburger untuk tampilan mobile
- **Smooth Scrolling**: Navigasi yang mulus antar section
- **Form Kontak**: Form kontak yang interaktif dengan validasi
- **Scroll Animations**: Animasi fade-in saat scroll
- **Parallax Effect**: Efek parallax pada hero section
- **Typing Animation**: Animasi typing pada judul utama

## 📁 Struktur File

```
portfolio/
├── index.html          # File HTML utama
├── styles.css          # File CSS untuk styling
├── script.js           # File JavaScript untuk interaktivitas
└── README.md           # Dokumentasi
```

## 🎨 Sections

1. **Hero Section**: Bagian utama dengan nama dan deskripsi singkat
2. **About Section**: Informasi tentang diri dan statistik pengalaman
3. **Skills Section**: Keahlian dan teknologi yang dikuasai
4. **Projects Section**: Portfolio proyek-proyek yang telah dikerjakan
5. **Contact Section**: Form kontak dan informasi kontak
6. **Footer**: Social media links dan copyright

## 🛠️ Teknologi yang Digunakan

- **HTML5**: Struktur semantic dan modern
- **CSS3**: 
  - Flexbox dan Grid untuk layout
  - CSS Variables untuk konsistensi warna
  - Animasi dan transisi
  - Media queries untuk responsivitas
- **JavaScript ES6+**:
  - Intersection Observer API untuk scroll animations
  - Event handling
  - DOM manipulation
  - Form validation

## 📱 Responsivitas

Website ini responsif dengan breakpoint:
- **Desktop**: > 768px
- **Tablet**: 768px - 480px
- **Mobile**: < 480px

## 🎯 Cara Kustomisasi

### 1. Mengubah Informasi Pribadi

Edit file `index.html` dan ubah:
- Nama di hero section (line 47)
- Deskripsi di about section (line 75-80)
- Statistik pengalaman (line 82-90)
- Informasi kontak (line 200-220)

### 2. Mengubah Warna

Edit file `styles.css` dan ubah CSS variables:
```css
:root {
    --primary-color: #2563eb;
    --secondary-color: #fbbf24;
    --gradient-primary: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}
```

### 3. Menambah Proyek

Tambahkan card proyek baru di section projects:
```html
<div class="project-card">
    <div class="project-image">
        <i class="fas fa-[icon-name]"></i>
    </div>
    <div class="project-content">
        <h3>Nama Proyek</h3>
        <p>Deskripsi proyek</p>
        <div class="project-tech">
            <span>Teknologi 1</span>
            <span>Teknologi 2</span>
        </div>
        <div class="project-links">
            <a href="#" class="btn btn-small">Demo</a>
            <a href="#" class="btn btn-small btn-outline">GitHub</a>
        </div>
    </div>
</div>
```

### 4. Menambah Keahlian

Tambahkan skill card baru di section skills:
```html
<div class="skill-card">
    <div class="skill-icon">
        <i class="fab fa-[icon-name]"></i>
    </div>
    <h3>Nama Skill</h3>
    <p>Deskripsi skill</p>
</div>
```

## 🚀 Cara Menjalankan

1. Clone atau download repository ini
2. Buka file `index.html` di browser
3. Atau gunakan live server untuk development

### Menggunakan Live Server (VS Code)

1. Install extension "Live Server"
2. Klik kanan pada `index.html`
3. Pilih "Open with Live Server"

### Menggunakan Python

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Kemudian buka `http://localhost:8000`

## 📧 Form Kontak

Form kontak saat ini menggunakan simulasi. Untuk implementasi nyata, Anda perlu:

1. **Backend Service**: Gunakan layanan seperti:
   - Formspree
   - Netlify Forms
   - EmailJS
   - Custom backend

2. **Implementasi dengan EmailJS**:
```javascript
// Tambahkan EmailJS script
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>

// Inisialisasi
emailjs.init("YOUR_USER_ID");

// Kirim email
emailjs.send("YOUR_SERVICE_ID", "YOUR_TEMPLATE_ID", {
    from_name: formData.get('name'),
    from_email: formData.get('email'),
    message: formData.get('message')
});
```

## 🎨 Kustomisasi Lanjutan

### Menambah Animasi

Tambahkan class CSS untuk animasi baru:
```css
@keyframes slideInFromLeft {
    from {
        transform: translateX(-100%);
        opacity: 0;
    }
    to {
        transform: translateX(0);
        opacity: 1;
    }
}

.slide-in-left {
    animation: slideInFromLeft 0.8s ease-out;
}
```

### Menambah Dark Mode

Tambahkan toggle dark mode:
```javascript
const darkModeToggle = document.querySelector('.dark-mode-toggle');
darkModeToggle.addEventListener('click', () => {
    document.body.classList.toggle('dark-mode');
});
```

## 📝 Lisensi

Proyek ini open source dan dapat digunakan untuk keperluan pribadi maupun komersial.

## 🤝 Kontribusi

Kontribusi selalu diterima! Silakan:
1. Fork repository
2. Buat branch fitur baru
3. Commit perubahan
4. Push ke branch
5. Buat Pull Request

## 📞 Support

Jika ada pertanyaan atau masalah, silakan buat issue di repository ini.

---

**Dibuat dengan ❤️ untuk portfolio pribadi yang profesional** 