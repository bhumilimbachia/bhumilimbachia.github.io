# Deployment Guide

This portfolio website is a static site that can be deployed to various hosting platforms. Here are the most popular options:

## GitHub Pages (Free)

1. **Upload to GitHub:**
   - Create a new repository on GitHub
   - Upload all files to the repository
   - Make sure `index.html` is in the root directory

2. **Enable GitHub Pages:**
   - Go to repository Settings
   - Scroll down to "Pages" section
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click "Save"

3. **Access your site:**
   - Your site will be available at `https://yourusername.github.io/repository-name`
   - Custom domain can be configured in the Pages settings

## Netlify (Free tier available)

### Option 1: Drag & Drop
1. Go to [netlify.com](https://netlify.com)
2. Drag the entire project folder to the deployment area
3. Your site will be live with a random URL
4. You can change the site name in Site Settings

### Option 2: Git Integration
1. Push your code to GitHub, GitLab, or Bitbucket
2. Connect your repository to Netlify
3. Set build settings (leave empty for static sites)
4. Deploy automatically on every push

## Vercel (Free tier available)

1. Go to [vercel.com](https://vercel.com)
2. Import your GitHub repository
3. Configure project settings (defaults work for static sites)
4. Deploy with automatic HTTPS and global CDN

## Traditional Web Hosting

Upload all files to your web hosting provider's public folder (usually `public_html` or `www`).

## Pre-Deployment Checklist

- [ ] Replace placeholder images with actual artwork
- [ ] Update contact form action URL (if using Formspree)
- [ ] Update social media links
- [ ] Test all links and functionality
- [ ] Optimize images for web (under 500KB each)
- [ ] Update meta tags with actual domain URL
- [ ] Test on different devices and browsers

## Contact Form Setup

The contact form currently uses Formspree. To set it up:

1. Go to [formspree.io](https://formspree.io)
2. Sign up for a free account
3. Create a new form
4. Copy your form endpoint
5. Replace `your-form-id` in `index.html` with your actual form ID:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

## Custom Domain Setup

### For GitHub Pages:
1. Add a `CNAME` file with your domain name
2. Configure DNS with your domain provider
3. Enable HTTPS in repository settings

### For Netlify/Vercel:
1. Add domain in dashboard settings
2. Configure DNS records as instructed
3. SSL certificates are automatically provided

## Performance Optimization

- Images are already optimized for web
- CSS and JavaScript are minified for production
- Consider using a CDN for faster global loading
- Enable gzip compression on your server

## SEO Considerations

- Update the canonical URL in the HTML head
- Submit your sitemap to Google Search Console
- Ensure all images have descriptive alt text
- Test with Google's PageSpeed Insights

## Analytics (Optional)

Add Google Analytics or similar tracking:

```html
<!-- Add before closing </head> tag -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

Replace `GA_MEASUREMENT_ID` with your actual Google Analytics ID.
