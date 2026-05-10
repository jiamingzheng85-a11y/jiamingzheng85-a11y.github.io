# Jiaming Zheng Personal Homepage

This directory contains a static personal homepage that can be deployed directly with `GitHub Pages`.

## Files

- `index.html`: main homepage file
- `styles.css`: page styling
- `.nojekyll`: ensures GitHub Pages serves the site as a plain static website

## Local Preview

The simplest way:

1. Open this directory
2. Double-click `index.html`
3. Your browser will open the page directly

If you prefer to preview it through a local server, open a terminal in this directory and run:

```powershell
python -m http.server 8000
```

Then visit `http://localhost:8000`

## Uploading to GitHub

The easiest option is to upload the files through the GitHub web interface:

1. Sign in to GitHub
2. Click the `+` icon in the upper-right corner
3. Select `New repository`
4. Recommended repository names:
   - `zhengjiaming-homepage`
   - or, if you want the site at the root personal URL, `your-github-username.github.io`
5. Set the repository to `Public`
6. After creating the repository, open it
7. Click `Add file`
8. Select `Upload files`
9. Drag the following files into the upload area:
   - `index.html`
   - `styles.css`
   - `.nojekyll`
10. After the upload completes, click `Commit changes`

## Enabling GitHub Pages

According to the current GitHub Pages workflow:

1. Open the repository
2. Click `Settings`
3. In the left sidebar, select `Pages`
4. Under `Build and deployment`:
   - set `Source` to `Deploy from a branch`
   - set `Branch` to `main`
   - set `Folder` to `/(root)`
5. Click `Save`
6. Wait from a few seconds to a few minutes for deployment

## Deployment URL

If your repository uses a standard name such as:

- `zhengjiaming-homepage`

the URL is typically:

- `https://your-username.github.io/zhengjiaming-homepage/`

If your repository is named:

- `your-username.github.io`

then the URL is typically:

- `https://your-username.github.io/`

## Future Updates

To update the site later, simply upload and replace the same files, then commit the changes. GitHub Pages will redeploy the site automatically.

## Notes

If you later want to add a profile photo, project images, or a downloadable CV, it is best to create an `assets/` folder for images and attachments.
