# Supun Wijekoon - Portfolio Website

A modern, responsive portfolio website showcasing professional experience, projects, skills, and research publications.

## Features

- **Modern Design**: Clean, professional design with smooth animations
- **Responsive Layout**: Fully responsive across all devices
- **Interactive Elements**: Hover effects, smooth scrolling, and animations
- **Professional Sections**:
  - Hero section with introduction
  - About section with statistics
  - Professional experience timeline
  - Education history
  - Skills and technologies
  - Featured projects
  - Research publications
  - Contact form

## Technologies Used

- HTML5
- CSS3 (with modern features like Grid, Flexbox, and CSS Variables)
- Vanilla JavaScript
- Font Awesome Icons
- Google Fonts (Inter)

## File Structure

```
Portfolio/
├── index.html          # Main HTML file
├── styles.css          # CSS styles
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## Customization Guide

### Personal Information

1. **Update Personal Details** in `index.html`:
   - Name and title in the hero section
   - About section content
   - Contact information
   - Social media links

2. **Update Experience** in the Experience section:
   - Job titles, companies, and durations
   - Skills used in each role
   - Job descriptions

3. **Update Education** in the Education section:
   - Degrees, institutions, and dates
   - Descriptions of studies

### Skills Section

The skills are organized into categories. Update the skills in `index.html`:

```html
<div class="skill-category">
    <h3>Programming Languages</h3>
    <div class="skill-items">
        <div class="skill-item">JavaScript</div>
        <div class="skill-item">Python</div>
        <!-- Add more skills -->
    </div>
</div>
```

### Projects Section

Update the projects in `index.html`:

```html
<div class="project-card">
    <div class="project-image">
        <i class="fas fa-university"></i> <!-- Change icon -->
    </div>
    <div class="project-content">
        <h3>Project Name</h3>
        <p>Project description...</p>
        <div class="project-tech">
            <span>Technology 1</span>
            <span>Technology 2</span>
        </div>
        <div class="project-links">
            <a href="#" class="project-link">View Details</a>
        </div>
    </div>
</div>
```

### Research Publications

Update the research section with your publications:

```html
<div class="publication-card">
    <div class="publication-header">
        <h3>Publication Title</h3>
        <span class="publication-date">Publication Date</span>
    </div>
    <div class="publication-journal">
        <strong>Journal:</strong> Journal Name
    </div>
    <div class="publication-abstract">
        <h4>Abstract</h4>
        <p>Abstract content...</p>
    </div>
    <div class="publication-keywords">
        <strong>Keywords:</strong>
        <span class="keyword">Keyword 1</span>
        <span class="keyword">Keyword 2</span>
    </div>
    <div class="publication-links">
        <a href="publication-url" target="_blank" class="btn btn-primary">
            <i class="fas fa-external-link-alt"></i> View Publication
        </a>
    </div>
</div>
```

### Styling Customization

#### Colors
The main color scheme can be customized in `styles.css`:

```css
:root {
    --primary-color: #2563eb;
    --secondary-color: #fbbf24;
    --text-color: #1f2937;
    --light-bg: #f8fafc;
    --border-color: #e2e8f0;
}
```

#### Fonts
Change the font by updating the Google Fonts link in `index.html`:

```html
<link href="https://fonts.googleapis.com/css2?family=YourFont:wght@300;400;500;600;700&display=swap" rel="stylesheet">
```

Then update the font-family in `styles.css`:

```css
body {
    font-family: 'YourFont', sans-serif;
}
```

## Deployment

### GitHub Pages
1. Push your code to a GitHub repository
2. Go to repository Settings > Pages
3. Select source branch (usually `main`)
4. Your site will be available at `https://username.github.io/repository-name`

### Netlify
1. Drag and drop your project folder to [Netlify](https://netlify.com)
2. Your site will be deployed instantly
3. You can set up custom domain if needed

### Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in your project directory
3. Follow the prompts to deploy

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Performance Features

- Optimized images and icons
- Minimal JavaScript
- CSS animations for smooth performance
- Responsive images
- Lazy loading for better performance

## SEO Optimization

The portfolio includes:
- Semantic HTML structure
- Meta tags for social sharing
- Proper heading hierarchy
- Alt text for images
- Fast loading times

## Contact Form

The contact form is currently set up to show a success message. To make it functional:

1. **EmailJS**: Use EmailJS service
2. **Netlify Forms**: If deploying on Netlify
3. **Custom Backend**: Create your own backend API

Example with EmailJS:
```javascript
// Add EmailJS script to HTML
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>

// Initialize EmailJS
emailjs.init("YOUR_USER_ID");

// Update form submission in script.js
emailjs.send("YOUR_SERVICE_ID", "YOUR_TEMPLATE_ID", {
    name: name,
    email: email,
    subject: subject,
    message: message
});
```

## License

This project is open source and available under the [MIT License](LICENSE).

## Support

If you need help customizing this portfolio, feel free to:
- Check the code comments for guidance
- Modify the CSS variables for easy customization
- Update the JavaScript for additional functionality

## Credits

- Icons: [Font Awesome](https://fontawesome.com/)
- Fonts: [Google Fonts](https://fonts.google.com/)
- Design inspiration: Modern web design principles
