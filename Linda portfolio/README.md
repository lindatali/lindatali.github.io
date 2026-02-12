# Linda Tali - Portfolio Website

Professional portfolio website for Linda Tali, Technical Program Manager specializing in AI/ML, AR/VR/XR platforms, and digital transformation.

## 🌐 Live Site
Your site will be at: `https://yourusername.github.io` or your custom domain

## ✨ Features

- **Modern, Responsive Design**: Mobile-first approach
- **SEO Optimized**: Meta tags, Open Graph for social sharing
- **Project Showcase**: Detailed case studies for major projects
- **Blog Section**: Competitions and technical posts
- **Academic Research**: Papers and research work
- **Contact Integration**: Direct email and LinkedIn links

## 📁 Files Included

```
portfolio/
├── index-improved.html          # Main homepage (RENAME to index.html)
├── blog.html                    # Blog landing page
├── deloitte-datathon.html       # Datathon blog post  
├── alpha3d-ai-platform.html     # Alpha3D project
├── tiktok-live-project.html     # TikTok Live project
├── artspaces-platform.html      # ArtSpaces project
├── miami-art-week.html          # Miami Art Week
├── worlds-away-festival.html    # World's Away Festival
├── rimowa-threedium.html        # Rimowa project
├── traderjoes-paper.html        # Research paper
└── README.md                    # This file
```

## 🚀 Quick Start - GitHub Pages Deployment

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and sign in (or create account)
2. Click **"+ New repository"** (top right)
3. Name it: `yourusername.github.io` (use your actual GitHub username)
4. Make it **Public**
5. Click **"Create repository"**

### Step 2: Upload Files

1. **IMPORTANT**: Rename `index-improved.html` to `index.html` first!
2. On your repo page, click **"uploading an existing file"**
3. Drag ALL your `.html` files into the upload area
4. Click **"Commit changes"**

### Step 3: Enable GitHub Pages

1. Go to **Settings** (in your repository)
2. Click **"Pages"** in left sidebar
3. Under "Source": Select **"main"** branch and **"/ (root)"** folder
4. Click **Save**
5. Wait 2-5 minutes
6. Your site is live at `https://yourusername.github.io` ✅

### Step 4: Connect Custom Domain (Optional)

If you want to use `lindatali.com`:

**In GitHub:**
1. Repository Settings → Pages
2. Add custom domain: `lindatali.com`
3. Check "Enforce HTTPS"

**In WordPress Domain Settings:**
1. Go to your domain registrar (WordPress.com or wherever you bought the domain)
2. Find DNS settings
3. Add these A records:
   ```
   Type: A     Name: @     Value: 185.199.108.153
   Type: A     Name: @     Value: 185.199.109.153
   Type: A     Name: @     Value: 185.199.110.153
   Type: A     Name: @     Value: 185.199.111.153
   Type: CNAME Name: www   Value: yourusername.github.io
   ```
4. Wait 24 hours for DNS to update

## 🎨 Customization Guide

### Update Your Information

**In `index.html`:**

Line 291-293: Your name and title
```html
<h1>Your Name</h1>
<div class="subtitle">Your Title</div>
```

Line 294: Your bio
```html
<p>Your bio here...</p>
```

Lines 296-314: Update stats
```html
<span class="stat-number">10+</span>
<span class="stat-label">Years Experience</span>
```

**In ALL files:**
- Replace `linda.tali@gmail.com` with your email
- Replace LinkedIn URL with yours
- Update copyright in footer

### Add Google Analytics

