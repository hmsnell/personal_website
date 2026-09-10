# Personal Site Template

A small, dependency-free personal website: plain HTML, CSS, and a sprinkle of
JS. No build step, no framework, no npm install — clone it, edit it, push it.

**[View a live preview →](#)** *(replace with your GitHub Pages URL once deployed)*

## What's in here

```
.
├── index.html          # all page content lives here
├── css/style.css        # design tokens + layout, edit :root for colors/fonts
├── js/main.js           # mobile nav toggle + footer year, ~20 lines
├── assets/              # placeholder images — swap these for your own
└── README.md
```

Sections included: hero, work (one featured project + a grid of smaller
ones), writing/notes list, about, and a contact footer. Delete or duplicate
any section — it's all plain HTML, nothing is generated.

## Quick start

1. **Use this template.** Click "Use this template" on GitHub (or fork/clone
   it) to get your own copy.
2. **Edit the content.** Open `index.html` and search for `[EDIT]` comments —
   they mark every place with placeholder text (name, bio, projects, writing,
   links). Replace as you go.
3. **Swap the design tokens if you want a different look.** The top of
   `css/style.css` has a `:root` block with all the colors and fonts named —
   change those and the whole site restyles.
4. **Replace the images.** Drop your own files into `assets/` (e.g.
   `portrait.jpg`, `project-01.jpg`) and update the `src` attributes in
   `index.html`. Or delete the `<img>` tags entirely for a text-only site.
5. **Preview locally.** Just open `index.html` in a browser — no server
   needed. (Or run `python3 -m http.server` from the project root and visit
   `http://localhost:8000`.)

## Deploying to GitHub Pages

1. Push this repo to GitHub.
2. In the repo, go to **Settings → Pages**.
3. Under "Build and deployment", set **Source** to `Deploy from a branch`,
   pick the `main` branch and the `/ (root)` folder, then save.
4. GitHub will publish the site at `https://<your-username>.github.io/<repo-name>/`.
   If you name the repo `<your-username>.github.io`, it publishes at the
   root domain instead (`https://<your-username>.github.io`).
5. Optional: to use a custom domain, add a `CNAME` file to the repo root
   containing just your domain (e.g. `janedoe.com`), and point your domain's
   DNS at GitHub Pages per
   [GitHub's custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

Pages usually take a minute or two to go live after the first push.

## Customization notes

- **Fonts** are loaded from Google Fonts in `index.html`'s `<head>` — swap
  the `<link>` tags and the `--font-*` variables in `style.css` together.
- **Colors** are all named CSS variables in `style.css` (`--bg`, `--ink`,
  `--accent`, etc.) — no colors are hardcoded elsewhere in the file.
- **Nav links** use anchor links (`#work`, `#about`, …) matching section
  `id`s — add or remove sections and update both.
- **No JavaScript is required** for the site to work; `main.js` only handles
  the mobile menu and the footer's copyright year.

## License

MIT — see `LICENSE`. Use this for anything, no attribution required (though
always appreciated).
