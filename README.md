# Affective Computing Group — Lab Website

Vanderbilt University · College of Connected Computing · Jonathan Gratch

## Quick Start

### 1. Install Jekyll
```bash
gem install bundler jekyll
bundle install
```

### 2. Run locally
```bash
bundle exec jekyll serve
# Open http://localhost:4000
```

### 3. Deploy to GitHub Pages
1. Push this folder to a GitHub repo (e.g. `username/acg-lab`)
2. Go to **Settings → Pages**
3. Set source to **main branch / root**
4. Done — your site will be live at `https://username.github.io/acg-lab`

---

## Updating Content (no coding needed)

### Add/edit students → `_data/people.yml`
```yaml
phd:
  - name: Jane Smith
    initials: JS
    year: 2nd year
    topic: Emotion recognition in VR
```

### Add publications → `_data/publications.yml`
```yaml
- year: 2025
  title: Your Paper Title Here
  venue: ACM CHI 2025
  url: https://link-to-paper.com
```

### Add news → `_data/news.yml`
```yaml
- date: May 2025
  text: Jane's paper accepted to ACM CHI 2025!
```

### Add lab photos
Replace the placeholder `<div class="ph-placeholder">` blocks in `index.html` with:
```html
<div class="ph ph-main">
  <img src="/assets/img/lab-photo.jpg" alt="Lab photo">
</div>
```
Put your images in `assets/img/`.

---

## File Structure
```
acg-lab/
├── _config.yml          ← site settings (name, email, etc.)
├── _data/
│   ├── people.yml       ← students & alumni
│   ├── publications.yml ← papers
│   └── news.yml         ← lab news
├── _layouts/
│   └── default.html     ← shared nav + footer
├── assets/css/
│   └── main.css         ← all styles
├── pages/
│   ├── research.html
│   ├── people.html
│   ├── publications.html
│   └── contact.html
└── index.html           ← home page
```
