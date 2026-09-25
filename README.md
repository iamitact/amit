# Twelve Clothing

The Twelve Clothing website: a scroll-driven 3D story for the Nocturne Polo, plus a demo storefront.

This repository is **ready for GitHub Pages as-is**. The files at the top level (`index.html`, `assets/`, `renders/`) are the finished website. The editable project is in [`source/`](source/).

## Publish (about 2 minutes)

1. On GitHub, create a new **public** repository.
2. Click **Add file → Upload files**. Open the folder you extracted from the ZIP, select **everything inside it** (`index.html`, `assets`, `renders`, `source`, `favicon.svg`, `README.md`, `.nojekyll`), and drag it all into the upload box. Upload the files **inside** the folder, not the folder itself, and not the ZIP. Then click **Commit changes**.
3. Go to **Settings → Pages**. Under *Build and deployment*, set **Source: Deploy from a branch**, **Branch: `main`**, folder **`/ (root)`**, then click **Save**.
4. Wait a minute or two, then refresh the Pages settings page. It shows your live link: `https://<your-username>.github.io/<repository-name>/`

Check: in your repository's file list, `index.html` must sit at the top level, next to `assets` and `renders`. If you see a single folder instead, you uploaded the folder itself. Delete it and upload its contents.

## Run it on your computer

```bash
cd source
npm ci
npm run dev        # then open http://localhost:5173
```

Opening `index.html` by double-click (as a `file://` page) won't work, because browsers block the site's JavaScript on local files. Use `npm run dev`, or `npm run preview` inside `source/`.

## Change the site

Edit files in `source/`, then run `npm run build:pages` inside `source/` to regenerate the top-level website, and commit. Full details are in [`source/README.md`](source/README.md).
