# Quick Start Guide

## First Steps

### 1. Update Site Metadata

Edit `src/_data/metadata.js`:

```javascript
module.exports = {
  title: "Your Name",  // Update with your name
  description: "Your description",
  url: "https://yourusername.github.io/218hosting",  // Update username
  author: "Your Name",
  email: "mailto:your.email@example.com",  // Update email
  github: "https://github.com/yourusername",  // Update username
  linkedin: "https://linkedin.com/in/yourprofile",  // Update profile
};
```

### 2. Test Locally

```bash
npm start
```

Visit `http://localhost:8080` to see your site.

### 3. Customize Content

- **Homepage**: Edit `src/index.njk`
- **About Page**: Edit `src/about.md`
- **Add Blog Posts**: Create `.md` files in `src/blog/`
- **Add Projects**: Create `.md` files in `src/projects/`

### 4. Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g., `218hosting`)
2. Initialize git and push:

```bash
git init
git add .
git commit -m "Initial commit: Professional portfolio setup"
git branch -M main
git remote add origin https://github.com/yourusername/218hosting.git
git push -u origin main
```

3. Enable GitHub Pages:
   - Go to your repository → Settings → Pages
   - Source: "GitHub Actions"
   - The workflow will automatically deploy your site

4. Your site will be live at: `https://yourusername.github.io/218hosting`

### 5. VS Code Tasks

Press `Ctrl+Shift+B` (or `Cmd+Shift+B` on Mac) to run:
- Start Eleventy Dev Server
- Build Site
- Clean Build

## Next Steps

- Replace sample content with your own
- Add your projects
- Write blog posts
- Customize colors in `src/assets/css/style.css`
- Add your photos to `src/assets/images/`

## Tips

- Use the sample blog post and project as templates
- Markdown files automatically get processed with your layout
- Front matter (the `---` section at top of files) controls metadata
- Collections are automatically generated from `blog/` and `projects/` folders

Enjoy building your portfolio! 🚀
