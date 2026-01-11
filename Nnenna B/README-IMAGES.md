# Personal Website - Image Guide

## 📸 Adding Your Images

Your website is now set up with proper `<img>` tags that will automatically display your images when you add them. Here's how to add your own photos and media:

### Profile Photo (About Page)

**Location**: Root directory  
**Filename**: `profile-photo.jpg`  
**Recommended size**: 800x800px (square, 1:1 aspect ratio)

Simply add your profile photo to the `personal` folder with the name `profile-photo.jpg`.

---

### Media Gallery Images

**Location**: Create a `media` folder in your `personal` directory  
**Path**: `c:/Users/User/OneDrive/Desktop/personal/media/`

Add the following images to the `media` folder:

#### Conference Photos

1. `conference-keynote-2024.jpg` - Keynote at AI Conference
2. `panel-discussion-mit.jpg` - Panel Discussion at MIT
3. `international-symposium-tokyo.jpg` - International Symposium
4. `workshop-presentation-icml.jpg` - Workshop Presentation

#### Research Photos

5. `lab-research-session.jpg` - Lab Research Session
6. `collaborative-research.jpg` - Collaborative Research Project
7. `experimental-setup.jpg` - Experimental Setup

#### Events Photos

8. `tech-innovation-summit.jpg` - Tech Innovation Summit
9. `guest-lecture-berkeley.jpg` - Guest Lecture Series
10. `industry-partnership.jpg` - Industry Partnership Event

#### Awards Photos

11. `best-paper-award.jpg` - Best Paper Award Ceremony
12. `excellence-research-award.jpg` - Excellence in Research Award

**Recommended size**: 1200x900px (4:3 aspect ratio)

---

### Video Files (Optional)

If you want to add actual video files instead of placeholders:

**Location**: `media` folder  
**Format**: MP4, WebM, or OGG

Example filenames:

- `tedx-talk-ai-future.mp4`
- `keynote-sustainable-computing.mp4`
- `research-overview.mp4`
- `panel-privacy-digital-age.mp4`

To use videos, replace the placeholder div in `media.html` with:

```html
<video controls style="aspect-ratio: 16/9; border-radius: var(--radius-lg);">
  <source src="media/your-video.mp4" type="video/mp4" />
  Your browser does not support the video tag.
</video>
```

---

## 🎨 Image Specifications

### Recommended Formats

- **Photos**: JPG or PNG
- **Videos**: MP4 (H.264 codec)
- **Graphics**: PNG with transparency

### Optimal Sizes

- **Profile Photo**: 800x800px (1:1 ratio)
- **Media Gallery**: 1200x900px (4:3 ratio)
- **Video Thumbnails**: 1920x1080px (16:9 ratio)

### File Size Tips

- Keep images under 500KB for fast loading
- Compress images using tools like TinyPNG or Squoosh
- For videos, keep under 50MB if possible

---

## 🔄 Fallback System

The website has a smart fallback system:

1. **If image exists**: Displays your actual photo
2. **If image is missing**: Shows a colorful gradient background with an emoji icon

This means the website will look great even before you add your images!

---

## 📁 Folder Structure

```
personal/
├── index.html
├── about.html
├── research.html
├── media.html
├── awards.html
├── talks.html
├── styles.css
├── script.js
├── profile-photo.jpg          ← Add your profile photo here
└── media/                      ← Create this folder
    ├── conference-keynote-2024.jpg
    ├── lab-research-session.jpg
    ├── tech-innovation-summit.jpg
    ├── best-paper-award.jpg
    ├── panel-discussion-mit.jpg
    ├── collaborative-research.jpg
    ├── guest-lecture-berkeley.jpg
    ├── international-symposium-tokyo.jpg
    ├── experimental-setup.jpg
    ├── industry-partnership.jpg
    ├── excellence-research-award.jpg
    └── workshop-presentation-icml.jpg
```

---

## 🚀 Quick Start

1. **Create the media folder**:

   - Right-click in the `personal` folder
   - Select "New Folder"
   - Name it `media`

2. **Add your profile photo**:

   - Rename your photo to `profile-photo.jpg`
   - Copy it to the `personal` folder

3. **Add gallery images**:

   - Rename your photos to match the filenames above
   - Copy them to the `media` folder

4. **Open the website**:
   - Double-click `index.html` to view
   - Your images will automatically appear!

---

## 💡 Tips

- **Use descriptive filenames** if you want to customize the image names (just update the `src` attribute in the HTML)
- **Maintain aspect ratios** for best appearance
- **Optimize images** before uploading for faster load times
- **Test locally** by opening `index.html` in your browser

---

## 🎯 Customization

To change image filenames or add more images:

1. Open the relevant HTML file (`about.html` or `media.html`)
2. Find the `<img>` tag you want to modify
3. Update the `src` attribute with your new filename
4. Update the `alt` attribute with a description

Example:

```html
<img
  src="media/my-custom-photo.jpg"
  alt="Description of my photo"
  onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';"
/>
```

---

## ✅ Checklist

- [ ] Create `media` folder
- [ ] Add profile photo (`profile-photo.jpg`)
- [ ] Add 12 gallery images to `media` folder
- [ ] Test website in browser
- [ ] Verify all images display correctly
- [ ] Optimize image sizes if needed

---

**Need help?** All image tags include automatic fallbacks, so your website will always look professional even while you're adding images!
