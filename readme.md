# Digital Twin Technologies | DIIM Lab

A modern, modular website showcasing Digital Twin research projects.

## 📁 File Structure

```
diim-digital-twin-site/
├── index.html                  # Homepage
├── css/
│   ├── styles.css              # Main styles (shared across all pages)
│   └── project-page.css        # Project detail page styles
├── js/
│   └── main.js                 # Shared JavaScript
└── projects/
    └── project-template.html   # Copy this for new project pages
```

## 🚀 Deploying to GitHub Pages

1. Create a new GitHub repository
2. Upload all files maintaining the folder structure
3. Go to **Settings** → **Pages**
4. Select **main** branch, **/ (root)** folder
5. Save — site will be live at `https://username.github.io/repo-name/`

## ➕ Adding a New Project

### Step 1: Add card to homepage

Open `index.html` and copy this block inside `<div class="projects__grid">`:

```html
<article class="project-card">
  <div class="project-card__image">
    <img src="images/your-image.jpg" alt="Project title" />
    <div class="project-card__overlay">
      <span class="project-card__tag">Category</span>
      <h3 class="project-card__title">Project Title</h3>
      <span class="project-card__author">Researcher Name</span>
    </div>
  </div>
  <div class="project-card__content">
    <p class="project-card__description">
      Short description for the homepage card.
    </p>
    <a href="projects/your-project.html" class="btn btn--link">
      Learn more
      <svg
        fill="none"
        stroke="currentColor"
        stroke-width="2"
        viewBox="0 0 24 24"
      >
        <path d="M5 12h14M12 5l7 7-7 7" />
      </svg>
    </a>
  </div>
</article>
```

### Step 2: Create project detail page

1. Copy `projects/project-template.html`
2. Rename to `projects/your-project.html`
3. Update the content (title, description, images, videos, publications)

## 🎨 Customizing Colors

Edit CSS variables in `css/styles.css`:

```css
:root {
  --primary: #0ea5e9; /* Change main color */
  --primary-dark: #0284c7;
  --primary-light: #38bdf8;
  --accent: #06b6d4;
  /* ... */
}
```

## 📹 Embedding Videos

In project pages, replace `VIDEO_ID` with your YouTube video ID:

```html
<iframe src="https://www.youtube.com/embed/YOUR_VIDEO_ID"></iframe>
```

## 📱 Responsive

All pages are fully responsive out of the box.

---

© 2025 DIIM Lab, University of Guelph
