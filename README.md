# Karthikeyan Danasagaran - Mechanical Engineer Portfolio

A beautiful, responsive, and feature-rich portfolio website built with modern web technologies. Perfect for showcasing your skills, projects, and experience as a mechanical engineer.

## 🌟 Features

### Modern Design & UX
- **Responsive Design**: Works perfectly on all devices (desktop, tablet, mobile)
- **Dark/Light Theme Toggle**: User preference with smooth transitions
- **Smooth Animations**: CSS animations and JavaScript-powered interactions
- **Modern UI**: Clean, professional design with gradient accents
- **Loading Screen**: Professional loading animation

### Technical Features
- **Semantic HTML5**: Better SEO and accessibility
- **CSS Grid & Flexbox**: Modern layout techniques
- **CSS Custom Properties**: Dynamic theming and easy customization
- **Intersection Observer API**: Scroll-triggered animations
- **Service Worker Ready**: PWA capabilities
- **Performance Optimized**: Lazy loading and efficient animations

### Interactive Elements
- **Animated Counters**: Statistics with counting animations
- **Skill Level Bars**: Visual representation of your skills
- **Project Showcase**: Hover effects and overlay interactions
- **Contact Form**: Form validation and submission handling
- **Page Counter**: Track website visits
- **Smooth Scrolling**: Enhanced navigation experience

### Content Sections
- **Hero Section**: Eye-catching introduction with call-to-action
- **About Section**: Personal story and background
- **Skills Section**: Technical skills with progress bars
- **Projects Section**: Portfolio showcase with live links
- **Experience Section**: Timeline of your career
- **Contact Section**: Contact form and social links

## 🚀 Getting Started

### Prerequisites
- A modern web browser
- Basic knowledge of HTML, CSS, and JavaScript (for customization)

### Installation

1. **Clone or Download**
   ```bash
   git clone https://github.com/yourusername/portfolio-website.git
   cd portfolio-website
   ```

2. **Open in Browser**
   - Simply open `index.html` in your web browser
   - Or use a local server for better development experience

3. **Local Development Server** (Optional)
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   
   # Using PHP
   php -S localhost:8000
   ```

## 📝 Customization Guide

### Personal Information

#### 1. Update Personal Details
Edit the following in `index.html`:

```html
<!-- Hero Section -->
<h1 class="hero-title">
    Hi, I'm <span class="highlight">Karthikeyan Danasagaran</span>
</h1>
<h2 class="hero-subtitle">Mechanical Engineer</h2>

<!-- Contact Information -->
<div class="contact-item">
    <i class="fas fa-envelope"></i>
    <span>karthikeyan.danasagaran@example.com</span>
</div>
<div class="contact-item">
    <i class="fas fa-phone"></i>
    <span>+1 (555) 123-4567</span>
</div>
```

#### 2. Update Statistics
Modify the hero section statistics:

```html
<div class="hero-stats">
    <div class="stat">
        <span class="stat-number" data-target="50">0</span>
        <span class="stat-label">Projects</span>
    </div>
    <!-- Add more stats as needed -->
</div>
```

#### 3. Update Skills
Edit the skills section in `index.html`:

```html
<div class="skill-item" data-skill="AutoCAD">
    <i class="fas fa-drafting-compass"></i>
    <span>AutoCAD</span>
    <div class="skill-level" data-level="95"></div>
</div>
```

### Projects Section

#### 1. Add Your Projects
Replace the placeholder projects with your own:

```html
<article class="project-card">
    <div class="project-image">
        <img src="path/to/your/project-image.jpg" alt="Project Name">
        <div class="project-overlay">
            <div class="project-links">
                <a href="https://your-project.com" class="project-link">
                    <i class="fas fa-external-link-alt"></i>
                </a>
                <a href="https://github.com/yourusername/project" class="project-link">
                    <i class="fab fa-github"></i>
                </a>
            </div>
        </div>
    </div>
    <div class="project-content">
        <h3>Your Project Name</h3>
        <p>Project description goes here...</p>
        <div class="project-tech">
            <span class="tech-tag">SolidWorks</span>
            <span class="tech-tag">ANSYS</span>
        </div>
    </div>
