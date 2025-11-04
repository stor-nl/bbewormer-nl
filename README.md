# Brassband Eensgezindheid Wormer

A modern Jekyll website for Brassband Eensgezindheid Wormer, optimized for GitHub Pages.

## About This Website

This website is a modern restructuring of the original [bbewormer.nl](https://bbewormer.nl/) website. The site is built with Jekyll and optimized for GitHub Pages hosting.

## Features

- **Modern Design**: Responsive design with a clean, professional look
- **Jekyll Powered**: Built with Jekyll for easy content management
- **GitHub Pages Ready**: Fully configured for GitHub Pages deployment
- **Mobile First**: Fully responsive design for all devices
- **SEO Optimized**: Optimized for search engines
- **Fast Loading**: Optimized for fast load times

## Local Development

### Requirements

- Ruby 3.1 or higher
- Bundler gem

### Installation

1. Clone the repository:
```bash
git clone https://github.com/stor-dev/bbewormer-nl
cd bbewormer-nl
```

2. Install dependencies:
```bash
bundle install
```

3. Start the Jekyll server:
```bash
bundle exec jekyll serve
```

4. Open your browser and navigate to `http://localhost:4000`

## Project Structure

```
├── _config.yml          # Jekyll configuration
├── _layouts/            # HTML templates
│   ├── default.html     # Main template
│   ├── page.html        # Page template
│   └── post.html        # Blog post template
├── _posts/              # Blog posts
├── assets/              # CSS, JS, and images
│   ├── css/
│   ├── js/
│   └── images/
├── index.html           # Homepage
├── over-ons.md          # About us page
├── dirigent.md          # Conductor page
├── agenda.md            # Events page
├── lid-worden.md        # Membership page
├── fotos.md             # Photos page
└── contact.md           # Contact page
```

## Adding Content

### New Pages
Create a new `.md` file in the root directory with the following front matter:

```yaml
---
layout: page
title: "Page Title"
subtitle: "Subtitle (optional)"
description: "Meta description for SEO"
---
```

### New Blog Posts
Create a new file in `_posts/` with the following naming convention:
`YYYY-MM-DD-title.md`

```yaml
---
layout: post
title: "Post Title"
date: 2024-01-01 12:00:00 +0200
author: "Author Name"
image: "/assets/images/post-image.jpg"
description: "Post description"
---
```

### Adding Photos
1. Upload photos to `assets/images/gallery/`
2. Update the photo gallery in `fotos.md`
3. Ensure optimized images (WebP or compressed JPEG)

## GitHub Pages Deployment

The website is automatically configured for GitHub Pages deployment:

1. Push to the `main` branch
2. GitHub Pages automatically builds the site
3. The site is available at `https://bbewormer.stor.dev`

## Customization

### Colors
Adjust the CSS variables in `assets/css/main.css`:

```css
:root {
  --primary-color: #2c5aa0;
  --secondary-color: #f4a261;
  --accent-color: #e76f51;
  /* ... */
}
```

### Navigation
Update the navigation in `_config.yml`:

```yaml
navigation:
  - title: "Home"
    url: "/"
  - title: "Over Ons"
    url: "/over-ons/"
  # ...
```

## Support

For questions or issues:
- Open an issue on GitHub

## License

© 2025 Brassband Eensgezindheid Wormer. All rights reserved.
