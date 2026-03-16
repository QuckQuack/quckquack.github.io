# Your Personal Website

## Files Included
- index.html      — Home page
- about.html      — About me page
- photography.html — Photo gallery with filter + lightbox
- blog.html       — Journal / blog page
- contact.html    — Contact form
- style.css       — All styles (edit colours/fonts here)
- script.js       — Hamburger menu, lightbox, filters, form
- images/         — Put all your photos in this folder

## Deploying to GitHub Pages

### First time setup
1. Go to github.com → sign in → click + → New Repository
2. Name it exactly: yourusername.github.io
3. Set to Public → Create Repository

### Upload your files
Option A (browser):
1. Open your new repo
2. Click "Add file" → "Upload files"
3. Drag all these files in (keep the folder structure)
4. Click "Commit changes"

Option B (Git command line):
  git clone https://github.com/yourusername/yourusername.github.io
  cd yourusername.github.io
  # copy all your website files here
  git add .
  git commit -m "Initial site"
  git push

### Enable GitHub Pages
1. Go to repo → Settings → Pages
2. Source: Deploy from a branch
3. Branch: main / (root)
4. Save → wait 1-2 mins
5. Visit https://yourusername.github.io

## Customising the Site

### Change your name throughout
Search and replace "Your Name" across all HTML files with your real name.

### Change the accent colour
In style.css, find:
  --accent: #C84B2F;
Replace with any hex colour you like.

### Add your photos (photography.html)
1. Put your photo files inside the images/ folder
2. Find any .photo-item div in photography.html
3. Replace the entire <div class="photo-placeholder">...</div> with:
   <img src="images/yourphoto.jpg" alt="Description of photo">
4. Set data-category on the parent .photo-item to: portrait, landscape, street, or travel

### Make the contact form send real emails
1. Sign up free at formspree.io
2. Create a form — you'll get an endpoint like https://formspree.io/f/abc123
3. In contact.html, change:
   <form id="contact-form">
   to:
   <form id="contact-form" action="https://formspree.io/f/abc123" method="POST">

### Update social links
In every HTML file, find the .footer-socials section and replace # with your real URLs.

### Add a favicon
Create a small square image (32x32 or 64x64 px) saved as favicon.ico
Add this inside the <head> of every HTML file:
  <link rel="icon" href="favicon.ico" type="image/x-icon">
