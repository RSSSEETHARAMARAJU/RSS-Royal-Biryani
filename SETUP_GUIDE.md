# 📚 Website Setup & Usage Guide

## Quick Start

1. **Open in Browser**: Double-click `index.html` to preview locally
2. **Test All Pages**: Click through all three pages (Home, Menu, Contact)
3. **Test Mobile**: Right-click → Inspect → Toggle Device Toolbar (Ctrl+Shift+M)
4. **Customize**: Edit HTML files with your actual information
5. **Deploy**: Upload to web hosting

## 🔄 Workflow

### Phase 1: Customization (Before Launch)
- [ ] Replace all placeholder phone numbers
- [ ] Update email address
- [ ] Add specific location in Vizag
- [ ] Change social media links to your accounts
- [ ] Replace placeholder images with restaurant photos
- [ ] Update menu items and prices

### Phase 2: Launch
- [ ] Choose web hosting provider
- [ ] Register domain (optional but recommended)
- [ ] Upload files via FTP/control panel
- [ ] Test all functionality
- [ ] Set up Google Analytics
- [ ] Submit to Google Search Console

### Phase 3: Promotion
- [ ] Share on social media
- [ ] List on Google Business Profile
- [ ] Add to local directories (Zomato, Swiggy, etc.)
- [ ] Collect customer reviews
- [ ] Post regular content on social media

## 🖼️ Image Recommendations

### Hero Image (Homepage)
- High-quality photo of your best biryani dish
- Size: 1200x800px minimum
- Format: JPG or WebP
- File size: <500KB

### Menu Item Images
- Professional food photography
- Size: 400x400px
- Format: JPG or WebP
- File size: <200KB each

### Tips for Better Images:
- Use natural lighting
- Shoot from above at 45° angle
- Include garnishes and fresh ingredients
- Keep background simple and dark
- Resize and compress before uploading

## 🔗 Important Links to Update

### Phone Numbers
Find and replace `+91 XXXX XXXX XX` with your actual number in:
- `index.html` (footer)
- `menu.html` (footer)
- `contact.html` (info card, button link)

### Email
Replace `info@royalbiryani.com` with your actual email:
- All three HTML files (footer)
- `contact.html` (info card)

### Address
Replace `Vizag, Visakhapatnam` with your exact location:
- All three HTML files (footer)
- `contact.html` (info card, map, page title)

### Social Media
Replace `#` links with your actual profiles:

```html
<!-- Facebook -->
<a href="https://www.facebook.com/yourpage" target="_blank">

<!-- Instagram -->
<a href="https://www.instagram.com/yourprofile" target="_blank">

<!-- Twitter -->
<a href="https://www.twitter.com/yourhandle" target="_blank">

<!-- WhatsApp -->
<a href="https://wa.me/91XXXXXXXXXX" target="_blank">
```

## 🧪 Testing Checklist

### Functionality
- [ ] Home page loads correctly
- [ ] Menu page displays all items
- [ ] Contact form validation works
- [ ] "Order Now" buttons link correctly
- [ ] All images load
- [ ] Mobile menu opens/closes
- [ ] Scroll animations work smoothly

### Responsive Design
- [ ] Desktop view (1920x1080)
- [ ] Tablet view (768x1024)
- [ ] Mobile view (375x667)
- [ ] All text is readable
- [ ] Images scale properly
- [ ] Menu collapses on mobile
- [ ] Forms are accessible on mobile

### Performance
- [ ] Pages load within 3 seconds
- [ ] Images are optimized
- [ ] No console errors
- [ ] Smooth scrolling works

### SEO
- [ ] Page titles are unique
- [ ] Meta descriptions are present
- [ ] Keywords are naturally included
- [ ] Heading hierarchy is correct (H1 > H2 > H3)
- [ ] Internal links work
- [ ] Mobile friendly

### Accessibility
- [ ] Tab navigation works
- [ ] Buttons are clickable via keyboard
- [ ] Color contrast is sufficient
- [ ] Alt text on all images
- [ ] Form labels are associated

## 📱 Mobile Optimization Tips

1. **Test on Real Devices**
   - iPhone and Android phones
   - Different screen sizes
   - Slow internet connections

2. **Optimize Images**
   - Compress images to <100KB
   - Use responsive image sizes
   - Consider WebP format

3. **Improve Performance**
   - Minimize CSS/JavaScript
   - Remove unused code
   - Enable browser caching

## 🌐 SEO Best Practices Implemented

### ✅ On-Page SEO
- Unique meta descriptions
- Proper heading structure
- Semantic HTML5
- Keyword optimization
- Internal linking

