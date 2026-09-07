# NC-11 congressional race model

An interactive, adjustable fundamentals model estimating Jamie Ager's (D) win
probability against Jennifer Balkcom (R) in North Carolina's 11th
Congressional District, November 3, 2026. Runs entirely in the browser —
no backend, no build step.

## Publish it with GitHub Pages (free, ~2 minutes)

1. Create a new repository on GitHub (e.g. `nc11-model`). Public repos get
   free Pages hosting.
2. Upload `index.html` (and this `README.md`) to the repo — either drag
   the file into the GitHub web UI ("Add file" → "Upload files"), or:
   ```
   git init
   git add index.html README.md
   git commit -m "Add NC-11 election model"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/nc11-model.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch",
   pick the **main** branch and the **/ (root)** folder, then **Save**.
5. GitHub builds the site — refresh the Pages settings tab after a minute
   and it'll show your live URL:
   `https://YOUR-USERNAME.github.io/nc11-model/`

That link is what you share. Anyone who opens it gets the full interactive
model — sliders, live simulation, and the comparison table — with nothing
to install.

## Updating it later

Edit `index.html` (the sliders, default values, and comparison figures are
all near the top of the `<script>` block and in the `<body>`), then push
the change. GitHub Pages redeploys automatically within a minute or two.

## Notes

- The only external dependency is Chart.js, loaded from cdnjs at the top
  of the page. If cdnjs is ever unreachable the sliders will still render
  but the chart won't — everything else is self-contained.
- The comparison figures (Kalshi, Cook Political Report, Sabato's Crystal
  Ball) are a late-August 2026 snapshot hardcoded into the page. Edit the
  `compareHtml` block in `index.html` to refresh them.
