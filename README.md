<p align="center">
  <img src="https://img.freepik.com/free-vector/blue-neon-glow-rectangle-frame_107791-27358.jpg?semt=ais_hybrid&w=740&q=80" alt="Neon Frame" width="100%">
</p>

# 🎨 Modern Card Stack Showcase

A stunning, interactive card stacking website featuring smooth scroll animations, modern design principles, and cutting-edge visual effects. Built with vanilla HTML, CSS, and GSAP ScrollTrigger.

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![GSAP](https://img.shields.io/badge/GSAP-3.12.2-brightgreen.svg)

## ✨ Features

- **Smooth Card Stacking Animation** - Cards elegantly stack and scale as you scroll
- **Interactive Parallax Effects** - Dynamic image movement for immersive experience
- **Glassmorphism Design** - Modern frosted glass aesthetics with backdrop blur
- **Animated Background Particles** - Floating gradient particles for depth
- **Fully Responsive** - Optimized for desktop, tablet, and mobile devices
- **Hardware Accelerated** - Smooth 60fps animations using GPU rendering
- **Progressive Enhancement** - Works without JavaScript, enhanced with it
- **Accessible Design** - Semantic HTML and proper contrast ratios

## 🚀 Demo

[Card Stack Demo](https://moderncardstack.netlify.app/)

*Smooth scroll-triggered stacking animation with progressive scaling*

## 🛠️ Technologies Used

- **HTML5** - Semantic markup structure
- **CSS3** - Advanced styling with Grid, Flexbox, and animations
- **JavaScript (ES6+)** - Modern JavaScript for interactions
- **GSAP 3.12.2** - Professional-grade animation library
- **ScrollTrigger** - Scroll-based animation plugin
- **Unsplash API** - High-quality placeholder images

## 📋 Prerequisites

No build tools or package managers required! This project uses:
- Modern web browser with ES6 support
- CDN-hosted libraries (GSAP, ScrollTrigger)

## 🎯 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/vishalvalvi/modern-card-stack.git
   cd modern-card-stack
   ```

2. **Open in browser**
   ```bash
   # Simply open the HTML file
   open index.html
   
   # Or use a local server
   python -m http.server 8000
   # Then visit http://localhost:8000
   ```

3. **Optional: Use Live Server**
   - Install [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in VS Code
   - Right-click on `index.html` and select "Open with Live Server"

## 📁 Project Structure

```
modern-card-stack/
│
├── index.html              # Main HTML file with embedded CSS and JS
├── README.md              # Project documentation

```

## 🎨 Customization

### Changing Colors

Update the CSS variables in the `:root` selector:

```css
:root {
  --color-dark: #0a0a0f;
  --color-accent: #6366f1;
  --color-white: #ffffff;
  --color-gradient-1: #667eea;
  --color-gradient-2: #764ba2;
}
```

### Adding New Cards

Add a new card block in the HTML:

```html
<div class="c-card">
  <div class="c-card__description">
    <div class="c-card__tagline">🎯 Your Category</div>
    <h2 class="c-card__title">Your Title</h2>
    <div class="c-card__excerpt">Your description here...</div>
    <div class="c-card__stats">
      <div class="stat">
        <div class="stat-number">100+</div>
        <div class="stat-label">Your Metric</div>
      </div>
    </div>
    <div class="c-card__cta">
      <a href="#" class="btn-primary">
        <span>Action</span>
        <span>→</span>
      </a>
    </div>
  </div>
  <div class="c-card__figure">
    <div class="feature-badge">✨ Badge</div>
    <img src="your-image.jpg" alt="Description">
  </div>
</div>
```

### Modifying Animation Speed

Adjust the `scrub` value in the JavaScript:

```javascript
scrollTrigger: {
  trigger: card,
  start: "top top",
  end: () => `+=${cardHeight + spacing}`,
  pin: true,
  pinSpacing: false,
  scrub: 1, // Lower = faster, Higher = slower
}
```

### Replacing Images

Replace Unsplash URLs with your own:

```html
<!-- Before -->
<img src="https://images.unsplash.com/photo-xyz" alt="Description">

<!-- After -->
<img src="assets/images/your-image.jpg" alt="Description">
```

## 🎭 Browser Support

| Browser | Version |
|---------|---------|
| Chrome  | ✅ 90+  |
| Firefox | ✅ 88+  |
| Safari  | ✅ 14+  |
| Edge    | ✅ 90+  |
| Opera   | ✅ 76+  |

**Note:** Requires support for CSS Grid, Flexbox, and ES6+ JavaScript

## ⚡ Performance Optimization

- **Hardware Acceleration**: Uses `transform` and `opacity` for GPU rendering
- **Lazy Loading**: Images can be lazy-loaded (add `loading="lazy"` attribute)
- **Debounced Resize**: Prevents excessive recalculations on window resize
- **Optimized ScrollTrigger**: Uses `invalidateOnRefresh` for accurate positioning

## 🐛 Known Issues & Solutions

### Cards Getting Stuck
**Solution**: Refresh ScrollTrigger after dynamic content loads
```javascript
ScrollTrigger.refresh();
```

### Jumpy Animations on Mobile
**Solution**: Reduce animation complexity or increase scrub value
```javascript
scrub: 2 // Instead of scrub: 1
```

### Images Not Loading
**Solution**: Check CORS policy and use proper image URLs or local files

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Vishal Valvi**

- GitHub: [@vishalvalvi](https://github.com/VishalValvi-83)
- LinkedIn: [Vishal Valvi](https://linkedin.com/in/vishal-valvi)
- Instagram: [vishalvalvi.com](https://www.instagram.com/v.i.s.h.a.l__83)

## 🙏 Acknowledgments

- **[GSAP (GreenSock)](https://greensock.com/gsap/)** - Professional-grade animation library
- **[Unsplash](https://unsplash.com)** - Beautiful free images and photos
- **[CSS-Tricks](https://css-tricks.com)** - Excellent web development resources
- **Design Inspiration**: Modern web design trends and best practices

## 📚 Resources & Learning

- [GSAP Documentation](https://greensock.com/docs/)
- [ScrollTrigger Guide](https://greensock.com/docs/v3/Plugins/ScrollTrigger)
- [CSS Grid Complete Guide](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [Modern JavaScript Tutorial](https://javascript.info/)

## 🔮 Future Enhancements

- [ ] Add dark/light theme toggle
- [ ] Implement touch gestures for mobile
- [ ] Add more card variations and layouts
- [ ] Create animation presets system
- [ ] Add accessibility improvements (ARIA labels)
- [ ] Integrate with CMS for dynamic content
- [ ] Add unit tests for animations
- [ ] Create React/Vue component versions

## 💬 Feedback

If you have any feedback, suggestions, or issues, please:
- Open an issue on GitHub
- Contact me via email
- Submit a pull request with improvements

## ⭐ Show Your Support

If you like this project, please give it a ⭐ on GitHub!

---

**Disclaimer**: This project is created for demonstration and educational purposes. All product names, technologies, and content examples are used for illustrative purposes only. Images are provided by Unsplash under their license terms. When using in production, ensure you have appropriate licenses for all resources.

---

Made with ❤️ by Vishal Valvi | © 2025 All Rights Reserved
