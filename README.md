# Parenting Life - Lifestyle Blog Website

A beautiful, modern website for sharing parenting tips, retreat ideas, and curated resources. Built with HTML, CSS, and JavaScript.

## 🌟 Features

- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Modern UI**: Clean, beautiful design with smooth animations
- **Interactive Elements**: Hover effects, smooth scrolling, and form handling
- **Mobile Navigation**: Hamburger menu for mobile devices
- **Search Functionality**: Built-in search bar (ready for expansion)
- **Newsletter Signup**: Forms for retreat updates and newsletter subscription
- **Back to Top Button**: Easy navigation back to the top of the page

## 📁 File Structure

```
parenting-lifestyle-blog/
├── index.html          # Main HTML file
├── styles.css          # CSS styles and responsive design
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## 🚀 Getting Started

1. **Open the website**: Simply open `index.html` in your web browser
2. **Local development**: You can use any local server or just open the file directly
3. **Deploy**: Upload all files to any web hosting service

## 🎨 Customization Guide

### Colors
The website uses a warm, parenting-friendly color palette:
- Primary: `#ff6b6b` (coral pink)
- Secondary: `#ff8e8e` (lighter coral)
- Background gradients: Various soft pastels

To change colors, edit the CSS variables in `styles.css`:
```css
/* Main brand colors */
--primary-color: #ff6b6b;
--secondary-color: #ff8e8e;
```

### Content Sections

#### 1. Hero Section
- **Location**: Top of the page
- **Customize**: Edit the title, subtitle, and stats in `index.html`
- **Stats**: Update the numbers and labels to reflect your actual content

#### 2. Parenting Tips
- **Add new tips**: Copy the `tip-card` structure in `index.html`
- **Icons**: Use Font Awesome icons (already included)
- **Tags**: Add relevant tags for categorization

#### 3. Retreats Section
- **Vision**: Update the retreat description and features
- **Signup form**: Currently logs to console - can be connected to email service
- **Background**: Customize the gradient background in CSS

#### 4. Resources
- **Categories**: Three main categories (People, Products, Places)
- **Add links**: Replace `#` with actual URLs
- **Descriptions**: Update descriptions for each resource

#### 5. Recipes
- **Add recipes**: Copy the `recipe-card` structure
- **Icons**: Use food-related Font Awesome icons
- **Meta info**: Update cooking time and tags

### Adding New Content

#### New Parenting Tip
```html
<article class="tip-card">
    <div class="tip-icon">
        <i class="fas fa-[icon-name]"></i>
    </div>
    <h3>Your Tip Title</h3>
    <p>Your tip description goes here.</p>
    <div class="tip-tags">
        <span class="tag">Category</span>
        <span class="tag">Age Group</span>
    </div>
</article>
```

#### New Recipe
```html
<article class="recipe-card">
    <div class="recipe-image">
        <i class="fas fa-[food-icon]"></i>
    </div>
    <div class="recipe-content">
        <h3>Recipe Name</h3>
        <p>Recipe description.</p>
        <div class="recipe-meta">
            <span><i class="fas fa-clock"></i> Prep Time</span>
            <span><i class="fas fa-star"></i> Kid Favorite</span>
        </div>
    </div>
</article>
```

#### New Resource
```html
<a href="[URL]" class="resource-link">
    <span class="resource-name">Resource Name</span>
    <span class="resource-desc">Resource description</span>
</a>
```

## 🔧 Technical Features

### JavaScript Functionality
- **Mobile menu toggle**
- **Smooth scrolling navigation**
- **Form handling with success messages**
- **Intersection Observer for animations**
- **Counter animations in hero section**
- **Touch/swipe support for mobile**
- **Performance optimizations**

### CSS Features
- **CSS Grid and Flexbox layouts**
- **CSS animations and transitions**
- **Responsive breakpoints**
- **Custom scrollbar styling**
- **Backdrop filter effects**

## 📱 Responsive Breakpoints

- **Desktop**: 1200px and above
- **Tablet**: 768px - 1199px
- **Mobile**: Below 768px
- **Small Mobile**: Below 480px

## 🎯 SEO and Performance

### Meta Tags to Add
Add these to the `<head>` section in `index.html`:
```html
<meta name="description" content="Parenting tips, retreats, and resources for modern parents">
<meta name="keywords" content="parenting, tips, retreats, recipes, resources">
<meta name="author" content="Your Name">
<meta property="og:title" content="Parenting Life - Tips, Retreats & Resources">
<meta property="og:description" content="A collection of parenting wisdom and resources">
<meta property="og:type" content="website">
```

### Performance Tips
- Images are optimized with Font Awesome icons
- CSS and JS are minified-ready
- Lazy loading can be added for images
- CDN links for fonts and icons

## 🔗 External Dependencies

- **Font Awesome**: Icons (loaded via CDN)
- **Google Fonts**: Inter font family (loaded via CDN)

## 📧 Form Integration

The website includes two forms:
1. **Retreat signup** (in retreats section)
2. **Newsletter signup** (in footer)

To connect these to actual email services:

### Option 1: EmailJS
```javascript
// Add EmailJS script
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>

// Initialize
emailjs.init("YOUR_USER_ID");

// Send email
emailjs.send("YOUR_SERVICE_ID", "YOUR_TEMPLATE_ID", {
    to_email: "your@email.com",
    from_email: userEmail,
    message: "New signup from website"
});
```

### Option 2: Netlify Forms
Add `netlify` attribute to forms:
```html
<form class="signup-form" netlify>
```

### Option 3: Custom Backend
Replace the form handlers in `script.js` with your API calls.

## 🚀 Deployment Options

### GitHub Pages
1. Create a GitHub repository
2. Upload all files
3. Enable GitHub Pages in repository settings

### Netlify
1. Drag and drop the folder to Netlify
2. Or connect your GitHub repository

### Vercel
1. Install Vercel CLI
2. Run `vercel` in the project directory

### Traditional Hosting
Upload all files to your web hosting service via FTP.

## 🎨 Design Inspiration

The design focuses on:
- **Warm, welcoming colors** suitable for parenting content
- **Clean typography** using Inter font
- **Card-based layout** for easy content organization
- **Smooth animations** for better user experience
- **Mobile-first approach** for accessibility

## 🔄 Future Enhancements

Potential features to add:
- **Blog post system** with individual pages
- **Comment system** for community engagement
- **Recipe calculator** for different serving sizes
- **Age-based filtering** for parenting tips
- **Email newsletter integration**
- **Social media sharing buttons**
- **Dark mode toggle**
- **Multi-language support**

## 📞 Support

This is a static website built with vanilla HTML, CSS, and JavaScript. No build process or dependencies required. Simply edit the files and refresh your browser to see changes.

## 📄 License

This project is open source and available under the MIT License.

---

**Happy parenting! 🌸** 