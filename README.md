# Marci Metzger Homes — redesigned Home page

Single file: `index.html`. No build step, no dependencies except Google Fonts (loaded via CDN link). Photos live in the `images/` folder alongside it.

## What's in the page

- **Hero**: full-bleed photo with headline overlay, hotlinked directly from the original site's CDN (`img1.wsimg.com`) — this is the real hero image from marcimetzger.com.
- **Agent section**: Marci's real portrait, also hotlinked from the original site's CDN.
- **Get It Sold**: stat ticker plus three image cards using real property photos (`images/1.webp`, `images/2.webp`, `images/3.webp`).
- **Photo gallery**: an auto-playing slideshow (not a static grid) with captions, an "Ask about this home/community" call-to-action button on each slide, prev/next arrows, and a clickable thumbnail strip. Pulls from `images/pg1.webp` through `images/pg7.webp` plus a couple others.
- **Services**: three image cards using `images/Os3.webp`, `images/0s1.webp`, and `images/0s2.webp`.
- **Listing search and contact form**: front-end only — no live MLS feed or email backend wired up. Both give the visitor clear feedback instead of silently doing nothing.

## Image file requirements

Everything in the `images/` folder needs to match these filenames exactly (case-sensitive):

```
images/1.webp
images/2.webp
images/3.webp (currently unused on the page, safe to leave or remove)
images/0s1.webp
images/0s2.webp
images/Os3.webp
images/pg1.webp
images/pg2.webp
images/pg3.webp
images/pg4.webp
images/pg5.webp
images/pg6.webp
images/pg7.webp
```

## Deploying for free

**Netlify Drop (no account needed for a first look)**
1. Go to https://app.netlify.com/drop
2. Drag `index.html` (and the `images` folder) into the browser window
3. You get a live URL immediately

**GitHub Pages (what this repo already uses)**
1. Repo Settings → Pages → source set to the `main` branch, root folder
2. Site is live at `https://<username>.github.io/<repo>/`
3. `index.html` must sit at the repo root — GitHub Pages serves it automatically over any README

## Notes on image sourcing

Two images (hero background, agent portrait) are hotlinked straight from marcimetzger.com's own CDN and will always load correctly for site visitors. All other photos are real property/lifestyle photos supplied directly and uploaded into `images/`.
