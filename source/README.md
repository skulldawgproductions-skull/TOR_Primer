# Tales of Reckoning — World Primer

A no-spoiler, fully responsive primer site for the Tales of Reckoning universe (Earth 5437). Covers the setting, the three factions, the band ("The Belts Oxidation"), key locations, and a spoiler-free teaser for Book One — *Dead Dog Society*.

This is a static site: one HTML file, one CSS file, one small JS file. No build step, no dependencies to install.

## Publish it on GitHub Pages

1. Create a new repository on GitHub (or use an existing one).
2. Add these three files to the repository root: `index.html`, `styles.css`, `script.js`, and the `.nojekyll` file.
3. Push to GitHub:
   ```
   git init
   git add .
   git commit -m "Add Tales of Reckoning primer site"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
   git push -u origin main
   ```
4. On GitHub, go to your repo's **Settings → Pages**.
5. Under **Build and deployment → Source**, choose **Deploy from a branch**.
6. Choose the `main` branch and `/ (root)` folder, then **Save**.
7. GitHub will give you a live URL, typically `https://YOUR-USERNAME.github.io/YOUR-REPO/` — it usually takes a minute or two to go live after the first push.

That's it — no other setup is required. The site works identically whether it's hosted at the root of a `username.github.io` repo or in a subpath like `username.github.io/repo-name/`, since every internal link uses relative paths.

## Updating content later

All the text lives directly in `index.html`, organized into clearly labeled sections (cosmology, factions, band, locations, Book One). Colors, fonts, and layout live in `styles.css`. The only JavaScript (`script.js`) handles the mobile menu toggle and the nav highlight-as-you-scroll behavior — there's nothing else dynamic on the page.

## A note on scope

This site was deliberately built to stay spoiler-free: it introduces the world, the cast, and the premise without revealing plot mechanics, character secrets, or anything from Book One's actual events. If you ever want to expand it (a Book One recap page, character deep-dives, etc.) that should live on separate pages so this primer can stay safe to link to anyone, including people who haven't read the book yet.
