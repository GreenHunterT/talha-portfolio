# Talha Rozajac — Portfolio

Personal portfolio site for Talha Rozajac, Junior Web Developer and Workflow Systems Builder.

Built with plain HTML, CSS, and a small amount of vanilla JavaScript. No build tools, no frameworks, no dependencies.

---

## What this is

A static single-page portfolio that presents:
- A hero section with name, title, and positioning statement
- Two deployed project cards (FlowDesk and Sahifa)
- A skills breakdown
- A short about section
- Contact links

---

## Run locally

No install step needed. Open `index.html` directly in a browser:

```
File > Open File > index.html
```

Or use any static file server. With VS Code and the Live Server extension:

1. Right-click `index.html` in the Explorer panel
2. Click **Open with Live Server**

---

## Update project links

All project URLs are in `index.html` inside the `#projects` section.

Each project card contains:
- `href` on the **Live Project** button — update this with the live Vercel URL
- `href` on the **GitHub** button — update this with the specific repo URL when ready

Search for `flowdesk-psi-seven.vercel.app` and `sahifa-plain-text-pdf.vercel.app` to find them quickly.

---

## Add a profile photo

1. Place your photo in the project folder (e.g. `photo.jpg`)
2. In `index.html`, find the `<div class="hero-photo">` section
3. Replace the `<div class="photo-placeholder">...</div>` block with:

```html
<img src="photo.jpg" alt="Talha Rozajac" class="profile-photo" />
```

4. Add this rule to `style.css`:

```css
.profile-photo {
  width: 200px;
  height: 200px;
  border-radius: 14px;
  object-fit: cover;
  border: 2px solid var(--clr-border);
}
```

---

## Deploy to Vercel

### First deploy

1. Push the project to a GitHub repository
2. Go to [vercel.com](https://vercel.com) and sign in
3. Click **Add New Project**
4. Import your GitHub repository
5. Leave all settings as default (Vercel detects static HTML automatically)
6. Click **Deploy**

Vercel will give you a live URL immediately.

### Update the site

Push any change to the `main` branch and Vercel redeploys automatically.

### Custom domain (optional)

In the Vercel project dashboard go to **Settings > Domains** and add your domain.

---

## File structure

```
talha-portfolio/
  index.html   — all page content and structure
  style.css    — all styles including responsive layout
  app.js       — mobile nav toggle only
  README.md    — this file
```
