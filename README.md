# Website Builder - Client Information Form

A standalone HTML form for collecting website information from clients. This form can be shared via GitHub Pages or emailed directly.

## 🚀 Quick Start

### Option 1: Use via GitHub Pages (Recommended)

1. **Fork or clone this repository**
2. **Enable GitHub Pages:**
   - Go to Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` (or `master`)
   - Folder: `/ (root)`
   - Click Save
3. **Share the link:**
   - Your form will be available at: `https://yourusername.github.io/website-builder-form/`
   - Direct form link: `https://yourusername.github.io/website-builder-form/website-builder-form.html`

### Option 2: Use Locally

1. Download `website-builder-form.html`
2. Open it in a web browser
3. Fill out the form and submit

**Note:** When used locally, the form will download a zip file instead of submitting automatically (backend not available).

## 📋 What This Form Does

This form collects all the information needed to generate a website:

- **Step 1:** Company name, colors, logo, slogan, description
- **Step 2:** Content sections (parsed from a write-up), images with categories
- **Step 3:** External links, social media, contact information
- **Step 4:** Products (optional)
- **Step 5:** Color palette upload

## 📤 Submission Options

### Automatic Submission (When Backend is Running)
If the Website Builder app is running, the form will automatically submit the zip file to the app's pending folder.

### Manual Submission (When Backend is Offline)
1. The form will download a zip file to your Downloads folder
2. Create a temporary folder (e.g., "tmp" on your Desktop)
3. Move the zip file there
4. Email the zip file to your website builder
5. They will import it into the Website Builder app

## 📁 File Structure

When submitted, the form creates a zip file containing:
- `website-builder-data.json` - All form data in JSON format
- `images/` - Folder containing all uploaded images (logo, content images, product images, color palette)

## 🔧 Technical Details

- **Standalone HTML** - No server required (except for automatic submission)
- **Uses JSZip** - Client-side zip file creation via CDN
- **File System Access API** - For saving files (with fallback to downloads)
- **Responsive Design** - Works on desktop and mobile

## 📝 For Website Builders

After receiving a zip file from a client:

1. Open the Website Builder app
2. Go to the "Pending" tab
3. Click "Review & Import" on the submission
4. The form data will be automatically loaded into the builder
5. Review and generate the website

## 🐛 Troubleshooting

**Form won't submit automatically:**
- Make sure the Website Builder app is running
- Check that the backend is accessible at `http://localhost:8000`
- The form will fall back to downloading the zip file

**Images not loading:**
- Make sure all images are uploaded before submitting
- Check that image files are valid (JPG, PNG, etc.)

**CDN blocked (local file):**
- If opening from `file://`, some browsers block CDN requests
- Use GitHub Pages or a local web server instead

## 📄 License

This form is part of the Website Builder project.
