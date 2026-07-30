# Mugilan Purushothaman — Resume Site

Interactive resume site with expandable project and skill bubbles. Single self-contained `index.html` — no build step, no dependencies.

## Publish on GitHub Pages

1. Create a new repository on GitHub named `<your-username>.github.io` (this makes it your personal site at `https://<your-username>.github.io`). Any other repo name works too — the site will then live at `https://<your-username>.github.io/<repo-name>`.
2. From this folder, run:

   ```bash
   git init
   git add index.html README.md
   git commit -m "Resume site with interactive bubbles"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages → Build and deployment** → Source: *Deploy from a branch* → Branch: `main` / `(root)` → Save.
4. Your site goes live in about a minute.

## Editing content

All content lives in the `ITEMS` array inside `index.html` (bottom `<script>` block). Each entry has:

- `type` — `"project"` or `"skill"` (drives the filter tabs)
- `size` — `"lg"`, `"md"`, or `"sm"` (bubble size)
- `icon`, `name`, `tag` — what shows on the bubble
- `meta`, `desc`, `high`, `tech` — what shows when the bubble expands
- `grad` — the two gradient colors
- `link` — optional external link (used on Pict-o-view)

Update the Pict-o-view App Store URL in that entry with your real listing link.
