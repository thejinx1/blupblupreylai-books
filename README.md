# Grade 9 PDF Archive

This repository publishes the PDF files as direct `.pdf` links on GitHub Pages.

## How it works

- `index.html` lists every PDF in the repository root.
- Each Open button points directly to `./filename.pdf`.
- `.github/workflows/pages.yml` checks out Git LFS files, builds a clean `_site` folder, and deploys it with GitHub Pages.
- `.nojekyll` keeps GitHub Pages from running Jekyll processing.

## GitHub Pages setup

1. Push this repository to GitHub.
2. Open the repository on GitHub.
3. Go to Settings -> Pages.
4. Set Source to GitHub Actions.
5. Run the `Deploy PDF archive to GitHub Pages` workflow, or push to `main`.

After deployment, the site URL will be shown in the workflow summary. Every PDF will be available at:

```text
https://<username>.github.io/<repository>/<filename>.pdf
```

## Size note

The current PDFs are about 912 MB total. GitHub Pages has a 1 GB published-site limit, so adding many more large PDFs may require moving some files to Releases or another file host.
