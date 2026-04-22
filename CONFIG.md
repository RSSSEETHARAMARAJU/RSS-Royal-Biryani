# ⚡ Quick Configuration Guide

## 🎯 Before You Launch - Update These Values

Use Find & Replace (Ctrl+H) in any text editor to quickly update these across all files.

---

## 📍 Location Information

### 1. Phone Number
**Find:** `+91 7981499951`
**Replace with:** Your actual phone number
**Format:** `+91 XXXXXXXXXX` (10 digits after +91)

**Also update:**
- In `contact.html`: `href="tel:+91XXXXXXXXXX"`

---

### 2. Email Address
**Find:** `info@royalbiryani.com`
**Replace with:** Your business email
**Example:** `contact@yourbiryaniplace.com`

---

### 3. Business Address
**Find:** `Vizag, Visakhapatnam`
**Replace with:** Your specific address
**Example:** `CSR Complex, Dwaraka Nagar, Vizag 530016`

---

### 4. Google Map Embedding
**In contact.html**, find and replace the iframe:

**Current:**
```html
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3842.7373801843757!2d83.22361!3d17.6930!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3a3e!5e0!3m2!1sen!2sin!4v1"
```

**Steps to get your map:**
1. Go to [Google Maps](https://maps.google.com)
2. Search your restaurant location
3. Click Share
4. Click "Embed a map"
5. Copy the iframe code
6. Replace in `contact.html`

---

## 🔗 Social Media Links

Update all instances in all HTML files:

### Facebook
**Find:** `href="#"` (in Facebook icon)
**Replace with:** `href="https://www.facebook.com/yourpagename"`

### Instagram
**Find:** `href="#"` (in Instagram icon)
**Replace with:** `href="https://www.instagram.com/yourusername"`

### Twitter
**Find:** `href="#"` (in Twitter icon)
**Replace with:** `href="https://twitter.com/yourhandle"`

### WhatsApp
**Find:** `href="#"` (in WhatsApp icon)
**Replace with:** `href="https://wa.me/91XXXXXXXXXX"`

---

## 🍽️ Menu Items

**In menu.html**, each item has this structure. Customize as needed:

```html
<div class="menu-item">
    <div class="menu-item-image">
        <img src="image-url" alt="Item Name">
    </div>
    <div class="menu-item-content">
        <h3>Item Name</h3>
        <p class="menu-description">Description here</p>
        <div class="menu-meta">
            <span class="menu-tag">TAG</span>
            <span class="menu-price">₹XXX</span>
        </div>
    </div>
</div>
```

**Update:**
- Item names
- Descriptions
- Prices (₹ symbol is already there)
- Image URLs
- Tags (Signature, Premium, etc.)

---

## 🖼️ Images to Replace

### Priority (High Impact):
1. Hero image (homepage) - `https://images.unsplash.com/photo-1454496522488-7a8e488e8606`
2. Menu item images (6 images on menu page)
3. Quick menu images (3 images on homepage)

### How to get your images:
1. Take professional photos of your food
2. Resize to recommended dimensions
3. Upload to your hosting or image service
4. Replace the URLs in HTML files

**Image Hosting Options (Free):**
- Cloudinary
- Imgur
- Unsplash (your own photos)
- Pexels (with permission)

---

## 📝 Meta Descriptions & Titles

### Homepage (index.html)
**Title:** Already optimized - contains "Best Biryani in Vizag"
**Meta Description:** Already optimized for SEO

### Menu Page (menu.html)
**Title:** Already optimized
**Meta Description:** Already optimized

### Contact Page (contact.html)
**Title:** Already optimized
**Meta Description:** Already optimized

---

## 🎨 Brand Colors (Optional)

If you want to change colors, edit `style.css`:

**Current Colors:**
- Gold: `#d4af37` (primary)
- Red: `#c41e3a` (secondary)
- Dark: `#1a1a1a` (background)
- Black: `#0a0a0a` (darker)

**To change:**
1. Open `style.css`
2. Find `:root {`
3. Update color codes
4. Example:
   ```css
   --color-primary: #FFD700;  /* Your gold */
   --color-secondary: #DC143C; /* Your red */
   ```

---

## 📊 Analytics Setup

### Google Analytics
**Step 1:** Go to [analytics.google.com](https://analytics.google.com)
**Step 2:** Create account, get Tracking ID
**Step 3:** Add to ALL HTML pages in `<head>`:

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

---

## ✉️ Contact Form Setup

### Option 1: Formspree (Easiest)
1. Go to [formspree.io](https://formspree.io)
2. Sign up and create form
3. In `contact.html`, find:
   ```html
   <form class="contact-form" id="contactForm">
   ```
4. Replace with:
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

### Option 2: Keep Current
- Current form shows success message
- Messages are logged to browser console
- Good for testing, needs backend for production

---

## 🚀 Quick Deployment Checklist

### Before uploading:
- [ ] Phone number updated
- [ ] Email added
- [ ] Address updated
- [ ] Social media links set
- [ ] Menu items customized
- [ ] Images added
- [ ] Analytics code added
- [ ] Form action set
- [ ] All links tested
- [ ] Mobile view checked

### Upload files:
1. All HTML files (`index.html`, `menu.html`, `contact.html`)
2. `style.css`
3. `script.js`
4. `README.md` (optional)

---

## 🔍 Test After Update

### Test These:
- [ ] Home page loads
- [ ] Menu page displays correctly
- [ ] Contact form works
- [ ] All images appear
- [ ] Mobile menu works
- [ ] Phone links work (tel:)
- [ ] Email links work (mailto:)
- [ ] Social media links work
- [ ] Scroll smooth
- [ ] No console errors

**Test in:**
- Chrome
- Firefox
- Safari
- Mobile browser

---

## 💾 File Checklist

**Must have:**
- ✅ index.html (Home)
- ✅ menu.html (Menu)
- ✅ contact.html (Contact)
- ✅ style.css (Styling)
- ✅ script.js (Interactivity)

**Optional:**
- ✅ README.md (Documentation)
- ✅ SETUP_GUIDE.md (Setup instructions)
- ✅ DEPLOYMENT.md (Deployment info)
- ✅ CONFIG.md (This file)

---

## 🎯 Most Important Updates

**DO THIS FIRST:**
1. Replace phone: `+91 XXXX XXXX XX` → Your number
2. Replace email: `info@royalbiryani.com` → Your email
3. Replace address: `Vizag, Visakhapatnam` → Your address
4. Add social media links
5. Replace hero image

**THEN:**
6. Update menu items
7. Replace all images
8. Add Google Analytics
9. Set up contact form
10. Deploy to hosting

---

## ⏱️ Update Time Estimate

| Task | Time |
|------|------|
| Replace contact info | 5 min |
| Update menu items | 10 min |
| Add images | 15 min |
| Update social links | 5 min |
| Add analytics | 3 min |
| Setup contact form | 5 min |
| **Total** | **~45 min** |

---

## 🆘 Common Issues & Fixes

### Issue: Images not showing
**Fix:** 
- Check image URLs are correct
- Make sure image files exist
- Try different image format (JPG vs PNG)

### Issue: Form not working
**Fix:**
- Check form action URL
- Verify JavaScript enabled
- Test in different browser

### Issue: Mobile menu broken
**Fix:**
- Clear browser cache (Ctrl+Shift+Delete)
- Verify `script.js` file uploaded
- Check for JavaScript errors

### Issue: Styling looks wrong
**Fix:**
- Check `style.css` is uploaded
- Clear browser cache
- Test in incognito window

---

## 📞 Quick Support

**Need help?**
1. Check README.md for detailed explanation
2. Check SETUP_GUIDE.md for step-by-step
3. Check DEPLOYMENT.md for deployment help
4. Google search the specific error
5. Check Stack Overflow

---

## 🎉 You're All Set!

Once you've completed these updates, your website is ready to launch!

**Next steps:**
1. Deploy to hosting
2. Set up Google Business Profile
3. Share on social media
4. Monitor analytics
5. Collect customer reviews

**Good luck! Your biryani restaurant deserves a great website!** 🍱

---

*Last updated: 2026-04-16*
