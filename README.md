# RecipesPinned Landing Page - Maintenance Guide

This guide will help you maintain and customize the RecipesPinned landing page. Whether you're new to web development or need a quick reference, follow these instructions to make common updates safely and effectively.

## 1. Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<!-- Located at the top of the page -->
<a href="/" class="text-2xl font-bold text-indigo-600">RecipesPinned</a>
```
To change the website name:
1. Locate this line in the header section
2. Replace "RecipesPinned" with your desired name
3. Keep the surrounding HTML tags intact

#### Hero Section
```html
<h1 class="text-4xl md:text-6xl font-bold leading-tight mb-6">
    Why Do 10,000+ Cooks Save These Recipe Ideas Daily? Find Out!
</h1>
<p class="text-xl md:text-2xl mb-8">Pinterest's Most-Saved Recipes—Yours Free!</p>
```
To update the main headline:
1. Find the `<h1>` tag in the hero section
2. Replace the text between the tags
3. Keep the same format and punctuation style

### Tailwind CSS Classes Explained

#### Responsive Design Classes
- `md:` prefix means the style applies to medium-sized screens and larger
- Example: `text-4xl md:text-6xl` means:
  - Normal screens: text is extra-large (4xl)
  - Medium screens and up: text is super-large (6xl)

#### Common Class Patterns
```html
<!-- Button styling example -->
<button class="bg-indigo-600 text-white px-6 py-2 rounded-full hover:bg-indigo-700">
```
Key classes explained:
- `bg-indigo-600`: Background color
- `text-white`: Text color
- `px-6`: Horizontal padding
- `py-2`: Vertical padding
- `rounded-full`: Rounded corners
- `hover:bg-indigo-700`: Color change on hover

## 2. Fixing Broken Links

### Navigation Menu Links
Current navigation structure:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-600 hover:text-indigo-600">Features</a>
    <a href="#benefits" class="text-gray-600 hover:text-indigo-600">Benefits</a>
    <a href="#contact" class="text-gray-600 hover:text-indigo-600">Contact</a>
</div>
```

To update navigation links:
1. Locate the `href` attribute in each `<a>` tag
2. Replace the `#` anchor links with your page URLs
3. Example:
   ```html
   <a href="features.html" class="text-gray-600 hover:text-indigo-600">Features</a>
   ```

### Social Media Links
Located in the footer:
```html
<div class="flex space-x-4">
    <a href="#" class="text-gray-400 hover:text-white">
        <!-- Facebook icon -->
    </a>
    <a href="#" class="text-gray-400 hover:text-white">
        <!-- Instagram icon -->
    </a>
</div>
```

To update social media links:
1. Replace the `#` in `href="#"` with your social media URLs
2. Example:
   ```html
   <a href="https://facebook.com/yourpage" class="text-gray-400 hover:text-white">
   ```

## 3. Linking Privacy and Terms Pages

### Footer Legal Links
Current structure:
```html
<ul class="space-y-2 text-gray-400">
    <li><a href="#" class="hover:text-white">Privacy Policy</a></li>
    <li><a href="#" class="hover:text-white">Terms of Service</a></li>
</ul>
```

To add privacy and terms pages:
1. Create your privacy.html and terms.html files
2. Update the href attributes:
   ```html
   <ul class="space-y-2 text-gray-400">
       <li><a href="privacy.html" class="hover:text-white">Privacy Policy</a></li>
       <li><a href="terms.html" class="hover:text-white">Terms of Service</a></li>
   </ul>
   ```

## Troubleshooting Tips

1. **Broken Styles**
   - Check for typos in Tailwind class names
   - Ensure all classes are space-separated
   - Verify the Tailwind CDN link is working

2. **Non-Working Links**
   - Confirm file names match exactly (case-sensitive)
   - Verify file locations relative to index.html
   - Test all links after updating

3. **Responsive Issues**
   - Test on multiple screen sizes
   - Check that `md:` classes are working
   - Verify the viewport meta tag is present

## Need Help?

If you encounter issues:
1. Check the browser's developer tools (F12) for errors
2. Verify all files are in the correct locations
3. Ensure all HTML tags are properly closed
4. Compare your changes against the original code

Remember to always backup your files before making changes!