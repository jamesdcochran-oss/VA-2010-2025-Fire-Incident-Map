VA Fires Map — GitHub Pages Ready
=================================

This ZIP contains a single-file interactive map that visualizes Virginia fire incidents (Oct-Dec 2020-2025).
The HTML file embeds the GeoJSON; no external files are required.

Files in this archive:
- index.html        (interactive map — drop this in the repo root)
- README.md         (this file)
- LICENSE           (MIT license)

Quick publish steps (web UI):
1. Create a new **public** repository on GitHub (e.g., `VA-Fires-Map`).
2. On your computer unzip this archive. Rename `VA_Fires_Recreated_Map.html` to `index.html` **if not already named**.
3. On the repo page click **Add file → Upload files** and drag `index.html` (and README.md, LICENSE) into the root of the repo. Commit.
4. Go to **Settings → Pages** (or Settings → Code and automation → Pages). Under "Source" choose branch **main** (or **master**) and folder **/ (root)**, then Save.
5. After a minute GitHub will publish the site at: https://<your-github-username>.github.io/<repo-name>/

Quick publish steps (CLI):
```bash
# in the folder with index.html
git init
git add index.html README.md LICENSE
git commit -m "Publish VA Fires map"
git branch -M main
git remote add origin https://github.com/<USERNAME>/<REPO>.git
git push -u origin main
```

Notes:
- Make the repository **public** so anyone can view the map.
- Because the GeoJSON is embedded, there are no fetch/CORS issues on GitHub Pages.
- If you want the site at the root of your username (https://<username>.github.io/), name the repo `<username>.github.io`.
- I did not change the map. The map file in this ZIP is the same single-file HTML you approved.