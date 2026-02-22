# Nicole Hartman - Personal Website

A cosmic-themed academic website built with Jekyll for GitHub Pages.

## Setup Instructions

### Prerequisites
- Ruby (version 2.7 or higher)
- Bundler
- Git

### Local Development

1. Clone this repository:
```bash
git clone https://github.com/yourusername/yourrepository.git
cd yourrepository
```

2. Install dependencies:
```bash
bundle install
```

3. Run the site locally:
```bash
bundle exec jekyll serve
```

4. Open your browser and visit `http://localhost:4000`

### Customization

#### Adding Your Images
1. Place your profile photo in `assets/images/` and name it `profile.jpg`
2. Place your particle collision background image in `assets/images/` and name it `particle-collision.jpg`

#### Updating Content
- Edit `_layouts/home.html` to update the homepage content
- Edit individual page files (`research.html`, `talks.html`, etc.) for other pages
- Update social media links in `_layouts/home.html`

#### Styling
- All CSS is in `assets/css/main.css`
- Color scheme can be adjusted in the `:root` variables at the top of the CSS file

### Deploying to GitHub Pages

1. Create a new repository on GitHub (e.g., `username.github.io`)

2. Update `_config.yml`:
   - Change `url` to: `https://username.github.io`
   - If using a project repository, set `baseurl` to: `/repository-name`

3. Push your code:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/username/repository.git
git push -u origin main
```

4. Enable GitHub Pages:
   - Go to repository Settings
   - Navigate to Pages
   - Under "Source", select the `main` branch
   - Click Save

5. Your site will be live at `https://username.github.io/repository-name`

### Project Structure
```
nicole-hartman-site/
├── _config.yml          # Jekyll configuration
├── _layouts/            # Page templates
│   ├── default.html
│   └── home.html
├── _includes/           # Reusable components
│   └── navigation.html
├── assets/
│   ├── css/
│   │   └── main.css
│   ├── js/
│   │   └── main.js
│   └── images/          # Add your images here
├── index.html           # Homepage
├── research.html        # Research page
├── talks.html           # Talks page
├── teaching.html        # Teaching page
├── miscellaneous.html   # Miscellaneous page
└── Gemfile              # Ruby dependencies
```

### Features
- Responsive design that works on all devices
- Cosmic particle physics aesthetic with animated stars
- Smooth animations and transitions
- Easy to customize colors and fonts
- GitHub Pages compatible

### Updating Links
Update your social media and professional links in `_layouts/home.html`:
- CV link
- Google Scholar
- LinkedIn
- Email
- GitHub
- GitLab
- Mattermost
- Teams
- X (Twitter)

### Need Help?
If you encounter any issues, check:
1. Ruby version: `ruby -v`
2. Bundler installation: `bundle -v`
3. Jekyll version: `bundle exec jekyll -v`

Common issues:
- If gems fail to install, try: `bundle update`
- If the site won't build, check for syntax errors in YAML front matter
- Make sure all file paths use forward slashes `/`