</article>
```

### Experience Section

#### 1. Update Work Experience
Modify the timeline items:

```html
<div class="timeline-item">
    <div class="timeline-content">
        <div class="timeline-date">2023 - Present</div>
        <h3>Your Job Title</h3>
        <h4>Company Name</h4>
        <p>Job description...</p>
        <ul>
            <li>Achievement 1</li>
            <li>Achievement 2</li>
        </ul>
    </div>
</div>
```

### Styling Customization

#### 1. Color Scheme
Update CSS custom properties in `styles.css`:

```css
:root {
    --primary-color: #4F46E5;    /* Main brand color */
    --secondary-color: #10B981;  /* Secondary color */
    --accent-color: #F59E0B;     /* Accent color */
    /* Add more colors as needed */
}
```

#### 2. Typography
Change fonts in `styles.css`:

```css
:root {
    --font-family: 'Your-Font', -apple-system, BlinkMacSystemFont, sans-serif;
}
```

#### 3. Animations
Customize animation speeds:

```css
:root {
    --transition-fast: 0.15s ease;
    --transition-normal: 0.3s ease;
    --transition-slow: 0.5s ease;
}
```

### Images and Assets

#### 1. Profile Photo
Replace the placeholder image:
```html
<img src="path/to/your-photo.jpg" alt="Karthikeyan Danasagaran" class="profile-img">
```

#### 2. Project Images
Update project screenshots:
```html
<img src="path/to/project-screenshot.jpg" alt="Project Name">
```

#### 3. Favicon
Replace `favicon.ico` with your own icon.

## 🎨 Advanced Customization

### Adding New Sections

1. **Create the HTML structure** in `index.html`
2. **Add CSS styles** in `styles.css`
3. **Add JavaScript functionality** in `script.js` if needed
4. **Update navigation** to include the new section

### Custom Animations

Add new CSS animations:

```css
@keyframes yourAnimation {
    0% { /* initial state */ }
    100% { /* final state */ }
}

.your-element {
    animation: yourAnimation 1s ease;
}
```

### Form Integration

The contact form is currently set up for demonstration. To make it functional:

1. **Backend Integration**: Connect to a server-side solution
2. **Email Service**: Use services like EmailJS, Formspree, or Netlify Forms
3. **Validation**: Enhance form validation as needed

## 📱 PWA Features

### Service Worker
The website is ready for PWA features. To enable:

1. Create a `sw.js` file
2. Add a web app manifest
3. Configure offline functionality

### Manifest Example
Create `manifest.json`:

```json
{
    "name": "Karthikeyan Danasagaran - Mechanical Engineer Portfolio",
    "short_name": "Karthikeyan Portfolio",
    "description": "Mechanical Engineer Portfolio",
    "start_url": "/",
    "display": "standalone",
    "background_color": "#ffffff",
    "theme_color": "#4F46E5",
    "icons": [
        {
            "src": "icon-192.png",
            "sizes": "192x192",
            "type": "image/png"
        }
    ]
}
```

## 🚀 Deployment

### GitHub Pages
1. Push your code to GitHub
2. Go to repository settings
3. Enable GitHub Pages
4. Select source branch

### Netlify
1. Connect your GitHub repository
2. Deploy automatically
3. Configure custom domain (optional)

### Vercel
1. Import your repository
2. Deploy with one click
3. Get automatic deployments

## 🔧 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## 📊 Performance

The website is optimized for:
- Fast loading times
- Smooth animations
- Mobile performance
- SEO best practices

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Font Awesome for icons
- Google Fonts for typography
- Modern CSS techniques and best practices

## 📞 Support

If you need help customizing your portfolio:
- Check the customization guide above
- Review the code comments
- Open an issue for bugs
- Contact for custom development

---

**Happy engineering! 🚀**

Karthikeyan Danasagaran's portfolio website is now ready to showcase your amazing mechanical engineering work and help you land your dream job!