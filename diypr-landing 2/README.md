# DIYPR Landing Page — Setup

## 1. Add your images

Create an `images/` folder next to `index.html` and drop in these files
(exact names matter):

| Filename | Used for | Suggested size |
|---|---|---|
| `images/book-cover.jpg` | Amazon book cover | 900×1200px (portrait) |
| `images/app-screenshot.jpg` | Screenshot inside the phone frame (e.g. one of your onboarding/plan screens) | 780×1600px (portrait, phone aspect) |
| `images/checklist-preview.jpg` | Preview graphic for the free checklist | 600×400px (landscape) |

Until a file exists at that path, the page shows a labeled gray
placeholder in its place instead of a broken image icon — so you can
push to GitHub before every image is ready and swap them in later
without touching the code.

The hero headshot currently pulls from Nikkia's existing Cloudinary
link. It'll keep working as-is, but if you want it independent of
her other site, save it locally as `images/nikkia-headshot.jpg` and
I can point the hero at that instead — just ask.

## 2. Push to GitHub

1. Create a new repo (public) on github.com
2. Add `index.html`, this `README.md`, and your `images/` folder
3. Commit and push

## 3. Go live

**GitHub Pages** (simplest):
Settings → Pages → Source: `main` branch, `/root` → done. Live at
`https://yourusername.github.io/repo-name`

**Cloudflare Pages** (faster CDN, easier custom domain):
Cloudflare dashboard → Pages → Connect to Git → pick the repo → no
build command needed (it's static HTML) → deploy. Live at
`https://your-project.pages.dev`

## 4. Before it's fully live

- The email capture form on the freebie section isn't connected to
  anything yet — it just shows an alert. Wire it to Mailchimp,
  ConvertKit, or whatever tool you use before sending traffic.
