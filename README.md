# Orit Cherny Golan — Academic Website

A clean, responsive, pastel-themed personal academic website built with pure HTML + CSS.  
No JavaScript · No backend · No frameworks — ready to host on **GitHub Pages** for free.

---

## 📁 File Structure

```
your-website/
├── index.html          ← Main website (all content)
├── style.css           ← All styles and colours
├── README.md           ← This file
└── images/
    ├── profile.jpg     ← Your profile photo (circular in hero section)
    └── hero-bg.jpg     ← Hero background image
```

---

## 🚀 How to Publish on GitHub Pages (Step by Step)

### Step 1 — Create a GitHub Account
1. Go to [github.com](https://github.com) and click **Sign up** (it's free).
2. Choose a username — this will appear in your website URL.

---

### Step 2 — Create a New Repository
1. After signing in, click the **+** button (top-right) → **New repository**.
2. Name it: `your-username.github.io`  
   *(Replace `your-username` with your actual GitHub username — exactly.)*
3. Set it to **Public**.
4. Click **Create repository**.

---

### Step 3 — Upload Your Files
1. In your new repository, click **Add file** → **Upload files**.
2. Drag and drop all files:
   - `index.html`
   - `style.css`
   - The `images/` folder (with `profile.jpg` and `hero-bg.jpg`)
3. Click **Commit changes**.

---

### Step 4 — Enable GitHub Pages
1. In your repository, go to **Settings** (top menu).
2. Scroll down to the **Pages** section (left sidebar).
3. Under **Branch**, select `main` → `/ (root)`.
4. Click **Save**.
5. Wait 1–3 minutes. Your site will be live at:  
   👉 `https://your-username.github.io`

---

## ✉️ Activating the Contact Form (Formspree)

The contact form is pre-built and styled. To make it send emails to you:

### Step 1 — Create a Formspree Account
1. Go to [formspree.io](https://formspree.io) and sign up for free.
2. The free plan allows **50 submissions/month** — plenty for academic use.

### Step 2 — Create a New Form
1. Click **+ New Form**.
2. Give it a name (e.g., "Website Contact").
3. Enter your email address (where you want to receive messages).
4. Copy the **Form Endpoint URL** — it looks like:  
   `https://formspree.io/f/xabc1234`

### Step 3 — Update index.html
1. Open `index.html` in any text editor (Notepad, TextEdit, etc.).
2. Find this line (search for `YOUR_FORM_ID_HERE`):
   ```html
   action="https://formspree.io/f/YOUR_FORM_ID_HERE"
   ```
3. Replace it with your actual endpoint:
   ```html
   action="https://formspree.io/f/xabc1234"
   ```
4. Save and re-upload `index.html` to GitHub.

✅ Done! Visitors can now send you messages through the website form.  
Your email address is **never visible** on the website.

---

## ✏️ How to Edit Content

All text is inside `index.html`. Every editable section has a clear comment like this:
```
<!-- ╔══════════════════════════════════════════════╗ -->
<!-- ║  EDIT: Change your name here.               ║ -->
<!-- ╚══════════════════════════════════════════════╝ -->
```

### Quick Edit Guide

| What to change | Where to find it in index.html |
|---|---|
| Page title (browser tab) | `<title>` tag in `<head>` |
| Your name in header | `<a class="header-name">` |
| Hero name, title, tagline | Inside `<section class="hero">` |
| About / bio text | Inside `<section id="about">` |
| Education | `.edu-list` inside about section |
| Research interests | `.interests-grid` cards |
| Current projects | `<section id="projects">` |
| Publications | `<section id="publications">` |
| Teaching table | `<section id="teaching">` |
| Talks & conferences | `.talks-grid` cards |
| Phone number | `<section id="contact">` |
| Footer copyright year | `<footer>` section |

---

## 🎨 How to Change Colours

Open `style.css` and find the `:root` block at the top.  
Change any colour value — the whole website updates automatically:

```css
:root {
  --clr-sage:        #A8C5B0;   /* primary green accent */
  --clr-rose:        #E8B9C0;   /* secondary rose accent */
  --clr-lavender:    #C5B8E2;   /* tertiary lavender accent */
  --clr-bg:          #FAFAF8;   /* main background */
  /* ... */
}
```

---

## 🖼️ How to Replace Images

### Profile Photo
1. Prepare a square photo (at least 400×400 pixels).
2. Name it `profile.jpg`.
3. Place it in the `images/` folder (replacing the existing one).
4. Upload to GitHub.

### Hero Background
1. Prepare a landscape photo (at least 1200×800 pixels).
2. Name it `hero-bg.jpg`.
3. Place it in the `images/` folder (replacing the existing one).
4. Upload to GitHub.

**Note:** HEIC photos (iPhone format) may not display in all browsers.  
Always convert to `.jpg` or `.png` before using. Free tools: [CloudConvert](https://cloudconvert.com/heic-to-jpg)

---

## 🔗 Academic Profile Links

All external links are in `index.html`. Current links configured:

| Profile | Link |
|---|---|
| Google Scholar | https://scholar.google.com/citations?user=xFIUFrQAAAAJ&hl=en |
| ORCID | https://orcid.org/0000-0003-0497-0111 |
| YVC Faculty Page | https://yedion.yvc.ac.il/... |

To add a new link (e.g., ResearchGate), find the `profile-links` section and add:
```html
<li><a href="https://www.researchgate.net/profile/YOUR_PROFILE" target="_blank" rel="noopener noreferrer">📄 ResearchGate</a></li>
```

---

## 🛠️ Technical Notes

- **Pure HTML + CSS only** — no JavaScript, no build tools, no dependencies.
- **Responsive** — works on mobile, tablet, and desktop.
- **Google Fonts** loaded via CDN (requires internet connection to display correctly).
- **Formspree** handles form submissions — no server needed.
- **GitHub Pages** hosts everything for free.

---

## 📞 Support

Website built for: **Orit Cherny Golan**  
If you need to make significant changes, you can ask Claude at [claude.ai](https://claude.ai) to help edit specific sections by sharing the relevant part of the HTML or CSS file.
