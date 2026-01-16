# Adding Product Images to Your Website

## Quick Guide

Your website now includes a product showcase section with three Broad purifier cards. Here's how to add your actual product images:

## Step 1: Prepare Your Images

**Recommended specifications:**
- **Format**: JPG or PNG
- **Size**: 800x800 pixels (minimum), up to 1200x1200 pixels (ideal)
- **Aspect ratio**: Square (1:1) or slightly landscape (4:3)
- **File size**: Under 500KB each for fast loading
- **Quality**: High resolution, professional product photography

**Tips for best results:**
- Use clean, white or neutral backgrounds
- Show the product from a front/slight angle view
- Ensure good lighting with no harsh shadows
- Include the entire product in frame

## Step 2: Rename Your Images

Rename your product and system photos to match these exact filenames:

**Product Images:**
1. **Home purifier**: `broad-home-purifier.jpg`
2. **Commercial system**: `broad-commercial-purifier.jpg`
3. **Industrial solution**: `broad-industrial-purifier.jpg`

**System/Technology Images:**
4. **Filtration technology**: `broad-filtration-technology.jpg`
5. **HEPA architecture**: `broad-hepa-architecture.jpg`

## Step 3: Create Images Folder

In your project directory (where `index.html` is located):

```
particulate-matter-website/
├── index.html
├── README.md
├── .gitignore
└── images/                                  ← Create this folder
    ├── broad-home-purifier.jpg              ← Product images
    ├── broad-commercial-purifier.jpg
    ├── broad-industrial-purifier.jpg
    ├── broad-filtration-technology.jpg      ← System images
    └── broad-hepa-architecture.jpg
```

## Step 4: Upload to GitHub

### Method A: GitHub Web Interface

1. Go to your repository on GitHub
2. Click "Add file" → "Upload files"
3. Drag and drop your entire `images` folder
4. Commit the changes
5. Wait 1-2 minutes for the site to update

### Method B: Git Command Line

```bash
# Add the images folder
git add images/

# Commit
git commit -m "Add product images"

# Push to GitHub
git push
```

## Step 5: Verify

1. Visit your live site: `https://YOUR-USERNAME.github.io/particulate-matter-website`
2. Scroll to the "Broad's Design Choice" section
3. Your product images should now be displayed

## Troubleshooting

**Images not showing?**
- Check that filenames match exactly (case-sensitive)
- Verify images are in the `images` folder, not a subfolder
- Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Wait 2-3 minutes after uploading to GitHub

**Images look distorted?**
- Use square or nearly-square aspect ratios
- Recommended: 800x800px to 1200x1200px
- Avoid very wide or very tall images

**Site loading slowly?**
- Compress images using tools like TinyPNG.com
- Keep each image under 500KB
- Use JPG format for photos (smaller file size)

## Optional: Add More Products

To add more product cards, edit `index.html` and copy this template:

```html
<div class="product-card">
    <div class="product-image">
        <img src="images/your-product-name.jpg" alt="Product Name">
    </div>
    <div class="product-info">
        <div class="product-category">CATEGORY</div>
        <h3 class="product-name">Product Name</h3>
        <p class="product-description">
            Your product description here.
        </p>
        <div class="product-features">
            <span class="feature-tag">FEATURE 1</span>
            <span class="feature-tag">FEATURE 2</span>
        </div>
    </div>
</div>
```

## Stock Images (Temporary)

If you don't have product photos yet, you can use free stock images temporarily:

**Free image sources:**
- Unsplash.com (search "air purifier")
- Pexels.com (search "air filter")
- Pixabay.com (search "air cleaner")

Download high-quality images and rename them to match the required filenames.

## Professional Product Photography

For best results, consider:
- Hiring a product photographer
- Using a lightbox for consistent lighting
- Taking multiple angles (front, side, detail shots)
- Creating lifestyle shots (products in actual environments)

## Mobile Display

The product cards automatically adapt to mobile screens:
- **Desktop**: 3 cards per row
- **Tablet**: 2 cards per row  
- **Mobile**: 1 card per row (stacked)

All images are optimized to look great on any device!
