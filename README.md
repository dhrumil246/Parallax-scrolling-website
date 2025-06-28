# Parallax Scrolling Website 🏔️

A visually stunning single-page website featuring an interactive parallax scrolling effect that takes users on a mystical mountain journey through different elevation zones.


## ✨ Features

- **Multi-layer Parallax Effect**: 9 different background layers moving at varying speeds to create depth
- **Smooth Animations**: CSS transitions and JavaScript-powered scroll animations
- **Responsive Design**: Optimized for both desktop and mobile devices
- **Interactive Elements**: Animated showcase gallery with scroll-triggered effects
- **Modern Typography**: Beautiful Pacifico and Poppins fonts
- **Performance Optimized**: Lightweight and fast-loading

## 🚀 Demo

Experience the live demo: [Parallax Scrolling Website](https://dhrumil246.github.io/Parallax-scrolling-website/)

## 📁 Project Structure

```
Parallax-scrolling-website/
├── index.html          # Main HTML file
├── style.css           # CSS styles and animations
├── app.js              # JavaScript functionality
└── img/                # Image assets
    ├── 0.png - 8.png   # Parallax background layers
    ├── 9.jpg - 12.jpg  # Showcase gallery images
    └── logo.jpg        # Profile image
```

## 🛠️ Technologies Used

- **HTML5**: Semantic markup structure
- **CSS3**: Advanced styling, flexbox, grid, and animations
- **Vanilla JavaScript**: Smooth scroll effects and DOM manipulation
- **Google Fonts**: Pacifico and Poppins font families

## 🎯 How It Works

### Parallax Effect
The parallax scrolling effect is achieved through JavaScript by:
1. Detecting scroll position using `window.scrollY`
2. Moving background layers at different speeds based on their index
3. Creating depth perception through varied translation speeds

```javascript
listBg.forEach((bg, index) => {
    if(index != 0 && index != 8){
        bg.style.transform = `translateY(${(top*index/2)}px)`;
    }else if(index == 0){
        bg.style.transform = `translateY(${(top/3)}px)`;
    }
})
```

### Animation System
Elements animate into view when they reach a specific scroll threshold:
- Uses intersection-based visibility detection
- Staggered animations with CSS transition delays
- Smooth opacity and transform transitions

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Web server (optional, for local development)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/dhrumil246/Parallax-scrolling-website.git
   ```

2. **Navigate to project directory**
   ```bash
   cd Parallax-scrolling-website
   ```

3. **Open with live server** (recommended)
   ```bash
   # Using VS Code Live Server extension
   # Or using Python
   python -m http.server 8000
   
   # Or using Node.js
   npx serve .
   ```

4. **Open in browser**
   ```
   http://localhost:8000
   ```

## 📱 Responsive Breakpoints

- **Desktop**: > 768px - Full grid layout with 4 columns
- **Mobile**: ≤ 768px - 2-column grid layout with adjusted font sizes

## 🎨 Customization

### Changing Background Images
Replace images in the `img/` folder:
- `0.png` to `8.png`: Parallax background layers (arrange from background to foreground)
- `9.jpg` to `12.jpg`: Showcase gallery images

### Modifying Parallax Speed
Adjust the speed multipliers in `app.js`:
```javascript
bg.style.transform = `translateY(${(top*index/2)}px)`; // Change the divisor
```

### Updating Colors
Modify the CSS variables in `style.css`:
```css
body {
    background-color: #210002; /* Main background */
}
```

## 🔧 Performance Tips

- Optimize images for web (WebP format recommended)
- Use CSS `will-change` property for animated elements
- Consider using `transform3d()` for hardware acceleration
- Implement lazy loading for images below the fold

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Dhrumil Amin**
- GitHub: [@dhrumil246](https://github.com/dhrumil246)
- Website: [Parallax Scrolling Website](https://github.com/dhrumil246/Parallax-scrolling-website)

## 🙏 Acknowledgments

- Inspiration from modern parallax scrolling websites
- Google Fonts for typography
- Community feedback and contributions

## 📊 Browser Support

| Browser | Version |
|---------|---------|
| Chrome  | ≥ 60    |
| Firefox | ≥ 55    |
| Safari  | ≥ 12    |
| Edge    | ≥ 79    |

---

⭐ Star this repository if you found it helpful!
