# 🏰 RSS Royal Biryani - Premium Restaurant Website

A modern, responsive, and SEO-optimized website for **RSS Royal Biryani**, an authentic dum biryani restaurant in Vizag (Visakhapatnam), India.

## 🌟 Features

### Design
- **Premium Dark Theme** - Black/deep brown background with gold and red accents
- **Responsive Design** - Mobile-first approach with breakpoints for tablets and desktops
- **Smooth Animations** - Elegant transitions and scroll effects
- **Modern Typography** - Professional serif headings with clean sans-serif body text

### Pages
1. **Home** - Hero section with CTA buttons, features showcase, and quick menu preview
2. **Menu** - Detailed menu items with high-quality food images and descriptions
3. **Contact** - Location info, contact form, business hours, social media links, and embedded map

### SEO Optimization
✅ **Meta Tags** - Descriptive titles and meta descriptions for each page
✅ **Keywords** - Natural inclusion of: "best biryani in Vizag", "non veg restaurant Vizag", "chicken biryani Vizag"
✅ **Semantic HTML** - Proper heading hierarchy and semantic structure
✅ **Mobile Responsive** - Google Mobile-Friendly design
✅ **Fast Loading** - Optimized images and minimal dependencies
✅ **Accessibility** - ARIA labels and keyboard navigation support

### Functionality
- **Mobile Menu** - Hamburger navigation for mobile devices
- **Form Validation** - Contact form with email and phone validation
- **Smooth Scrolling** - Elegant page transitions
- **Scroll Animations** - Elements fade in as they come into view
- **Interactive Buttons** - Ripple effect on button clicks
- **Notifications** - Success/error messages for form submissions

## 📁 File Structure

```
RSS-Royal-Biryani/
├── index.html          # Home page
├── menu.html           # Menu page
├── contact.html        # Contact page
├── style.css           # Main stylesheet (responsive design)
├── script.js           # JavaScript for interactivity
└── README.md           # This file
```

## 🚀 Getting Started

### Option 1: Open Locally
1. Download all files to your computer
2. Make sure all files are in the same folder
3. Open `index.html` in your web browser

### Option 2: Host Online
1. Upload all files to a web hosting service
2. Make sure `index.html` is the default/index file
3. Update the site URL with your domain name

## 🎨 Customization

### Update Contact Information
Edit the following in all HTML files:

**In Navigation and Footer:**
- Replace `+91 XXXX XXXX XX` with actual phone number
- Replace `info@royalbiryani.com` with actual email
- Update `Vizag, Visakhapatnam` with specific address

**In contact.html:**
- Update the phone link: `href="tel:+91XXXXXXXXXX"`
- Update the embedded Google Map iframe with your location coordinates

### Update Social Media Links
Replace the `#` placeholders with actual social media URLs:

```html
<a href="https://www.facebook.com/yourpage" target="_blank">
    <i class="fab fa-facebook"></i>
</a>
```

### Change Colors
Edit the CSS variables in `style.css`:

```css
:root {
    --color-primary: #d4af37;      /* Gold */
    --color-secondary: #c41e3a;    /* Red */
    --color-dark: #1a1a1a;         /* Very Dark */
    --color-darker: #0a0a0a;       /* Black */
}
```

### Replace Images
The website uses images from Unsplash (placeholder). To use your own images:

1. Place your images in an `assets/images/` folder
2. Replace the `src` URLs in HTML files:

```html
<!-- Before -->
<img src="https://images.unsplash.com/..." alt="Chicken Dum Biryani">

<!-- After -->
<img src="assets/images/biryani.jpg" alt="Chicken Dum Biryani">
```

### Update Menu Items
Add or modify menu items in `menu.html`:

```html
<div class="menu-item">
    <div class="menu-item-image">
        <img src="your-image.jpg" alt="Item Name">
    </div>
    <div class="menu-item-content">
        <h3>Item Name</h3>
        <p class="menu-description">Your description here</p>
        <div class="menu-meta">
            <span class="menu-tag">TAG</span>
            <span class="menu-price">₹XXX</span>
        </div>
    </div>
</div>
```

## 📱 Responsive Breakpoints

