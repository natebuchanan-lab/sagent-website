# Sagent Global website

Plain HTML/CSS, no build step, no framework — just `index.html`, `styles.css`, and `/assets`. Opening `index.html` directly in a browser previews the whole site.

## Deploy (using your existing GitHub + Vercel accounts)

1. Create a new GitHub repo (e.g. `sagent-website`) and push this folder's contents to it — either via the GitHub web UI's "upload files" (drag this whole folder in) or via git if you're comfortable with the CLI.
2. In Vercel: **Add New Project** → **Import** the `sagent-website` repo. Framework preset: **Other** (no build command, no output directory needed — it'll serve the files as-is).
3. Deploy. Vercel gives you a `*.vercel.app` URL immediately to preview.
4. In the Vercel project's **Settings → Domains**, add `sagentglobal.com` (and `www.sagentglobal.com`). Vercel will show you the exact DNS records to add.
5. Wherever sagentglobal.com's DNS is currently managed (Squarespace, per your setup), update the A/CNAME records to what Vercel shows you. Propagation is usually fast (minutes to a couple hours).

## Contact form

The form currently points to a placeholder Formspree endpoint (`YOUR_FORM_ID` in `index.html`). Formspree is free for this volume of traffic and needs no backend:

1. Sign up at formspree.io (free).
2. Create a new form, copy the form ID it gives you.
3. Replace `YOUR_FORM_ID` in `index.html` (search for `formspree.io/f/`) with your real ID.

Until that's done, the form will just fail to submit silently — the direct email/LinkedIn links below the form still work either way.

## Making changes going forward

Tell me what you want changed — copy, a new case study, colors, layout — and I'll edit `index.html`/`styles.css` directly and hand you the updated files (or push to the repo if you'd rather set that up as a connected workflow). No Framer editor, no drag-and-drop.

## Notes

- Brand colors/fonts pulled from the Sagent Global slide design system (navy `#041635`, Arial throughout).
- Logo assets (`assets/logo-leaf.png`, `assets/logo-wordmark.png`) are the same transparent PNGs extracted from your LinkedIn banner work.
- Case study copy and generalization level (e.g. "Australian poultry producer") came straight from what you gave me — flag if you want any of them anonymized further.
