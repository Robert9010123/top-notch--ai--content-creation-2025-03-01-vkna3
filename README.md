# Landing Page Maintenance Guide

This guide will help you maintain and customize the AI Content Pro landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common maintenance tasks.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<!-- Original -->
<div class="text-2xl font-bold text-gray-800">AI Content Pro</div>

<!-- How to modify -->
<div class="text-2xl font-bold text-gray-800">Your Company Name</div>
```

#### Hero Section
The main headline and subheading are located in the hero section:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 mb-6 leading-tight">
    TOP NOTCH AI CONTENT CREATION
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12 leading-relaxed">
    WE WANT TO GENERATE LEADING AI CONTENTS
</p>
```

### Understanding Tailwind Classes

Key class explanations:
- `text-4xl`: Large text size
- `md:text-5xl`: Larger text on medium screens
- `font-bold`: Bold text weight
- `mb-6`: Bottom margin spacing
- `text-gray-900`: Dark gray text color

To modify styles:
1. Find the element you want to change
2. Locate its class attribute
3. Modify or add Tailwind classes as needed

Example of changing text color and size:
```html
<!-- Original -->
<h3 class="text-xl font-bold text-gray-900 mb-4">PERSONALIZATION</h3>

<!-- Modified (blue text, larger size) -->
<h3 class="text-2xl font-bold text-blue-600 mb-4">PERSONALIZATION</h3>
```

## Fixing Broken Links

### Navigation Menu Links
Current navigation links are:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>
```

To update:
1. Locate the `href` attribute
2. Replace the `#` value with your desired URL
   ```html
   <!-- Example of external link -->
   <a href="https://your-website.com/features">Features</a>
   ```

### Call-to-Action Links
Current CTA links point to a YouTube channel:
```html
<a href="https://www.youtube.com/@robertbabalola8450" class="inline-block bg-blue-600 text-white px-8 py-4 rounded-lg">
    Get Started Today
</a>
```

To update:
1. Replace the YouTube URL with your desired destination
2. Ensure the new URL includes `https://` or `http://`

## Linking Privacy and Terms Pages

### Footer Privacy/Terms Links
Current placeholder links:
```html
<ul class="space-y-2">
    <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a></li>
</ul>
```

To add proper links:
1. Create privacy.html and terms.html files in your project
2. Update the href attributes:
```html
<ul class="space-y-2">
    <li><a href="privacy.html" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a></li>
    <li><a href="terms.html" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a></li>
</ul>
```

### Social Media Links
Update social media links in the footer:
```html
<div class="flex space-x-4">
    <a href="https://twitter.com/your-handle" class="text-gray-400 hover:text-white transition duration-300">
        <i class="fab fa-twitter text-2xl"></i>
    </a>
    <!-- Repeat for LinkedIn and YouTube -->
</div>
```

## Troubleshooting

Common issues and solutions:

1. **Broken Navigation Links**
   - Ensure IDs match href values (e.g., `href="#features"` needs matching `id="features"`)
   - Check for typos in IDs and href attributes
   - Verify file paths for external pages

2. **Responsive Design Issues**
   - Check media query classes (md:, lg:)
   - Ensure viewport meta tag is present:
   ```html
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   ```

3. **Font Awesome Icons Not Showing**
   - Verify the Font Awesome CDN link is working
   - Check icon class names for accuracy
   - Try refreshing the CDN cache

Remember to:
- Test all links after updating
- Preview changes in multiple browsers
- Check mobile responsiveness
- Maintain consistent styling across all pages
- Back up files before making changes

Need more help? Contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).