1. Sign up at [analytics.google.com](https://analytics.google.com)
2. Get your Measurement ID (looks like `G-XXXXXXXXXX`)
3. In EVERY HTML file, find this section in `<head>` and uncomment:

```html
<!-- Remove the comment marks and add your ID -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'G-XXXXXXXXXX');  <!-- Your ID here -->
</script>
```

### Change Colors

All files use CSS variables. Edit in `<style>` section:

```css
:root {
    --navy: #0a1628;      /* Dark background */
    --tech-blue: #3b82f6; /* Primary color - change to your brand */
    --gray: #6b7280;      /* Text color */
}
```

## ➕ Adding New Content

### Add a Blog Post

1. Copy `deloitte-datathon.html`
2. Rename to `my-new-post.html`
3. Edit content (title, date, body text)
4. Open `blog.html`
5. Add a new card in the grid:

```html
<a href="my-new-post.html" class="blog-card">
    <div class="blog-image">🏆</div>
    <div class="blog-content">
        <span class="blog-tag">Competition</span>
        <h3>My New Post Title</h3>
        <p>Brief description...</p>
        <div class="blog-meta">
            <span>📅 March 2025</span>
            <span>⏱️ 5 min read</span>
        </div>
        <span class="read-more">Read Full Post</span>
    </div>
</a>
```

6. Save and upload to GitHub

### Add a Project

1. Copy a similar project file (e.g., `alpha3d-ai-platform.html`)
2. Rename to `my-project.html`
3. Replace ALL content with your project details
4. Open `index.html`
5. Find the `<div class="projects-grid">` section
6. Add:

```html
<a href="my-project.html" class="project-card">
    <span class="project-tag">Category</span>
    <h3>Project Name</h3>
    <p>Brief description of what you did...</p>
    <span class="read-more">View Project</span>
</a>
```

### Add Images

**Method 1: Upload to GitHub**
1. Create `images` folder in your repository
2. Upload images through GitHub interface
3. Reference as: `<img src="images/photo.jpg" alt="Description">`

**Method 2: Use Image Hosting**
1. Upload to [imgur.com](https://imgur.com) or similar
2. Get direct image link
3. Use: `<img src="https://i.imgur.com/xxxxx.jpg" alt="Description">`

**Replace placeholders:**
```html
<!-- Find this -->
<div class="image-placeholder">
    <p>📸 Image description</p>
</div>

<!-- Replace with -->
<img src="images/your-photo.jpg" alt="Description" style="width: 100%; border-radius: 16px; margin: 3rem 0;">
```

## 🔄 Updating Your Site

**After making changes:**

1. **Easy Way** (Web Interface):
   - Go to your GitHub repository
   - Click on the file you want to edit
   - Click the pencil icon (Edit)
   - Make changes
   - Click "Commit changes"
   - Wait 2-3 minutes for site to update

2. **Advanced Way** (Git):
   ```bash
   git add .
   git commit -m "Updated content"
   git push
   ```

## 🧪 Testing Before Upload

**Simple**: Just double-click `index.html` to open in your browser

**Better**: Use a local server:
```bash
# Python 3
python -m http.server 8000
# Then visit http://localhost:8000
```

## ✅ Pre-Launch Checklist

Before you publish, verify:

- [ ] Renamed `index-improved.html` to `index.html`
- [ ] Updated all email addresses to yours
- [ ] Updated LinkedIn URL
- [ ] Tested all internal links (click every link!)
- [ ] Checked on mobile (use phone or Chrome DevTools F12)
- [ ] Added Google Analytics (optional but recommended)
- [ ] Spell-checked all content
- [ ] Removed placeholder text

## 🐛 Troubleshooting

**Site not appearing?**
- Wait 5-10 minutes after enabling GitHub Pages
- Check Settings → Pages shows "Your site is live"
- Make sure `index.html` exists (not `index-improved.html`)

**404 errors on links?**
- File names are case-sensitive: `Project.html` ≠ `project.html`
- All HTML files must be in root directory (same folder as index.html)
- Double-check file name spelling

**Images not loading?**
- Check image path: `images/photo.jpg`
- File uploaded to GitHub?
- No spaces in filename (use `my-photo.jpg` not `my photo.jpg`)

**Mobile menu not working?**
- Basic mobile menu is functional but simple
- For advanced menu, you'd need JavaScript framework

**Custom domain not working?**
- Wait 24-48 hours for DNS propagation
- Check DNS settings are correct
- Try clearing browser cache
- Visit in incognito/private mode

## 📱 Mobile Testing

Your site is mobile-responsive. Test on:
- iPhone (Safari)
- Android (Chrome)
- Tablet

Or use Chrome DevTools:
1. Open site in Chrome
2. Press F12
3. Click device icon (toggle device toolbar)
4. Select different devices

## 🔐 Security

- GitHub Pages automatically provides HTTPS
- No passwords or sensitive data stored
- All code is client-side (runs in browser)

## 💡 Tips for Success

1. **Keep it updated**: Add new projects as you complete them
2. **Blog regularly**: Write about competitions, learnings
3. **SEO**: Use descriptive file names (good: `data-analysis-project.html`, bad: `project1.html`)
4. **Images**: Add real images to replace placeholders
5. **LinkedIn**: Share your portfolio link on LinkedIn profile
6. **Resume**: Keep downloadable resume link updated

## 🆘 Need Help?

1. Read this README thoroughly
2. Check [GitHub Pages Docs](https://docs.github.com/pages)
3. Google specific errors
4. Ask on [Stack Overflow](https://stackoverflow.com)

## 📊 Analytics Tips

After adding Google Analytics:
- Check daily visitors
- See which projects get most views
- Track LinkedIn referrals
- Identify popular content

## 🎓 Learning Resources

Want to customize further?
- **HTML**: [w3schools.com/html](https://w3schools.com/html)
- **CSS**: [w3schools.com/css](https://w3schools.com/css)
- **GitHub Pages**: [pages.github.com](https://pages.github.com)

---

**You're ready to launch! 🚀**

After deployment, share your portfolio on:
- LinkedIn profile (add to "Featured" section)
- Resume (add website link)
- Email signature
- Job applications

**Last Updated**: February 2025
