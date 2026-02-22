# Quick Start Guide

## Immediate Next Steps

### 1. Add Your Images
You need to add two images to `assets/images/`:

- **profile.jpg** - Your profile photo (the one on the right side of your reference design)
- **particle-collision.jpg** - The ATLAS particle collision visualization (the colorful background on the left)

These should be high-resolution images. For best results:
- Profile photo: 600-800px wide
- Particle collision: 1920px wide or larger

### 2. Update Your Links
Edit `_layouts/home.html` and replace the `#` placeholders with your actual links:
- CV link
- Google Scholar profile
- LinkedIn profile
- Email address
- GitHub username
- GitLab username
- Mattermost
- Teams
- X/Twitter handle

### 3. Customize Your Content
The text content is already filled in based on your reference image, but you can:
- Edit `_layouts/home.html` to refine the bio text
- Update `_config.yml` with your actual email
- Add content to the other pages (research.html, talks.html, etc.)

### 4. Test Locally
```bash
cd nicole-hartman-site
bundle install
bundle exec jekyll serve
```
Visit http://localhost:4000 to see your site!

### 5. Deploy to GitHub Pages

1. Create a new repository on GitHub named `username.github.io` (replace username with your GitHub username)
   OR create a project repository with any name

2. Update `_config.yml`:
   - If using `username.github.io`: set `url: "https://username.github.io"` and keep `baseurl: ""`
   - If using a project repo: set `url: "https://username.github.io"` and `baseurl: "/repository-name"`

3. Push your code:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/username/repository.git
git push -u origin main
```

4. Enable GitHub Pages in your repository settings (Settings → Pages → Source: main branch)

Your site will be live in a few minutes!

## Design Features

✨ The site includes:
- Cosmic particle physics aesthetic with animated stars
- Responsive design that works on all devices
- Smooth parallax effects
- Professional navigation with all your sections
- Social media links with hover effects
- Custom fonts: Oswald for headers, IBM Plex Mono for body text
- Gold accent color matching the particle physics theme
- Transparent overlays and glass morphism effects

## Color Customization

Want to change colors? Edit the CSS variables in `assets/css/main.css`:
```css
:root {
    --color-cosmic-black: #0a0a0f;
    --color-particle-gold: #ffd700;
    --color-accent-blue: #4fc3f7;
    /* etc... */
}
```

## Need Help?

The README.md file contains detailed instructions for:
- Installation and setup
- Troubleshooting common issues
- Project structure explanation
- Advanced customization options
