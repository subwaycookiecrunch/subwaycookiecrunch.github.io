# Minimalist Personal Portfolio — Shri Raj Bisaria

An ultra-minimalist, typographic personal portfolio website modeled after [x7f.ca](https://x7f.ca) (Alfred Xing's website), customized for **Shri Raj Bisaria**.

## Features

- **Pure Typographic Minimalism**: Clean layout featuring neo-grotesque typography (`Inter` / system font stack), generous whitespace, 40px editorial indentations, and standard `#4080c0` link accents.
- **Accurate Profile Representation**:
  - Highlights your AI/ML research in spectral optimizer geometry (ICLR 2027 paper under review, OpenReview #8176).
  - Founder experience with EdgeCI (YC W27 applicant, Apple Silicon regression gate adopted by RapidMLX).
  - Standout projects: Thinking Budget (Meta PyTorch OpenEnv Hackathon Global Finalist), drift (Homebrew), godmode (NPM), ZenTorrent (Go, #1 trending r/golang), PARASITE EVOLVED, and VOID Zero.
  - Direct links to Email, GitHub (`subwaycookiecrunch`), LinkedIn, and Hugging Face (`lucid987654`).
- **Strict Privacy Compliance**: Zero mention of your college/university name anywhere in the copy or codebase. Education is cleanly stated as *B.Tech in Computer Science and Engineering (Expected 2028)*.
- **Interactive Controls**:
  - **View Toggle** (`compact` vs `full`): Toggle between the pure 1:1 two-paragraph x7f replica and the full editorial index with your research, projects, and achievements.
  - **Theme Toggle** (`light` vs `dark`): Respects system color scheme by default and allows smooth manual switching with persistence in `localStorage`.
- **Zero Framework Overhead**: Vanilla HTML5, CSS3, and modern JavaScript. Blazing fast, zero build steps, 100% lighthouse score.

## Directory Structure

```
portfolio/
├── index.html        # Main HTML markup
├── style.css         # Minimalist stylesheet with light/dark theme & responsive styles
├── script.js         # View switcher (compact/full) and theme toggle
├── avatar.svg        # Modern circular monogram avatar
└── README.md         # Documentation & deployment guide
```

## How to Preview Locally

Open `index.html` directly in any web browser:
```bash
open index.html
```
Or start a local development server:
```bash
python3 -m http.server 8000
```
Then visit `http://localhost:8000`.

## Adding a Custom Photo Avatar

To use a personal photograph instead of the monogram SVG:
1. Save your square photo as `avatar.jpg` or `avatar.png` inside this folder.
2. In `index.html`, update the `<img>` tag on line 18:
   ```html
   <img class="icon" src="avatar.jpg" alt="Shri Raj Bisaria" width="24" height="24">
   ```

## Deployment Options

Because this is a pure static site with no build steps, deployment is instant:

### 1. GitHub Pages (Free)
1. Push this folder to a GitHub repository (e.g. `subwaycookiecrunch/subwaycookiecrunch.github.io`).
2. In GitHub repository **Settings** > **Pages**, set branch to `main` and folder to `/ (root)`.
3. Your site will be live at `https://subwaycookiecrunch.github.io` in under 60 seconds.

### 2. Vercel or Netlify (Free)
- Drag and drop this folder directly into the [Vercel](https://vercel.com) or [Netlify](https://netlify.com) dashboard.

### 3. Cloudflare Pages (Free)
- Connect your GitHub repository to Cloudflare Pages with build command left empty and output directory set to `/`.
