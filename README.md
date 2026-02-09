# Will Napolini - # 🔗 LinkBio - Modern Links in Bio Website

> A beautiful, modern alternative to Linktree with glassmorphism design, smooth animations, and mobile-first approach.

![LinkBio Preview](https://github.com/willnapolinighub/willinks/blob/main/assets/assets-will-napolini-linkbio-preview.png)

![Portfolio Preview](https://img.shields.io/badge/Status-Active-success)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![TailwindCSS](https://img.shields.io/badge/Tailwind-38B2AC?logo=tailwind-css&logoColor=white)

## ✨ Features

### 🎨 Visual Design
- **Glassmorphism UI** - Modern frosted glass aesthetic with backdrop blur effects
- **5 Theme Options** - Switch between Blazing Suns, Ocean Breeze, Forest Green, Night Mode, and Purple Haze
- **Smooth Animations** - Floating avatar, gentle bounces, and elegant transitions
- **Responsive Design** - Mobile-first approach optimized for all screen sizes
- **Accessibility First** - ARIA labels, keyboard navigation, and reduced motion support

### 🔗 Content Sections
- **Profile Card** - Avatar, name, tagline, and theme switcher
- **Social Media Links** - Telegram, Twitter, Pinterest, and Threads
- **Video Platforms** - YouTube, TikTok, and Instagram Reels with external link indicators
- **GitHub Connection** - Direct link to GitHub profile

### 💾 Persistent Settings
- Theme preference saved to localStorage
- Remembers user's theme choice across sessions

## 🚀 Quick Start

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/willnapolini/portfolio.git
cd portfolio
```

2. **Open in browser**
```bash
# Simply open index.html in your browser
# No build process or dependencies required!
```

### Customization

Edit the following sections in `index.html`:

**Profile Information:**
```html
<!-- Line 140-142 -->
<img src="YOUR_AVATAR_URL" alt="Your Name">
<h1>Your Name</h1>
<p>Your Tagline</p>
```

**Social Media Links:**
```html
<!-- Lines 151-162 -->
<a href="https://t.me/yourusername">...</a>
<a href="https://twitter.com/yourusername">...</a>
<a href="https://pinterest.com/yourusername">...</a>
<a href="https://www.threads.net/@yourusername">...</a>
```

**Video Platform Links:**
```html
<!-- Lines 167-201 -->
<a href="https://youtube.com/@yourusername">...</a>
<a href="https://tiktok.com/@yourusername">...</a>
<a href="https://instagram.com/yourusername/reels">...</a>
```

**GitHub Link:**
```html
<!-- Line 207 -->
<a href="https://github.com/yourusername">...</a>
```

## 🎨 Theme System

The portfolio includes 5 pre-built themes:

| Theme | Colors | Best For |
|-------|--------|----------|
| **Blazing Suns** | Orange → Red → Yellow | Energy, Creativity |
| **Ocean Breeze** | Cyan → Blue → Indigo | Calm, Professional |
| **Forest Green** | Green → Emerald → Teal | Nature, Growth |
| **Night Mode** | Gray → Dark Gray → Black | Minimalist, Tech |
| **Purple Haze** | Purple → Fuchsia → Pink | Creative, Bold |

### Adding Custom Themes

Add to the `themes` array in the JavaScript section:

```javascript
{
  name: 'Your Theme Name',
  classes: 'bg-gradient-to-br from-color-400 via-color-500 to-color-600'
}
```

## 📁 Project Structure

```
portfolio/
├── index.html          # Main HTML file (includes CSS & JS)
├── README.md           # This file
├── DOCUMENTATION.md    # Detailed technical documentation
└── LICENSE             # MIT License
```

## 🛠️ Technology Stack

- **HTML5** - Semantic markup
- **CSS3** - Custom properties, animations, glassmorphism
- **JavaScript (Vanilla)** - Theme switching, localStorage
- **Tailwind CSS** - Utility-first styling via CDN
- **Font Awesome** - Icon library

**No build tools, no npm, no frameworks!** This is pure, vanilla web development.

## 🌐 Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

**Note:** Backdrop filter effects require modern browser support.

## 📱 Responsive Breakpoints

- **Mobile**: < 480px (optimized default)
- **Tablet**: 480px - 768px
- **Desktop**: > 768px

Max container width: 375px (optimal for mobile-first design)

## ♿ Accessibility Features

- ✅ ARIA labels on all interactive elements
- ✅ Keyboard navigation support
- ✅ Focus-visible indicators
- ✅ Reduced motion support for users with motion sensitivity
- ✅ Semantic HTML structure
- ✅ Alt text on images

## 🚀 Deployment

### GitHub Pages
1. Push code to GitHub
2. Go to Settings → Pages
3. Select main branch
4. Your site will be live at `https://yourusername.github.io/portfolio`

### Vercel
```bash
npm i -g vercel
vercel
```

### Netlify
```bash
# Drag and drop the folder to netlify.com
# Or connect your GitHub repo
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Design inspiration from modern glassmorphism trends
- Icons provided by [Font Awesome](https://fontawesome.com/)
- Styling framework by [Tailwind CSS](https://tailwindcss.com/)

## 📧 Contact

Will Napolini - [@willnapolini](https://twitter.com/willnapolini)

Project Link: [https://github.com/willnapolini/portfolio](https://github.com/willnapolini/portfolio)

---

⭐ If you found this helpful, please give it a star!

Made with ❤️ by Will Napolini
