# The Handy Mantis Website

Professional handyman services website for The Handy Mantis serving Independence, MO and surrounding areas.

## Files Included

- `index.html` - Home page
- `services.html` - Services and pricing page
- `contact.html` - Contact page with form
- `styles.css` - Stylesheet for all pages
- `logo.png` - Your logo (you'll need to add this)

## Setup Instructions

### 1. Set Up Formspree (Contact Form)

1. Go to https://formspree.io and sign up for a free account
2. Create a new form
3. Copy your form ID (looks like: `xrbzgpqw`)
4. Open `contact.html` and replace `YOUR_FORM_ID` on line 54 with your actual form ID:
   ```html
   <form action="https://formspree.io/f/xrbzgpqw" method="POST" class="contact-form">
   ```
5. Form submissions will be sent to thehandymantis@gmail.com

### 2. Add Your Logo

1. Save your logo image as `logo.png` 
2. Place it in the same folder as the HTML files
3. Recommended size: 400x400 pixels (transparent background works best)

### 3. Deploy to GitHub Pages

#### Create a GitHub account (if you don't have one):
1. Go to https://github.com and sign up

#### Create a new repository:
1. Click the "+" in the top right, select "New repository"
2. Name it: `yourusername.github.io` (replace "yourusername" with your GitHub username)
3. Make it Public
4. Don't initialize with a README
5. Click "Create repository"

#### Upload your files:
1. Click "uploading an existing file"
2. Drag and drop all files:
   - index.html
   - services.html
   - contact.html
   - styles.css
   - logo.png
3. Click "Commit changes"

Your site will be live at: `https://yourusername.github.io`

### 4. Connect Your Custom Domain (thehandymantis.com)

#### In your GitHub repository:
1. Go to Settings > Pages
2. Under "Custom domain", enter: `thehandymantis.com`
3. Click Save
4. Check "Enforce HTTPS" (wait a few minutes for it to become available)

#### In Namecheap:
1. Log in to Namecheap
2. Go to Domain List > Manage for thehandymantis.com
3. Click "Advanced DNS"
4. Delete any existing A Records and CNAME Records
5. Add these A Records (all with Host: @):
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
6. Add this CNAME Record:
   - Type: CNAME Record
   - Host: www
   - Value: `yourusername.github.io.` (replace with your GitHub username, keep the dot at the end)
   - TTL: Automatic

#### Wait for DNS propagation:
- This can take 24-48 hours
- Your site will then be live at thehandymantis.com

## Making Changes

To update your website:
1. Edit the HTML or CSS files on your computer
2. Go to your GitHub repository
3. Click on the file you want to update
4. Click the pencil icon (Edit)
5. Paste your updated content
6. Click "Commit changes"
7. Changes go live immediately

## Color Scheme

The website uses a green color scheme to match your logo:
- Primary Green: #2d5016
- Light Green: #4a7c2c
- Accent Orange: #e67e22 (for buttons and highlights)

## Support

If you need help:
- GitHub Pages docs: https://docs.github.com/en/pages
- Formspree docs: https://help.formspree.io
- Contact me if you run into issues!

## Future Enhancements

Consider adding:
- Before/after photos of your work
- Customer testimonials
- Service area map
- FAQ section
- Blog for home maintenance tips
