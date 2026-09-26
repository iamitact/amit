# Twelve Clothing

The Twelve Clothing website: a multi-page storefront (Home, Shop, product pages, Story, Lookbook, About, Contact, Bag) with a 3D editorial story.

This folder is **ready for GitHub Pages as-is**. The files here are the finished website. The editable project is packed in `twelve-clothing-source.zip`.

> **Preview, not final.** Products are 3D concept renders with prices, sizes and availability "to be confirmed". Business details are pending, and online payment is not active (the site says so and takes no orders). What the client still needs to supply is listed in `docs/CLIENT-CHECKLIST.md` inside the source ZIP.

## Publish

This folder has 76 files, under the GitHub web uploader's limit of 100 per upload.

**With the website:** open the repository → **Add file → Upload files**. In File Explorer select **everything** in this folder (Ctrl + A, including the folders and the hidden `.nojekyll`) and **drag** it onto the upload box. The "choose your files" button can't select folders. Check that the list shows paths such as `assets/…`, `shop/…` and `renders/…`, then commit.

**With Git:**

```bash
git clone https://github.com/<user>/<repo>.git
# copy everything from this folder into the clone (including .nojekyll), then:
git add -A
git commit -m "Publish Twelve Clothing site"
git push
```

**Then:** Settings → Pages → **Deploy from a branch** → `main` → `/ (root)` → Save. Pages are served at `https://<user>.github.io/<repo>/`, `…/shop/`, `…/about/` and so on.

This build's absolute links (canonical, sitemap, 404 page) point at `https://iamitact.github.io/amit/`. For another repository, rebuild from source with `SITE_URL=https://<user>.github.io/<repo>/`.

## Edit and rebuild

Extract `twelve-clothing-source.zip` into a folder named `source` next to these files, then:

```bash
cd source
npm ci
npm run dev          # local preview at http://localhost:5173
npm run build:pages  # rebuilds and replaces the site files in this folder
```
