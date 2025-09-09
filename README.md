# Bhumi's 3D Art Portfolio

A minimalistic, dark-themed portfolio website showcasing 3D art across multiple genres.

## Features

- **Responsive Design**: Mobile-first approach with smooth transitions
- **Dark Theme**: Professional dark color scheme (#121212) with blue accents (#4A90E2)
- **Smooth Scrolling**: Enhanced navigation between sections
- **Form Validation**: Contact form with client-side validation
- **Accessibility**: WCAG AA compliant with keyboard navigation support
- **Performance Optimized**: Lightweight, fast-loading static site

## Structure

```
bhumi-portfolio/
├── index.html          # Main HTML file
├── styles.css          # All CSS styles
├── script.js           # JavaScript functionality
├── assets/
│   ├── portfolio/      # Portfolio images
│   │   ├── scifi-1.jpg
│   │   ├── fantasy-1.jpg
│   │   └── ...
│   ├── profile-photo.jpg
│   └── favicon.ico
└── README.md
```

## Sections

1. **Hero Section**: Name, tagline, and call-to-action buttons
2. **About Me**: Personal bio, skills, and profile photo
3. **Portfolio**: Organized by genres (Sci-Fi, Fantasy, Realistic, Abstract)
4. **Contact**: Contact form and social media links

## Customization

### Adding Portfolio Images
1. Add images to the `assets/portfolio/` folder
2. Update the `src` attributes in `index.html`
3. Optimize images for web (recommended: under 500KB each)

### Contact Form Setup
The contact form uses Formspree for handling submissions. To set it up:
1. Sign up at [Formspree.io](https://formspree.io)
2. Replace `your-form-id` in the form action with your actual Formspree form ID
3. The form will automatically handle submissions and send emails

### Color Scheme
The site uses CSS custom properties for easy color customization:
- Primary Background: `#121212`
- Secondary Background: `#1a1a1a`
- Text Color: `#FFFFFF`
- Accent Color: `#4A90E2`

## Deployment

This is a static website that can be deployed to:
- **GitHub Pages**: Push to a GitHub repository and enable Pages
- **Netlify**: Drag and drop the folder or connect to GitHub
- **Vercel**: Import from GitHub or upload files
- **Any web hosting service**: Upload files to the public folder

## Browser Support

- Chrome 60+
- Firefox 60+
- Safari 12+
- Edge 79+

## Performance

- Optimized for fast loading (target: under 2 seconds)
- Minimal JavaScript footprint
- Compressed CSS and optimized images
- Lazy loading for portfolio images

## Accessibility Features

- Semantic HTML structure
- ARIA labels for interactive elements
- Keyboard navigation support
- High contrast mode compatibility
- Screen reader friendly
- Skip links for better navigation

## License

This portfolio template is free to use and modify for personal projects.
