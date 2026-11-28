# AYAMAI website

Four static pages: `index.html` (AYAMAI home), `dreams.html` (DREAMS), `sphota.html` (Sphota) and `vision.html` (the original vision note). No build step. `logo-mark.svg` is the AYAMAI mark (magenta ring, blue point) with a transparent background.

## Deploy on Render

Render deploys static sites from a Git repository, not from an uploaded zip.

1. Create a new GitHub repository (for example `ayamai-site`) and push these files to it.
2. In the Render dashboard choose **New → Static Site** and connect the repository.
3. Settings:
   - Build command: `echo "No build step needed"`
   - Publish directory: `.`
4. Click **Create Static Site**. Render gives you an `onrender.com` address.

Alternatively choose **New → Blueprint** and Render will read `render.yaml` and fill these settings for you.

To use your own domain (for example `ayamai.com`), add it under the site's **Settings → Custom Domains** and follow the DNS instructions Render shows.
