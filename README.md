# Open Source Design Jekyll Theme

A modern, responsive Jekyll theme for the Open Source Design community.

## Features

- Clean, modern design with navy blue and mint green color scheme
- Responsive grid layout with sticky sidebar
- Modular SCSS architecture
- Reusable Jekyll components (layouts and includes)
- Decorative geometric motifs
- Mobile-friendly

## Installation

1. Install Ruby and Bundler if you haven't already
2. Install Jekyll dependencies:
   ```bash
   bundle install
   ```

## Usage

### Running the site locally

```bash
bundle exec jekyll serve
```

Visit `http://localhost:4000` to view the site.

### Building the site

```bash
bundle exec jekyll build
```

The built site will be in the `_site` directory.

## File Structure

```
├── _includes/          # Reusable HTML components
│   ├── header.html
│   ├── footer.html
│   ├── sidebar.html
│   ├── head.html
│   └── hero-motif.html
├── _layouts/           # Page templates
│   ├── default.html
│   └── home.html
├── _sass/              # SCSS partials
│   ├── _variables.scss
│   ├── _base.scss
│   ├── _layout.scss
│   └── _components.scss
├── assets/
│   └── css/
│       └── main.scss   # Main stylesheet (imports all partials)
├── _config.yml         # Jekyll configuration
├── Gemfile             # Ruby dependencies
└── index.md            # Homepage content
```

## Customization

### Colors

Edit `_sass/_variables.scss` to customize the color scheme.

### Site Title and Description

Edit `_config.yml`:

```yaml
title: Your Site Title
description: Your site description
```

### Adding New Pages

Create a new `.md` or `.html` file in the root directory with front matter:

```yaml
---
layout: default
title: Your Page Title
---

Your content here...
```

### Modifying the Sidebar

Edit `_includes/sidebar.html` to change the sidebar content.

### Navigation Links

Edit `_includes/header.html` to modify the navigation menu.

## Deployment

This theme works with:
- GitHub Pages
- Netlify
- Vercel
- Any static hosting service

For GitHub Pages, push to your repository and enable Pages in settings.

## License

Open source - feel free to use and modify!
