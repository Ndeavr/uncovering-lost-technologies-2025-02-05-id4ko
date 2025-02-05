# NDEAVR Landing Page Maintenance Guide

This guide will help you maintain and customize the NDEAVR landing page. Whether you're new to web development or need a quick reference, follow these instructions to make common updates safely and effectively.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Policy Pages](#adding-policy-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Main Sections
The landing page is divided into these key sections:
1. Header/Navigation
2. Hero Section
3. Features Section
4. Benefits Section
5. FAQ Section
6. Call-to-Action Section
7. Footer

### Updating Text Content

#### Hero Section
```html
<!-- Located in the first <section> tag -->
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-8">Uncovering Lost Technologies</h1>
<p class="text-xl md:text-2xl text-gray-300 mb-12">Developing technologies...</p>
```
To update:
1. Locate the `<h1>` tag for the main heading
2. Replace the text between the tags
3. For the subtitle, modify the text within the `<p>` tag

#### Features Section
```html
<div class="bg-gray-700/50 rounded-2xl p-8">
    <h3 class="text-2xl font-semibold mb-4">Recover Lost Technologies</h3>
    <p class="text-gray-300 leading-relaxed">Rediscovering ancient wisdom...</p>
</div>
```
To update feature cards:
1. Find the feature section (`id="features"`)
2. Locate each feature card within the grid
3. Update the `<h3>` for titles and `<p>` for descriptions

### Modifying Tailwind CSS Classes

#### Understanding Key Classes
- `container`: Centers content and sets max-width
- `mx-auto`: Centers elements horizontally
- `px-6`: Adds horizontal padding
- `py-24`: Adds vertical padding
- `grid`: Creates grid layouts
- `rounded-2xl`: Rounds corners
- `hover:`: Prefix for hover effects

#### Example: Adjusting Card Styling
Original:
```html
<div class="bg-gray-700/50 rounded-2xl p-8 hover:bg-gray-700">
```
To modify:
1. Change background color: Replace `bg-gray-700/50` with another color (e.g., `bg-blue-700/50`)
2. Adjust padding: Change `p-8` to `p-4` (smaller) or `p-12` (larger)
3. Modify hover effect: Update `hover:bg-gray-700` to desired color

## Managing Links

### Current Link Structure
```html
<!-- Navigation Menu Links -->
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="https//www.ndeavr.com/making-contact">Contact Us</a>
```

### Updating Links
1. Internal Links (Same Page):
   ```html
   <!-- Format: -->
   <a href="#section-id">Section Name</a>
   ```

2. External Links:
   ```html
   <!-- Format: -->
   <a href="https://full-website-url.com/page">Page Name</a>
   ```

### Fixing Common Link Issues
1. Check for typos in URLs
2. Ensure internal links match section IDs exactly
3. Add `https://` to external links
4. Test all links after updating

## Adding Policy Pages

### Footer Policy Links
Current placeholder links:
```html
<div>
    <h4 class="text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-blue-400">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-blue-400">Terms of Service</a></li>
    </ul>
</div>
```

To link policy pages:
1. Create your policy pages (privacy.html, terms.html)
2. Update the href attributes:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-blue-400">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-blue-400">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. Broken Layout
- Check for missing closing tags
- Verify container classes are present
- Ensure proper grid column settings

2. Styling Issues
- Confirm Tailwind CSS is properly loaded
- Check for typos in class names
- Verify responsive classes (md:, lg:) are correct

3. Non-Working Links
- Verify file paths and URLs
- Check for proper section IDs
- Ensure external URLs include `https://`

### Need Help?
If you encounter issues:
1. Check the browser console for errors
2. Verify all files are in the correct directory
3. Test responsive layouts using browser dev tools
4. Contact support at git@ndeavr.com

Remember to always backup your files before making changes!