- **Desktop** - 1200px and above
- **Tablet** - 768px to 1199px
- **Mobile** - Below 768px

## 🔍 SEO Tips

1. **Update Meta Descriptions** - Edit the meta description in each page's `<head>` section
2. **Add Google Analytics** - Add tracking code to `<head>` section
3. **Create sitemap.xml** - List all pages for search engines
4. **robots.txt** - File to guide search engine crawlers
5. **Local Business Schema** - Add JSON-LD schema for local business
6. **Mobile Optimization** - Already implemented with responsive design

### Add Google Analytics

Add this to the `<head>` section of all pages:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR_TRACKING_ID"></script>
<script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'YOUR_TRACKING_ID');
</script>
```

## 🔧 Form Submission

The contact form currently shows a success message but doesn't send emails. To enable email functionality:

### Option 1: Using FormSubmit (Free Service)
1. Go to [formsubmit.co](https://formsubmit.co)
2. Replace the form action in `contact.html`:

```html
<form action="https://formsubmit.co/your-email@example.com" method="POST">
    <!-- form fields -->
</form>
```

### Option 2: Using Backend Service
Modify `script.js` to send data to your server:

```javascript
// In contactForm submit handler
fetch('/api/contact', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(data)
})
.then(response => response.json())
.then(data => showNotification('Email sent successfully!', 'success'));
```

## 📊 Performance Optimization

✅ **Optimized CSS** - Single stylesheet with minification potential
✅ **Lightweight JavaScript** - No jQuery or heavy frameworks
✅ **Image Optimization** - Use compressed images or WebP format
✅ **Lazy Loading** - Images load as they come into view
✅ **Caching** - Browser caching headers can be configured on server

### Further Optimization:
1. Minify CSS and JavaScript
2. Use CDN for Font Awesome icons
3. Compress images to WebP format
4. Enable Gzip compression on server
5. Use service workers for offline capability

## 🌐 Hosting Recommendations

- **Affordable**: Netlify, Vercel, GitHub Pages (free)
- **Standard**: Bluehost, HostGator, SiteGround
- **Premium**: AWS, Google Cloud, Azure
- **India-specific**: Hostinger India, GoDaddy India, BigRock

## 🔐 Security

- Use HTTPS on your domain
- Keep backups of all files
- Validate and sanitize form inputs
- Use strong passwords for hosting accounts
- Regularly update any backend scripts

## 📞 Contact Form Features

- **Validation** - Email and phone number validation
- **Notifications** - Success and error messages
- **Subject Options** - Order, Inquiry, Feedback, Catering, Other
- **Accessibility** - Keyboard navigation and screen reader support

## 🎯 Local SEO Checklist

- [ ] Google Business Profile created and verified
- [ ] Phone number displayed consistently
- [ ] Physical address included
- [ ] Schema markup added for local business
- [ ] Keywords naturally included (biryani Vizag, restaurant near me, etc.)
- [ ] Mobile-friendly design verified
- [ ] Page load speed optimized
- [ ] Backlinks from local directories
- [ ] Customer reviews encouraged
- [ ] Local keywords in meta descriptions

## 📈 Next Steps

1. **Test** - Check all links and functionality
2. **Customize** - Update with your actual business info and images
3. **Launch** - Deploy to your web hosting
4. **Promote** - Share on social media and local directories
5. **Monitor** - Track analytics and user behavior
6. **Update** - Keep menu and information current

## 🎓 Learning Resources

- [MDN Web Docs](https://developer.mozilla.org)
- [Google Search Console](https://search.google.com/search-console)
- [Google My Business](https://www.google.com/business/)
- [SEO Best Practices](https://developers.google.com/search)

## 📝 License

This website template is free to use and modify for your restaurant. No attribution required.

## 💡 Support & Tips

**For Better Results:**
1. Use high-quality, professional food photography
2. Keep content fresh and updated
3. Encourage customer reviews
4. Post regularly on social media
5. Engage with your local community online
6. Use local keywords in all content
7. Maintain consistent branding

---

**Created with ❤️ for RSS Royal Biryani - Your authentic dum biryani destination in Vizag!**

*Last Updated: 2026*
