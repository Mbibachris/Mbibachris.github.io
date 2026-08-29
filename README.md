# Christopher Mbiba, Portfolio Website

A free, static portfolio site (plain HTML/CSS/JS, no build step, no framework) covering
research, publications (published / under review / ongoing), projects, experience, and contact info.

## Deploy for free with GitHub Pages

1. Create a new **public** repo on GitHub. For a personal site at the root domain, name it
   exactly `Mbibachris.github.io` (replace with your GitHub username if different).
   Otherwise any repo name works and the site will live at `Mbibachris.github.io/<repo-name>`.
2. From this folder, run:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/Mbibachris/Mbibachris.github.io.git
   git push -u origin main
   ```
3. On GitHub: go to the repo **Settings → Pages**, set Source to `Deploy from a branch`,
   branch `main`, folder `/ (root)`, then Save.
4. Your site will be live in a minute or two at:
   `https://mbibachris.github.io/` (or `https://mbibachris.github.io/<repo-name>/` for a project repo).

No domain purchase or hosting cost is needed. GitHub Pages is free forever for public repos.

## Updating content later

- **Photo**: replace `assets/images/profile.jpg`.
- **CV**: replace `assets/docs/Christopher_Mbiba_CV.pdf` (keep the same filename, or update the
  link in `index.html`'s "Download CV" button).
- **Projects**: the three project cards in the `#projects` section of `index.html` already link
  to real repos. Swap them for others any time by editing the `.project-card` blocks.
- **Published papers**: once you have one, open `index.html`, find the
  `<!-- PLACEHOLDER: no published papers -->` comment under `#publications`, and replace it
  with a `.pub-card` block (copy the format used under "Under Review").
- **Favicon**: add an image at `assets/images/favicon.png` and uncomment the `<link rel="icon">`
  line in the `<head>` of `index.html`.

After editing, just commit and push. GitHub Pages redeploys automatically.
