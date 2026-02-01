# Personal Portfolio Website

A modern, sophisticated personal portfolio website with a dark editorial aesthetic. Built with HTML, CSS, and vanilla JavaScript.

## Features

- 🎨 **Distinctive Design**: Editorial-style dark theme with elegant typography
- 📱 **Fully Responsive**: Optimized for all screen sizes
- ✨ **Smooth Animations**: Fade-in effects, hover interactions, and parallax scrolling
- 🎯 **Clean Code**: Semantic HTML5, modern CSS, and vanilla JavaScript
- 🚀 **GitHub Pages Ready**: Easy deployment to GitHub Pages

## Sections

- **Hero**: Eye-catching introduction with animated text
- **About**: Personal introduction with skills and statistics
- **Work**: Project showcase with hover effects
- **Contact**: Contact form and social links
- **Footer**: Professional footer with branding

## Customization Guide

### 1. Personal Information

Edit `index.html` to update:
- **Navigation Logo**: Change "YN" to your initials (line 19)
- **Hero Section**: Update your name and title (lines 42-46)
- **About Section**: Customize your bio and skills (lines 61-128)
- **Projects**: Replace with your own projects (lines 138-255)
- **Contact Details**: Update email, phone, and location (lines 271-284)
- **Social Links**: Add your GitHub, LinkedIn, Twitter, etc. (lines 286-291)
- **Footer**: Update your name (line 323)

### 2. Colors and Styling

Edit `style.css` to customize the color scheme:

```css
:root {
    --color-bg: #0a0a0a;              /* Main background */
    --color-bg-secondary: #151515;     /* Secondary background */
    --color-text: #e8e8e8;             /* Main text color */
    --color-text-secondary: #a0a0a0;   /* Secondary text */
    --color-accent: #c9a961;           /* Accent color (gold) */
    --color-accent-hover: #d4b976;     /* Accent hover state */
    --color-border: #2a2a2a;           /* Border color */
}
```

### 3. Add Your Images

Replace the placeholder elements with your images:

**Profile Image** (line 116-119 in index.html):
```html
<div class="image-placeholder">
    <img src="your-photo.jpg" alt="Your Name" style="width: 100%; height: 100%; object-fit: cover;">
</div>
```

**Project Images** (replace `.project-placeholder` divs):
```html
<div class="project-placeholder">
    <img src="project-image.jpg" alt="Project Name" style="width: 100%; height: 100%; object-fit: cover;">
</div>
```

### 4. Contact Form Setup

The contact form currently shows an alert. To make it functional, you can:

**Option 1: Formspree (Recommended)**
1. Sign up at [Formspree](https://formspree.io/)
2. Update the form in `index.html`:
```html
<form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

**Option 2: Netlify Forms**
Add `netlify` attribute to the form tag:
```html
<form class="contact-form" name="contact" method="POST" netlify>
```

**Option 3: EmailJS**
Follow the [EmailJS documentation](https://www.emailjs.com/docs/) to integrate email sending.

## GitHub Pages Deployment

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right and select "New repository"
3. Name it `username.github.io` (replace `username` with your GitHub username)
4. Make it public
5. Click "Create repository"

### Step 2: Upload Your Files

**Method A: Using GitHub Web Interface**
1. Click "uploading an existing file"
2. Drag and drop all files (`index.html`, `style.css`, `script.js`)
3. Click "Commit changes"

**Method B: Using Git Command Line**
```bash
# Navigate to your project folder
cd path/to/your/portfolio

# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit: Personal portfolio website"

# Add GitHub repository as remote
git remote add origin https://github.com/username/username.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings"
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select "main" branch
5. Click "Save"
6. Your site will be live at `https://username.github.io` in a few minutes!

## File Structure

```
portfolio/
│
├── index.html          # Main HTML file
├── style.css           # Stylesheet
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Performance Tips

1. **Optimize Images**: 
   - Use WebP format for smaller file sizes
   - Compress images using tools like TinyPNG
   - Recommended sizes: Profile (800x1000px), Projects (1600x1000px)

2. **Lazy Loading**: Add `loading="lazy"` to images:
```html
<img src="image.jpg" alt="Description" loading="lazy">
```

3. **Minify CSS/JS**: Use tools like [CSS Minifier](https://cssminifier.com/) before deployment

## Customization Ideas

- Add a blog section
- Include a resume/CV download
- Add a dark/light mode toggle
- Include testimonials section
- Add project case studies
- Integrate Google Analytics
- Add a custom domain

## Support

If you encounter any issues:
1. Check the browser console for errors
2. Ensure all file paths are correct
3. Verify GitHub Pages is enabled in repository settings

## License

Free to use for personal and commercial projects.

## Credits

- Fonts: [Google Fonts](https://fonts.google.com/) (Playfair Display, DM Sans)
- Icons: Update with your preferred icon library (Font Awesome, Feather Icons, etc.)

---

**Pro Tips:**
- Keep your content concise and impactful
- Update your portfolio regularly with new projects
- Use high-quality images
- Test on multiple devices before deploying
- Consider adding animations sparingly for better performance

Good luck with your portfolio! 🚀
