# Professional Portfolio Website

A modern, professional portfolio website built with [Eleventy](https://www.11ty.dev/) and [Nunjucks](https://mozilla.github.io/nunjucks/) templates, deployed on GitHub Pages.

## Features

- ✨ Clean, professional design
- 📝 Blog with markdown support
- 🚀 Projects showcase
- 📱 Fully responsive
- 🎨 Modern CSS with custom properties
- 🔍 SEO-friendly
- ⚡ Fast and lightweight
- 🌐 GitHub Pages deployment with CI/CD

## Tech Stack

- **Static Site Generator**: Eleventy 3.x
- **Templating**: Nunjucks
- **Markdown**: markdown-it with plugins
- **Styling**: Custom CSS with CSS Variables
- **Deployment**: GitHub Actions → GitHub Pages

## Project Structure

```
218hosting/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions workflow
├── .vscode/
│   ├── extensions.json         # Recommended extensions
│   ├── settings.json           # VS Code settings
│   └── tasks.json              # Build tasks
├── src/
│   ├── _data/
│   │   └── metadata.js         # Site metadata
│   ├── _includes/
│   │   ├── components/
│   │   │   ├── header.njk      # Site header
│   │   │   └── footer.njk      # Site footer
│   │   └── layouts/
│   │       ├── base.njk        # Base layout
│   │       ├── page.njk        # Page layout
│   │       ├── post.njk        # Blog post layout
│   │       └── project.njk     # Project layout
│   ├── assets/
│   │   ├── css/
│   │   │   └── style.css       # Main stylesheet
│   │   ├── js/
│   │   │   └── main.js         # JavaScript
│   │   └── images/             # Images
│   ├── blog/
│   │   ├── index.njk           # Blog listing
│   │   └── *.md                # Blog posts
│   ├── projects/
│   │   ├── index.njk           # Projects listing
│   │   └── *.md                # Project pages
│   ├── index.njk               # Homepage
│   ├── about.md                # About page
│   └── 404.md                  # 404 page
├── .eleventy.js                # Eleventy configuration
├── .gitignore
├── package.json
└── README.md
```

## Getting Started

### Prerequisites

- Node.js 18+ (includes npm)
- Git

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/218hosting.git
   cd 218hosting
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

   The site will be available at `http://localhost:8080`

## Available Scripts

- `npm start` - Start development server with live reload
- `npm run build` - Build the site for production
- `npm run debug` - Build with debug output
- `npm run clean` - Remove the `_site` directory

## Customization

### Site Metadata

Edit `src/_data/metadata.js` to update:
- Site title and description
- Author information
- Social media links
- URL

### Styling

The main stylesheet is located at `src/assets/css/style.css`. It uses CSS custom properties (variables) for easy theming.

Key variables to customize:
- Colors: `--primary-color`, `--secondary-color`, `--accent-color`
- Typography: `--font-sans`, `--font-mono`
- Spacing: `--spacing-*`

### Adding Content

#### Blog Posts

Create a new `.md` file in `src/blog/`:

```markdown
---
layout: layouts/post.njk
title: "Your Post Title"
description: "A brief description"
date: 2025-11-04
tags:
  - blog
  - your-tag
---

Your content here...
```

#### Projects

Create a new `.md` file in `src/projects/`:

```markdown
---
layout: layouts/project.njk
title: "Project Name"
description: "Project description"
technologies:
  - JavaScript
  - Node.js
github: "https://github.com/username/repo"
demo: "https://demo-url.com"
order: 1
---

Project details...
```

## Deployment

### GitHub Pages Setup

1. Push your code to GitHub
2. Go to repository Settings → Pages
3. Set Source to "GitHub Actions"
4. The site will automatically deploy on push to `main` branch

### Custom Domain (Optional)

1. Add a `CNAME` file to the `public/` directory with your domain
2. Configure DNS with your domain provider
3. Enable "Enforce HTTPS" in GitHub Pages settings

## Development

### VS Code Extensions

Recommended extensions (automatically suggested when you open the project):
- ESLint
- Prettier
- Nunjucks
- Markdown All in One
- Code Spell Checker

### Tasks

Use VS Code tasks (Ctrl+Shift+B or Cmd+Shift+B):
- **Start Eleventy Dev Server** - Default build task
- **Build Site** - Production build
- **Clean Build** - Remove output directory

## Contributing

Feel free to use this template for your own portfolio! If you find bugs or have suggestions, please open an issue.

## License

ISC

## Acknowledgments

- Built with [Eleventy](https://www.11ty.dev/)
- Templating by [Nunjucks](https://mozilla.github.io/nunjucks/)
- Deployed on [GitHub Pages](https://pages.github.com/)

---

**Note**: Remember to update the metadata, content, and links to reflect your personal information before deploying!
