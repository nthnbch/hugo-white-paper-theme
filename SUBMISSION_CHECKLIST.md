# Hugo Themes Repository Submission Checklist

This checklist ensures the theme is ready for submission to the official Hugo themes repository.

## ✅ Required Files

- [x] **LICENSE** - MIT license in place
- [x] **README.md** - Comprehensive documentation with:
  - Theme description
  - Screenshot/demo
  - Installation instructions (3 methods)
  - Configuration examples
  - Features list
  - Customization guide
- [x] **theme.toml** - All required metadata:
  - `name`
  - `license`
  - `licenselink`
  - `description`
  - `homepage`
  - `demosite`
  - `tags`
  - `features`
  - `min_version`
  - `author` (with name, homepage)
- [x] **CHANGELOG.md** - Version history
- [x] **CONTRIBUTING.md** - Contribution guidelines

## ✅ ExampleSite Requirements

- [x] **exampleSite/** folder exists
- [x] **config.toml** - Working configuration
- [x] **content/** - Sample content (no Winston/1984 references)
- [x] **data/** - Sample data files (author.json, social.json)
- [x] Builds successfully: `hugo --source=exampleSite --themesDir=../..`

## ✅ Theme Structure

- [x] **layouts/** - All template files
- [x] **assets/** - SCSS/JS source files
- [x] **archetypes/** - Content templates (clean, generic)
- [x] **.gitignore** - Properly configured
- [x] No build artifacts committed (public/, resources/)

## ✅ Code Quality

- [x] Clean, commented code
- [x] No references to other themes (Winston removed)
- [x] Follows Hugo best practices
- [x] Responsive design
- [x] SEO optimized (meta tags, Schema.org)

## ✅ Screenshots

- [ ] **images/screenshot.png** (1500x1000px) - Full page screenshot
- [ ] **images/tn.png** (900x600px) - Thumbnail

## 🚀 Next Steps

1. **Create screenshots** (currently marked as TODO)
2. **Create GitHub repository**: `nthnbch/hugo-white-paper-theme`
3. **Push theme to GitHub**
4. **Test installation from GitHub**: 
   ```bash
   hugo new site test-site
   cd test-site
   git init
   git submodule add https://github.com/nthnbch/hugo-white-paper-theme themes/hugo-white-paper
   ```
5. **Submit to Hugo themes**: Fork https://github.com/gohugoio/hugoThemes and create PR

## 📝 Notes

- Theme name: **Hugo White Paper**
- GitHub: https://github.com/nthnbch/hugo-white-paper-theme
- Demo site: https://nathan.swiss
- License: MIT
- Hugo min version: 0.115.0

## 🎨 Theme Features

- Fraktur typography (UnifrakturCook) for headings
- Inter sans-serif for body text
- Material Design 3 color system
- Fully responsive
- SEO optimized (Open Graph, Twitter Cards, Schema.org)
- Clean, minimal design
- Social links support
- Blog pagination
- Syntax highlighting
