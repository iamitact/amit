# Twelve Clothing

The Twelve Clothing website: a scroll-driven 3D story for the Nocturne Polo, plus a demo storefront.

This repository is **ready for GitHub Pages as-is**. The files here are the finished website. The editable project is packed in `twelve-clothing-source.zip`.

## What must be in the repository

```
index.html
favicon.svg
.nojekyll
README.md
twelve-clothing-source.zip
assets/     ← 10 files (code, styles, fonts) — REQUIRED, the page is blank without it
renders/    ← 30 images                     — REQUIRED
```

## Publish with the GitHub website

1. Open your repository on GitHub and click **Add file → Upload files**.
2. In File Explorer, open the folder you extracted, press **Ctrl + A** to select everything (including the `assets` and `renders` **folders**), and **drag** the selection onto the GitHub upload box.
   - Drag and drop is needed: the *“choose your files”* button can't select folders.
   - Wait until the list shows files such as `assets/index-….js` and `renders/story-hero-1600.webp`, then click **Commit changes**.
3. **Settings → Pages**: set **Source: Deploy from a branch**, **Branch: `main`**, folder **`/ (root)`**, then **Save**.
4. Wait 1–2 minutes and open `https://<your-username>.github.io/<repository-name>/`. Press **Ctrl + F5** to bypass the cache.

**Check:** on the repository's main page you must see the `assets` and `renders` folders. If they are missing, the site shows a black page. Upload them again by dragging the two folders in.

## Run it on your computer

Extract `twelve-clothing-source.zip`, then in that folder:

```bash
npm ci
npm run dev        # open http://localhost:5173
```

Double-clicking `index.html` (a `file://` page) won't work, because browsers block the site's scripts on local files.
