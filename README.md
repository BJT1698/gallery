# Gallery 🖼️

A simple photo gallery website built with [Hugo](https://gohugo.io/) and the [hugo-theme-gallery](https://github.com/nicokaiser/hugo-theme-gallery) theme by [Nico Kaiser](https://github.com/nicokaiser).

## Structure

```
/
├── content/              # Gallery content (photos and albums)
│   ├── _index.md         # Home page configuration
│   ├── about.md          # About page
│   └── [album-folders]/  # Individual photo albums
├── static/               # Static files (robots.txt, favicon, etc.)
├── layouts/              # Custom layouts (if needed)
├── assets/               # Custom assets (if needed)
├── hugo.toml             # Hugo configuration
└── public/               # Built site (generated)
```

## Adding a New Album

1. Create a new folder in `content/`, e.g., `content/my-album/`
2. Add an `index.md` with front matter:

```yaml
---
title: "My Album"
description: "Description of the album"
date: 2025-01-01
featured_image: feature.jpg
---
```

3. Add your photos to the folder
4. Build with `hugo`

## Adding Photos to an Existing Album

Simply drop images into the album folder. Supported formats: JPG, PNG, WEBP, etc.

Optional: Add EXIF data (title, date) to images for automatic captioning.

## Commands

- `hugo` - Build the site
- `hugo server` - Start local development server
- `./build_and_deploy` - Build and push to remote

## Deployment

The site is automatically deployed to GitHub Pages via GitHub Actions on push to main.

## Theme

Based on [hugo-theme-gallery](https://github.com/nicokaiser/hugo-theme-gallery) by [Nico Kaiser](https://github.com/nicokaiser).

## License

Content and photos are personal. Theme is MIT licensed.
