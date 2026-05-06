# XooPress Themes

Welcome to the theme repository for **XooPress** – a collection of beautiful, responsive themes following the WordPress-style theming system.

## What are XooPress Themes?

Themes control the visual appearance of your XooPress site. They follow the familiar WordPress template hierarchy, support child themes, and offer per-theme settings stored in the database.

## Theme Structure

```
themes/my-theme/
├── style.css # Theme metadata (required)
├── index.php # Main template (required fallback)
├── header.php # Header template part
├── footer.php # Footer template part
├── sidebar.php # Sidebar template part
├── functions.php # Theme functions (loaded on every request)
├── screenshot.png # Admin preview image (880x660)
├── theme.json # Advanced configuration (optional)
└── assets/ # CSS, JS, images
```


## Available Themes

| Theme | Description | Tags |
|-------|-------------|------|
| [XooPress Lite](https://github.com/XooPress-Themes/xoopress-lite) | Default light theme, clean and modern | light, responsive, accessibility-ready |
| [XooPress Dark](https://github.com/XooPress-Themes/xoopress-dark) | Sleek dark theme for night owls | dark, modern, developer-friendly |
| [OrangeBlaze](https://github.com/XooPress-Themes/orangeblaze) | Vibrant orange theme for creative agencies | orange, vibrant, creative |
| [GreenLeaf](https://github.com/XooPress-Themes/greenleaf) | Fresh, organic green theme | green, nature, eco-friendly |
| [PurpleHaze](https://github.com/XooPress-Themes/purplehaze) | Elegant purple theme for premium brands | purple, elegant, sophisticated |

## Theme Features

- ✅ **WordPress-style template hierarchy**
- ✅ **Child theme support** – safe updates without losing customizations
- ✅ **Per-theme settings** – store configuration in database
- ✅ **Responsive design** – mobile-friendly out of the box
- ✅ **Accessibility ready** – semantic HTML, ARIA labels
- ✅ **Multiple editor formats** – Visual, HTML, Markdown, PHP
- ✅ **Print styles** – optimized for printing

## style.css Header Example

```css
/*
Theme Name: My Theme
Theme URI: https://example.com/
Author: Your Name
Description: A description of your theme.
Version: 1.0.0
License: GPL-3.0-or-later
Template: parent-theme-dir  /* For child themes */
Tags: responsive, two-columns, custom-header
Text Domain: my-theme
*/
```

### Creating a Child Theme
A child theme only needs a style.css with the Template: header:

```css
/*
Theme Name: My Child Theme
Template: xoopress-lite
*/
```

## Theme Development
See the Theme Development Guide for complete documentation.

#### Available Template Variables
| Variable | Description |
| -------- | ------- |
| $theme	 | ThemeManager instance |
| $siteName | Site name from settings |
| $posts	 | Array of post records |
| $post	 | Single post record |

#### Template Parts
```php
$theme->getHeader();      // header.php
$theme->getFooter();      // footer.php
$theme->getSidebar();     // sidebar.php
$theme->getTemplatePart('loop'); // loop.php
```

## Contributing
- Fork the theme repository

- Create your feature branch

- Test your theme with XooPress Core

- Submit a pull request

### Theme Requirements
- Must have valid style.css header

- Must be responsive (test on mobile devices)

- Should include screenshot.png (880x660)

- Must follow accessibility best practices

## License
All themes are licensed under GPL-3.0-or-later unless specified otherwise.


_**Design beautiful sites with XooPress themes.**_



---

### Summary Dashboard

| Organization | Purpose | Key Repositories |
|--------------|---------|------------------|
| **XooPress** | Core CMS system | Core, Installer, Documentation |
| **XooPress-Modules** | Extend functionality | System, Content, Wiki, Gallery, Forms, SEO, E-commerce |
| **XooPress-Themes** | Visual appearance | XooPress Lite, XooPress Dark, OrangeBlaze, GreenLeaf, PurpleHaze |

