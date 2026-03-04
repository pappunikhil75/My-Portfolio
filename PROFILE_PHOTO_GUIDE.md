# Profile Photo Setup Guide

## How to Add Your Own Profile Photo

Your portfolio now has a profile photo section in the hero area! Currently, it's using a placeholder image. Here's how to replace it with your own photo:

### Option 1: Use a Local Image File (Recommended)

1. **Prepare Your Image:**
   - Get a square image (e.g., 300x300px or larger)
   - Save it as `profile.jpg`, `profile.png`, or `profile.webp`
   - Place it in the same folder as your `index.html`

2. **Update the HTML:**
   - Open `index.html`
   - Find this line (around line 46):
     ```html
     <img src="https://via.placeholder.com/300x300?text=Your+Photo" alt="Profile Photo" class="profile-photo">
     ```
   - Replace the `src` with your image:
     ```html
     <img src="profile.jpg" alt="Profile Photo" class="profile-photo">
     ```
   - Save the file

### Option 2: Use an Online Image URL

1. Upload your image to a free image hosting service like:
   - Imgur (imgur.com)
   - imgBB (imgbb.com)
   - Cloudinary (cloudinary.com)

2. Copy the image URL and replace in `index.html`:
   ```html
   <img src="YOUR_IMAGE_URL_HERE" alt="Profile Photo" class="profile-photo">
   ```

### Option 3: Use Base64 Encoded Image

For advanced users, you can encode your image and embed it directly:
- Use an online converter: base64-image.de
- Convert your image to base64
- Replace the `src` with: `data:image/jpeg;base64,BASE64_CODE_HERE`

## Photo Specifications

- **Recommended size:** 300x300px or larger
- **Aspect ratio:** 1:1 (square)
- **File formats:** JPG, PNG, or WebP
- **File size:** Under 500KB for faster loading

## Photo Styling Features

Your profile photo automatically includes:
- ✓ Circular shape with border
- ✓ Glowing shadow effect
- ✓ Smooth hover animations
- ✓ Floating animation effect
- ✓ Fully responsive (scales on mobile)

## Tips for Best Results

1. Use a high-quality, well-lit photo
2. Ensure your face is clearly visible
3. Use a simple, professional background
4. Avoid logos or text in the image
5. Keep the image square for best results

## Having Issues?

- **Image not showing?** 
  - Check the file path is correct
  - Make sure the file exists in the same folder
  - Try opening the image URL directly in your browser

- **Image looks stretched?**
  - Ensure your image is square (1:1 aspect ratio)
  - It will automatically crop to fit

- **Want to change colors?**
  - Edit `style.css`
  - Look for `.profile-photo` and modify the `border` and `box-shadow` properties
  - Default color: `var(--primary-color)` (blue gradient)

Enjoy your portfolio with your professional photo! 📸
