# Water Heater Landing Page - Maintenance Guide

This guide will help you maintain and customize the Water Heater Palm City landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common updates.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu. To update:

1. Company Name:
```html
<div class="text-xl font-bold text-white">Water Heater Palm City</div>
```
Simply replace "Water Heater Palm City" with your company name.

### Hero Section
Located at the top of the page with the main headline:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-6">
    Water Heater Repair, Installation or Replacement in Palm City
</h1>
```
- To modify text size:
  - `text-4xl`: Base size for mobile
  - `md:text-5xl`: Medium screens
  - `lg:text-6xl`: Large screens

### Services Section
Each service card follows this structure:
```html
<div class="bg-gray-900 p-8 rounded-xl hover:shadow-2xl transition duration-300">
    <i class="fas fa-wrench text-blue-500 text-4xl mb-4"></i>
    <h3 class="text-xl font-semibold mb-4">Water Heater Repair</h3>
    <p class="text-gray-400">Professional repair services...</p>
</div>
```
To modify:
1. Change icon: Update `fa-wrench` to any [Font Awesome](https://fontawesome.com/icons) icon
2. Update heading: Replace text in `<h3>` tag
3. Update description: Modify text in `<p>` tag

## Managing Links

### Navigation Menu Links
Current navigation structure:
```html
<div class="hidden md:flex space-x-8">
    <a href="#services" class="hover:text-blue-400 transition duration-300">Services</a>
    <a href="#benefits" class="hover:text-blue-400 transition duration-300">Benefits</a>
    <a href="#faq" class="hover:text-blue-400 transition duration-300">FAQ</a>
    <a href="tel:7287770057" class="bg-blue-600 hover:bg-blue-700 px-4 py-2 rounded-lg transition duration-300">
        (728) 777-0057
    </a>
</div>
```

To update:
1. Internal links (starting with #): Match with section IDs
2. Phone number: Update both `href="tel:XXXXXXXXXX"` and the displayed number
3. Add new links by copying existing `<a>` tag structure

### Footer Links
Located at the bottom of the page:
```html
<ul class="space-y-2">
    <li><a href="#services" class="text-gray-400 hover:text-white">Services</a></li>
    <li><a href="#benefits" class="text-gray-400 hover:text-white">Benefits</a></li>
    <li><a href="#faq" class="text-gray-400 hover:text-white">FAQ</a></li>
</ul>
```

## Adding Privacy and Terms Pages

To add privacy and terms links to the footer:

1. Add new list items to the footer's Quick Links section:
```html
<ul class="space-y-2">
    <!-- Existing links -->
    <li><a href="privacy.html" class="text-gray-400 hover:text-white">Privacy Policy</a></li>
    <li><a href="terms.html" class="text-gray-400 hover:text-white">Terms of Service</a></li>
</ul>
```

2. Create corresponding HTML files:
   - Create `privacy.html` in the same directory
   - Create `terms.html` in the same directory
   - Use the same styling classes for consistency

## Troubleshooting

Common issues and solutions:

### Responsive Design Issues
If elements don't stack properly on mobile:
- Check for `md:` prefixes in classes
- Ensure container has proper padding: `px-4`
- Verify grid classes: `grid-cols-1 md:grid-cols-3`

### Link Problems
If internal links don't scroll:
1. Verify section IDs match href attributes
2. Check for `scroll-smooth` class on HTML tag
3. Ensure no typos in href values

### Style Inconsistencies
If new elements don't match existing style:
1. Copy classes from similar elements
2. Maintain color scheme:
   - Background: `bg-gray-900`
   - Text: `text-gray-100`
   - Accent: `text-blue-400`
   - Hover: `hover:text-blue-300`

Remember to test all changes across different screen sizes using browser developer tools.

---

Need additional help? Contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).