### ✅ Technical SEO
- Mobile responsive
- Fast loading time
- Clean URL structure
- SSL ready
- Structured data ready

### ✅ Local SEO
- Location-specific keywords
- Business information
- Contact details
- Map integration
- Local business schema ready

### To Further Improve SEO:

1. **Add Schema Markup**
```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Restaurant",
  "name": "RSS Royal Biryani",
  "image": "image_url",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "Your address",
    "addressLocality": "Vizag",
    "postalCode": "530002",
    "addressCountry": "IN"
  },
  "telephone": "+91-XXXXXXXXXX"
}
</script>
```

2. **Create sitemap.xml**
```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://yourdomain.com/index.html</loc>
    <lastmod>2026-04-16</lastmod>
    <priority>1.0</priority>
  </url>
  <url>
    <loc>https://yourdomain.com/menu.html</loc>
    <lastmod>2026-04-16</lastmod>
    <priority>0.9</priority>
  </url>
  <url>
    <loc>https://yourdomain.com/contact.html</loc>
    <lastmod>2026-04-16</lastmod>
    <priority>0.9</priority>
  </url>
</urlset>
```

3. **Create robots.txt**
```
User-agent: *
Allow: /
Sitemap: https://yourdomain.com/sitemap.xml
```

## 💬 Contact Form Integration

The form currently shows success messages but doesn't send emails. Choose one:

### Option 1: Formspree (Recommended)
1. Go to [Formspree.io](https://formspree.io)
2. Create account and set up form
3. Add this to `contact.html`:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option 2: EmailJS (No Backend Needed)
1. Go to [EmailJS.com](https://www.emailjs.com)
2. Set up email service
3. Add JavaScript to `script.js`

### Option 3: Backend (Advanced)
Create a simple PHP/Node.js endpoint to handle form submissions

## 🎯 Marketing Strategy

### Social Media Content Ideas
1. **Weekly Specials** - Share limited-time offers
2. **Behind the Scenes** - Show food preparation
3. **Customer Testimonials** - Share customer reviews
4. **Food Photos** - High-quality biryani pictures
5. **Cooking Videos** - Short clips of preparation
6. **Events** - Announce special occasions/promotions
7. **Polls & Engagement** - Ask followers about preferences

### Local Marketing
1. **Google Business Profile** - Add complete information, photos, posts
2. **Food Delivery Apps** - List on Zomato, Swiggy, Uber Eats
3. **Local Directories** - JustDial, LocalOye, etc.
4. **Partnerships** - Collaborate with local businesses
5. **Events** - Sponsor local community events
6. **Offline Promotion** - Flyers, posters with QR code to website

## 📊 Analytics & Tracking

Add Google Analytics to track:
- Visitor traffic
- Popular pages
- User behavior
- Conversion rates
- Traffic sources

Find the unique ID at: [Google Analytics](https://analytics.google.com)

## 🔒 Security Tips

1. **Always use HTTPS** - Encrypts data
2. **Regular Backups** - Keep copies of all files
3. **Form Protection** - Add CAPTCHA if needed
4. **Keep Files Updated** - Update links periodically
5. **Monitor Website** - Check for errors regularly

## 🆘 Troubleshooting

### Issue: Mobile menu not working
- Check JavaScript is enabled
- Verify `script.js` is in same folder
- Clear browser cache (Ctrl+Shift+Delete)

### Issue: Images not loading
- Check image file paths are correct
- Verify image files exist
- Check file permissions on server

### Issue: Form not submitting
- Check form action URL
- Verify JavaScript is enabled
- Test in different browser

### Issue: Styling looks broken
- Check `style.css` is in same folder
- Clear browser cache
- Test in incognito window

## 📞 Next Steps

1. **Backup**
   - Create copies of all files
   - Store in cloud (Google Drive, Dropbox)

2. **Domain**
   - Consider registering a domain
   - Get SSL certificate

3. **Hosting**
   - Choose reliable hosting provider
   - Ensure good uptime history
   - Good customer support

4. **Email**
   - Set up business email
   - Professional email address

5. **Analytics**
   - Set up Google Analytics
   - Monitor website performance

6. **Maintenance**
   - Update content regularly
   - Respond to inquiries quickly
   - Monitor and fix errors

---

Good luck with your website! Remember:
✨ Keep content fresh
✨ Respond to customers quickly
✨ Post regularly on social media
✨ Encourage customer reviews
✨ Monitor and improve continuously

**Your success is our priority!**
