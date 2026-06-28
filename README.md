# Prapti Verma — Portfolio Website

Personal portfolio for Prapti Verma / Poppy Play Design.  
Built with plain HTML + CSS (no frameworks, no build tools).

## File Structure

```
/
├── index.html              ← Homepage (hero, about, projects grid, contact)
├── style.css               ← Shared styles for all pages
├── logo.png                ← Poppy Play Design logo
└── projects/
    ├── kitchen-adventures.html
    ├── my-world.html
    ├── buildables.html
    ├── farmveer.html
    ├── medo.html
    └── art-craft.html
```

## Swapping in your photos

Every image slot is a dashed placeholder with a filename hint. To replace:

### Hero photo (index.html)
1. Add your photo to an `images/` folder as `hero-photo.jpg`
2. In `index.html`, find the `.hero-photo-wrap` div and replace the inner `<div class="photo-placeholder">` with:
   ```html
   <img src="images/hero-photo.jpg" alt="Prapti Verma" class="hero-img" />
   ```
3. Add this CSS: `.hero-img { width:100%; aspect-ratio:3/4; object-fit:cover; border-radius:20px; }`

### About working shots (index.html)
Inside `.about-photos`, replace each `<div class="photo-placeholder">` with an `<img>` tag pointing to your working shot files.

### Project cover images (index.html cards)
Each `.card-img-placeholder` div shows the expected filename. Replace with:
```html
<img src="images/[filename]" alt="[project name]" class="card-img" />
```

### Project page galleries (projects/*.html)
Each `.gallery-placeholder` div shows the expected filename. Replace with:
```html
<img src="../images/[filename]" alt="[description]" class="gallery-img" />
```

## Deploying to GitHub Pages

1. Push this folder to a GitHub repo
2. Go to **Settings → Pages → Source → Deploy from branch (main, / root)**
3. Site is live at `https://yourusername.github.io/repo-name`

## Fonts
- **Fredoka One** — display headings (loaded from Google Fonts)
- **DM Sans** — body text (loaded from Google Fonts)
