# Parts Finder

Enter a model number (and optionally a part name) and open parts search results on several sites. Static page: no backend, no storage.

## Publish free on GitHub Pages

1. Create a GitHub account at https://github.com if you don't have one.
2. Click **New repository**. Name it `parts-finder`, set it to **Public**, and click **Create repository**. Don't add a README (this zip has one).
3. Unzip this folder, then in a terminal run inside it:

       git init
       git add .
       git commit -m "Initial commit"
       git branch -M main
       git remote add origin https://github.com/YOUR-USERNAME/parts-finder.git
       git push -u origin main

   (No terminal? On the empty repo page click **uploading an existing file**, drag in `index.html`, `README.md` and `.nojekyll`, then **Commit changes**.)
4. In the repo, go to **Settings → Pages**.
5. Under **Build and deployment**, set **Source** to **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
6. Wait 1-2 minutes. Your site will be live at:

       https://YOUR-USERNAME.github.io/parts-finder/

## Updating the site
Edit `index.html`, then:

    git add . && git commit -m "Update" && git push

The site redeploys automatically.

## Adding or changing search sites
Edit the `SITES` list near the bottom of `index.html`. Each entry is a name and a search URL, with `{q}` where the model number goes.

## Other free hosts
Netlify Drop (app.netlify.com/drop), Cloudflare Pages and Vercel also serve this folder as-is, with no build step.
