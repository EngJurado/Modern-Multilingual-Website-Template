# Modern Multilingual Website Template

A clean, modern, and responsive website template with **automatic language detection** and **dark/light theme support**. Perfect for personal portfolios, landing pages, or small projects hosted on GitHub Pages.

![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-blue?style=flat-square&logo=github)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🌍 **Auto Language Detection** | Detects user's browser language (Spanish/English) |
| 🌓 **Dark/Light Theme** | Automatic theme detection + manual toggle button |
| 💾 **LocalStorage** | Remembers user preferences (language & theme) |
| 📱 **Responsive Design** | Works perfectly on mobile, tablet, and desktop |
| 🎨 **Modern CSS** | Native CSS nesting, variables, and smooth transitions |
| ⚡ **No Dependencies** | Pure HTML, CSS, and JavaScript (no frameworks) |
| 🚀 **GitHub Pages Ready** | Deploy in minutes with zero configuration |

---

## 🚀 Live Demo

[View Demo](https://engjurado.github.io/Modern-Multilingual-Website-Template/)

---

## 📦 Quick Start

### Option 1: Use as Template
1. Click **"Use this template"** → **"Create a new repository"**
2. Name your repository (e.g., `my-website`)
3. Clone your new repo:
   ```bash
   git clone https://github.com/EngJurado/my-website.git
   cd my-website
   ```

### Option 2: Clone Directly
```bash
git clone https://github.com/EngJurado/Modern-Multilingual-Website-Template.git
cd Modern-Multilingual-Website-Template
```

### Option 3: Download ZIP
1. Click the **"Code"** button above
2. Select **"Download ZIP"**
3. Extract and upload to your repository

---

## ⚙️ GitHub Pages Setup

1. Go to your repository **Settings** → **Pages**
2. Under **Build and deployment**:
   - Source: `Deploy from a branch`
   - Branch: `main` → `/ (root)`
3. Click **Save**
4. Wait ~60 seconds for deployment
5. Your site will be live at: `https://yourusername.github.io/your-repo-name`

---

## 🛠️ Customization

### 🌐 Add More Languages

Edit the `translations` object in `index.html`:

```javascript
const translations = {
    es: { 
        title: "¡Hola! Diseño Moderno", 
        description: "Descripción en español...",
        lang_label: "Idioma detectado:"
    },
    en: { 
        title: "Hello! Modern Design", 
        description: "Description in English...",
        lang_label: "Detected language:"
    },
    // Add new language below 👇
    fr: {
        title: "Bonjour! Design Moderne", 
        description: "Description en français...",
        lang_label: "Langue détectée:"
    }
};
```

Add the button in HTML:
```html
<button class="btn btn-fr" onclick="setLanguage('fr')">🇫🇷 Français</button>
```

### 🎨 Customize Colors

Edit CSS variables in the `<style>` section:

```css
:root {
    --bg-body: #f0f2f5;          /* Page background */
    --bg-card: #ffffff;          /* Card background */
    --text-primary: #1a1a1a;     /* Main text */
    --text-secondary: #65676b;   /* Secondary text */
    --accent-color: #3b82f6;     /* Buttons & links */
    --accent-hover: #2563eb;     /* Button hover */
    --border-color: #e4e6eb;     /* Borders */
    --shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}
```

### 📝 Add More Content

Add any HTML element with `data-i18n` attribute:

```html
<h2 data-i18n="subtitle">Your Subtitle</h2>
<p data-i18n="paragraph">Your paragraph text...</p>
<a href="#" data-i18n="link">Click here</a>
```

Then add translations:
```javascript
const translations = {
    es: {
        subtitle: "Tu subtítulo",
        paragraph: "Texto del párrafo...",
        link: "Haz clic aquí"
    },
    en: {
        subtitle: "Your subtitle",
        paragraph: "Paragraph text...",
        link: "Click here"
    }
};
```

---

## 📁 File Structure

```
Modern-Multilingual-Website-Template/
│
├── index.html          # Main file (HTML + CSS + JS)
├── README.md           # Documentation
└── .github/            # GitHub configurations (optional)
    └── FUNDING.yml     # Sponsorship info (optional)
```

---

## 🖥️ Browser Support

| Browser | Version | CSS Nesting |
|---------|---------|-------------|
| Chrome | 112+ | ✅ |
| Firefox | 117+ | ✅ |
| Safari | 17+ | ✅ |
| Edge | 112+ | ✅ |
| Opera | 98+ | ✅ |

> **Note:** Native CSS nesting requires modern browsers. For legacy support, use Sass/PostCSS with a nesting plugin.

---

## 🔧 Troubleshooting

### Language not changing?
1. Open DevTools (`F12`) → Console tab
2. Check for warnings about missing translation keys
3. Verify `data-i18n` attributes match keys in the `translations` object
4. Hard refresh: `Ctrl + Shift + R` (Windows) or `Cmd + Shift + R` (Mac)

### Theme not detecting automatically?
1. Check your OS theme settings (System Preferences → Appearance)
2. Clear localStorage: DevTools → Application → Local Storage → Clear
3. Reload the page

### GitHub Pages not updating?
1. Wait up to 2 minutes for deployment
2. Hard refresh your browser
3. Check **Settings** → **Pages** for build errors
4. Verify you're pushing to the correct branch (`main`)

---

## 🤝 Contributing

Contributions are welcome! Here's how:

1. **Fork** the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit changes: `git commit -m 'Add: your feature'`
4. Push: `git push origin feature/your-feature`
5. Open a **Pull Request**

### Contribution Guidelines
- Keep changes focused and well-documented
- Test in both light/dark modes
- Ensure translations are consistent
- Follow existing code style

---

## 📄 License

This project is licensed under the **MIT License**.

```
MIT License

Copyright (c) 2026 EngJurado

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 🙏 Acknowledgments

- Built with pure HTML, CSS, and JavaScript
- Inspired by modern design systems and accessibility best practices
- Optimized for GitHub Pages static hosting

---

## 📞 Contact

- **Author:** EngJurado
- **GitHub:** [@EngJurado](https://github.com/EngJurado)
- **Demo:** [Live Site](https://engjurado.github.io/Modern-Multilingual-Website-Template/)

---

<div align="center">

**Made with ❤️ by [EngJurado](https://github.com/EngJurado)**

If you find this template useful, please give it a ⭐ star!

</div>

---

*Last Updated: 2026 | Version: 1.0.0*
