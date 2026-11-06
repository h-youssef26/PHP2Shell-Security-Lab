# Security Lab Notes — GitHub Pages blog

This is a Jekyll blog, ready to publish on GitHub Pages for free.

## 1. Create the GitHub repo

- If you want it at `https://<your-username>.github.io`, name the repo exactly `<your-username>.github.io`.
- Otherwise, name it anything (e.g. `security-lab-notes`) — it'll publish at `https://<your-username>.github.io/security-lab-notes`.

Create it on GitHub (empty, no README) at: https://github.com/new

## 2. Push these files

From this folder:

```bash
git init
git add .
git commit -m "Initial blog: PHP session upload_progress lab writeup"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

## 3. Turn on GitHub Pages

In the repo: **Settings → Pages → Build and deployment → Source: "Deploy from a branch" → Branch: `main` / `(root)` → Save.**

GitHub will build the Jekyll site automatically (no action needed locally) — give it 1–2 minutes, then your blog is live at the URL shown on that same Pages settings screen.

## 4. Editing / adding posts

- Edit `about.md` with your own bio.
- New posts go in `_posts/` named `YYYY-MM-DD-title.md`, each starting with the same `---` front matter block you see in the existing post.
- Edit `_config.yml` to change the blog title/description.

## 5. (Optional) preview locally before pushing

```bash
gem install bundler
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.
