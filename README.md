# Dopa-Loop Prototype

This repository contains a static prototype for Dopa-Loop — an archive-first, circular-fashion loyalty concept. The main artifact is `dopa-loop-share.html` which is a single-file mockup of the app UI.

Preview locally:

```bash
python3 -m http.server 8000
# then open http://localhost:8000/dopa-loop-share.html
```

Publishing to GitHub Pages

- This repo includes a GitHub Actions workflow that copies `dopa-loop-share.html` to `docs/index.html` and deploys it to GitHub Pages on pushes to `main`.
- After pushing, enable GitHub Pages (if needed) or wait for the action to complete.

How to publish (one-time):

1. Create a GitHub repository and add it as the `origin` remote.
2. Push the `main` branch.
3. The workflow will run and deploy to Pages.

If you want, I can try to create the remote automatically (requires `gh` CLI authenticated). Otherwise, paste the git commands I provide.
