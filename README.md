# Barsa Rana — Portfolio Site

A single-file, no-build-step portfolio site. Just edit `index.html` and deploy — no npm, no framework, no build process needed.

## 1. Before you deploy — what to edit

Open `index.html` in any text editor (VS Code recommended) and update:

| Section | What to change |
|---|---|
| Hero | Tagline / one-line pitch if you want to tweak the wording |
| `resume.pdf` link | Either upload a `resume.pdf` file next to `index.html`, or change the link to your Google Drive/LinkedIn resume link |
| Projects (3 cards) | Replace title, description, tags, and the `href="#"` links with your real GitHub repo / live demo links |
| Experience | Add your real company name and 2–3 bullet points about what you actually did |
| Contact section | Replace `your.email@example.com`, LinkedIn, and GitHub links with your real ones |

Everything else (colors, layout, fonts) is ready to go.

## 2. Deploy for free — 3 options

### Option A: GitHub Pages (recommended)
Best if you want a permanent, professional link tied to your GitHub — which recruiters will look at anyway.

1. Create a free GitHub account if you don't have one: https://github.com
2. Create a new repository, e.g. `portfolio` (make it **Public**)
3. Upload `index.html` (and `resume.pdf` if you have one) — either drag-and-drop via the GitHub web UI ("Add file" → "Upload files") or via git:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/portfolio.git
   git push -u origin main
   ```
4. In the repo, go to **Settings → Pages**
5. Under "Source", select **Deploy from a branch** → branch `main`, folder `/ (root)` → Save
6. Wait ~1 minute. Your site will be live at:
   ```
   https://YOUR-USERNAME.github.io/portfolio/
   ```
7. **Tip:** if you name the repo `YOUR-USERNAME.github.io` instead of `portfolio`, your site becomes `https://YOUR-USERNAME.github.io/` (no extra path) — cleaner for a CV link.

### Option B: Netlify (fastest, no GitHub required)
Good if you want something live in under a minute.

1. Go to https://app.netlify.com/drop
2. Drag the `portfolio` folder straight into the browser window
3. Netlify instantly gives you a live URL like `https://random-name-123.netlify.app`
4. Optional: in Site settings → change site name to something like `barsa-rana.netlify.app`

### Option C: Vercel
Similar to Netlify, also free and fast — good if you're already familiar with it.

1. Go to https://vercel.com and sign up (can use GitHub login)
2. Click "Add New → Project", import your GitHub repo (push the folder to GitHub first, same as Option A steps 2–3)
3. Leave build settings blank (static HTML needs no build command) → Deploy
4. You'll get a URL like `https://portfolio-yourname.vercel.app`

## 3. Optional: custom domain

All three options support a free custom domain connection if you later buy one (e.g. from Namecheap, ~$10–15/year for a `.com`). Instructions:
- GitHub Pages: Settings → Pages → Custom domain
- Netlify: Site settings → Domain management → Add custom domain
- Vercel: Project → Settings → Domains

Not necessary to get started — the free subdomain is perfectly fine to put on a CV.

## 4. Recommended: which one to pick

For a job-search CV link, **GitHub Pages** is the strongest choice — it's free forever, looks credible to technical recruiters, and having the repo public also doubles as a visible sign you use git/version control.
