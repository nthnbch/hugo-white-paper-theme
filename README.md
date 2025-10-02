# Hugo White Paper Theme

A clean, modern Hugo theme featuring Fraktur typography and Material Design principles. Built for readability, elegance, and performance.

![Hugo White Paper Theme](https://nathan.swiss/screenshot.png)

## Features

- **Fraktur Typography**: Beautiful UnifrakturCook headings with Inter body text
- **Material Design**: Clean implementation of Material Design 3 principles
- **Minimalist Layout**: Focus on content with subtle visual enhancements
- **Responsive Design**: Optimized for all screen sizes
- **Fast Loading**: Lightweight and optimized assets
- **SEO Optimized**: Comprehensive meta tags, Schema.org markup, and Open Graph
- **Accessible**: WCAG compliant color contrasts and navigation

## Demo

Live demo: [nathan.swiss](https://nathan.swiss)

## Installation

### Method 1: Git Submodule (Recommended)

```bash
cd your-hugo-site
git submodule add https://github.com/nthnbch/hugo-white-paper-theme themes/hugo-white-paper-theme
```

### Method 2: Clone

```bash
cd your-hugo-site
git clone https://github.com/nthnbch/hugo-white-paper-theme themes/hugo-white-paper-theme
```

### Method 3: Download

Download the theme from GitHub and extract it to `themes/hugo-white-paper-theme`

## Configuration

Update your `config.toml`:

```toml
theme = "hugo-white-paper-theme"
title = "Your Site Name"

[params]
  # Google Analytics (optional)
  google_analytics_id = "G-XXXXXXXXXX"
  
  # Display options
  showIntroContentOnHomepage = true
  showPostsOnHomepage = false
  usePaginationOnHomepage = false
  limitPostsOnHomepage = 1
  sortPostsByDateOldestFirst = false
  addDot = true
  
  # Colors (Material Design)
  highlightColor = '#000000'
  baseColor = "#fdfbff"
  baseOffsetColor = "#f7f2fa"
  headingColor = "#1c1b1f"
  textColor = "#49454f"
  
  # Fonts
  enableGoogleFonts = true 
  googleFontsUrl = "https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&family=UnifrakturCook:wght@700&display=swap"
  fontFamilyHeading = "UnifrakturCook"
  fontFamilyParagraph = "Inter"
  fontFamilyMonospace = "Inter"
```

## Content Structure

```
content/
├── _index.md           # Homepage
├── pages/
│   ├── about.md       # About page
│   └── projects.md    # Projects page
└── posts/
    ├── _index.md      # Blog listing
    └── post-name.md   # Individual posts
```

## Customization

### Colors

The theme uses CSS custom properties for easy color customization:

```css
:root {
  --primary: #000000;
  --on-primary: #ffffff;
  --surface: #fef7ff;
  --on-surface: #1d1b20;
  --on-surface-variant: #49454f;
}
```

Override these in `assets/css/extended/custom.css`

### Typography

Customize fonts in your `config.toml`:

```toml
[params]
  fontFamilyHeading = "Your Heading Font"
  fontFamilyParagraph = "Your Body Font"
  fontFamilyMonospace = "Your Code Font"
```

## Social Links

Add social links in `data/social.json`:

```json
{
  "links": [
    {
      "name": "GitHub",
      "url": "https://github.com/yourusername"
    },
    {
      "name": "LinkedIn",
      "url": "https://linkedin.com/in/yourusername"
    }
  ]
}
```

## Development

### Prerequisites

- Hugo Extended v0.55.0 or higher
- Go (optional, for Hugo Modules)

### Local Development

```bash
# From your Hugo site root
hugo server

# Or from the theme directory
hugo server --source=exampleSite --themesDir=../..
```

## License

MIT License - See [LICENSE](LICENSE) file for details

## Credits

Created by [Nathan Buache](https://nathan.swiss)

## Support

- [Documentation](https://github.com/nthnbch/hugo-white-paper-theme/wiki)
- [Issues](https://github.com/nthnbch/hugo-white-paper-theme/issues)
- [Discussions](https://github.com/nthnbch/hugo-white-paper-theme/discussions)
