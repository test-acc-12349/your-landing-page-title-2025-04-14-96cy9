# Landing Page Maintenance Guide

This guide will help you maintain and customize your landing page. Follow these detailed instructions to make updates while preserving the design and functionality.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your logo and navigation menu. To update:

1. Change the logo text:
```html
<!-- Find this line in the header -->
<div class="text-2xl font-bold text-gray-800">Logo</div>
<!-- Replace "Logo" with your company name -->
```

2. Modify navigation menu items:
```html
<div class="hidden md:flex space-x-8">
    <!-- Each link can be customized here -->
    <a href="#features" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Features</a>
</div>
```

### Hero Section
Located at the top of the page with the main headline:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-extrabold text-gray-900 leading-tight mb-8">
    Create stunning landing pages in minutes
</h1>
```

To modify:
1. Replace the text between the `<h1>` tags
2. Keep the existing classes to maintain responsive design
3. The `text-4xl`, `md:text-5xl`, and `lg:text-6xl` control text size at different screen sizes

### Understanding Tailwind Classes

Key classes explained:
- `container mx-auto`: Centers content and sets max-width
- `px-6`: Adds horizontal padding
- `py-4`: Adds vertical padding
- `text-gray-600`: Sets text color
- `hover:text-gray-900`: Changes text color on hover
- `md:`: Applies styles only on medium screens and larger

## Managing Links

### Navigation Menu Links
Current internal links in the navigation:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>
```

To update:
1. Locate the link in the header section
2. Change the `href` attribute to your desired destination
3. Update the link text between the `<a>` tags

### Call-to-Action Buttons
The "Get Started" buttons currently point to a placeholder URL:

```html
<!-- Find these lines -->
<a href="https://example.com/signup" class="inline-flex items-center...">
    Get Started Now
</a>

<!-- Replace with your actual signup URL -->
<a href="https://yourwebsite.com/signup" class="inline-flex items-center...">
    Get Started Now
</a>
```

### Footer Links
The footer contains several sections of links:

```html
<ul class="space-y-2">
    <li><a href="#" class="hover:text-white transition-colors duration-300">About</a></li>
    <li><a href="#" class="hover:text-white transition-colors duration-300">Blog</a></li>
    <li><a href="#" class="hover:text-white transition-colors duration-300">Careers</a></li>
</ul>
```

To update:
1. Replace `#` with your actual page URLs
2. Maintain the existing classes for consistent styling
3. Update the link text as needed

## Adding Privacy and Terms Pages

### Step 1: Locate the Legal Section
Find this section in the footer:

```html
<div>
    <h3 class="text-white text-lg font-semibold mb-4">Legal</h3>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

### Step 2: Update the Links
Replace the placeholder `#` with your actual page URLs:

```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

Common issues and solutions:

1. **Broken Links**
   - Check that all `href` attributes point to valid URLs
   - Ensure internal links (starting with #) match section IDs
   - Test all links after updating

2. **Responsive Design Issues**
   - Don't remove `md:`, `lg:`, or other responsive prefixes
   - Keep the `container` class on parent elements
   - Maintain the existing padding classes (`px-6`, etc.)

3. **Style Inconsistencies**
   - Copy existing classes when adding new elements
   - Use the same color classes (e.g., `text-gray-600`)
   - Maintain hover effects with `hover:` classes

Need help? Contact your web developer or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).