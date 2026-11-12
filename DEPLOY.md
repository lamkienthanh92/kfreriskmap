# Publishing: GitHub, Netlify and a Zenodo DOI

## 1. GitHub
1. Create a new public repository, for example `kfre-risk-map` (no README, licence or .gitignore, because they are included here).
2. Upload the contents of this folder (not the folder itself), either by dragging the files into "Add file → Upload files", or from a terminal:
   ```bash
   cd kfre-risk-map
   git init
   git add .
   git commit -m "KFRE Risk Map v2.2.0"
   git branch -M main
   git remote add origin https://github.com/YOUR-USER/kfre-risk-map.git
   git push -u origin main
   ```
3. Edit `CITATION.cff` and replace `YOUR-USER` in `repository-code` with your account name.

## 2. Netlify
1. Sign in at https://app.netlify.com with your GitHub account.
2. "Add new site → Import an existing project → GitHub", choose the repository.
3. Leave the build command empty; the publish directory is `.` (already set in `netlify.toml`). Deploy.
4. Optionally rename the site under "Site configuration → Change site name", then put the address in `README.md`.

Alternative without GitHub: drag this whole folder onto https://app.netlify.com/drop.

## 3. Zenodo DOI

Two routes are possible. Route A (manual upload) is described step by step in `ZENODO_UPLOAD.md`. Route B (automatic, through GitHub) follows.

### Route B: GitHub integration
1. Sign in at https://zenodo.org with your GitHub account (use https://sandbox.zenodo.org first if you want a test run; sandbox DOIs are not real).
2. Open the GitHub page in your Zenodo account settings and switch the repository **on**.
3. On GitHub, create a release: "Releases → Draft a new release", tag `v2.2.0`, title `KFRE Risk Map v2.2.0`, publish.
4. Zenodo archives the release within a few minutes and mints a DOI, using the metadata in `.zenodo.json`. Check the record and correct anything you need on Zenodo.
5. Copy the DOI and replace `10.5281/zenodo.XXXXXXX` in `README.md`, `CITATION.cff` and the "Cite this tool" card in `index.html`. Commit the change. Zenodo also gives a "concept DOI" that always points to the latest version; use it if you want one DOI for all versions.

Before step 3, confirm the author list, ORCID iDs and affiliations in `.zenodo.json` and `CITATION.cff`, and confirm that publishing `assets/js/cohort.js` is covered by your ethics approval. A Zenodo record cannot be deleted after publication.
