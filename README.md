# NexusPlay — Gaming Referral Hub

A professional, fully static website for sharing game referral links — built to deploy on GitHub Pages in minutes.

## 📁 Project Structure

```
/
├── index.html              ← Home page
├── css/
│   └── style.css           ← All shared styles
├── js/
│   └── main.js             ← Shared JavaScript
└── pages/
    ├── games.html          ← Game library with filter + referral links
    ├── about.html          ← About page with team & timeline
    └── contact.html        ← Contact form with FAQ
```

## 🚀 Deploy to GitHub Pages

1. Create a new GitHub repository (e.g. `my-game-hub`)
2. Upload all files keeping the folder structure exactly as-is
3. Go to **Settings → Pages**
4. Under **Source**, select `Deploy from a branch`
5. Choose `main` branch and `/ (root)` folder
6. Click **Save** — your site will be live at `https://yourusername.github.io/my-game-hub`

## ✏️ Adding Your Own Referral Links

Open `pages/games.html` and find any game card block. Replace the `href` and `data-url` values:

```html
<a href="YOUR_REFERRAL_URL" target="_blank" class="btn btn-primary">Play Now ↗</a>
<button class="btn btn-outline btn-sm copy-btn" data-url="YOUR_REFERRAL_URL">Copy Link</button>
```

To add a brand new game card, copy an existing `.card.game-card` block and update:
- `data-genre` attribute (rpg / shooter / moba / strategy / sports)
- The emoji icon and background gradient in `.gc-thumb`
- Title, rating, description, reward text, and referral URLs

## 🎨 Customization

All color and font settings live at the top of `css/style.css` inside `:root { }`:

```css
--accent: #6c63ff;       /* Main purple — change to your brand color */
--accent-2: #00d4ff;     /* Cyan accent */
--bg-primary: #080b14;   /* Main background */
```

## ✅ Features

- Responsive on all screen sizes
- Live genre filter tabs on Games page
- Live search on Games page
- One-click copy referral link button
- Animated stat counters
- Scroll-reveal animations
- FAQ accordion on Contact page
- Contact form with topic selector
- No dependencies — pure HTML, CSS, JavaScript
