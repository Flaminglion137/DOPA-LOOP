# Dopa-Loop Prototype

This repository contains a static prototype for Dopa-Loop — an archive-first, circular-fashion loyalty concept. The main artifact is `dopa-loop-share.html` which is a single-file mockup of the app UI.

Preview locally:

```bash
python3 -m http.server 8000
# then open http://localhost:8000/dopa-loop-share.html
```

Publishing to GitHub Pages

- This repo includes a GitHub Actions workflow that copies `dopa-loop-share.html` to `docs/index.html` and deploys it to GitHub Pages on pushes to `main`.
- After pushing, the site will be published at:

- https://Flaminglion137.github.io/DOPA-LOOP/

- If you see a 404 when visiting the URL, the usual causes and steps are below.

Troubleshooting a 404

1. Wait a few minutes — Pages can take 1–5 minutes after the Action completes to become available.
2. Check the repository Actions page for the `Deploy to GitHub Pages` run and verify it completed successfully: https://github.com/Flaminglion137/DOPA-LOOP/actions
3. If the Action failed, open the run and review the logs, then push another commit (or re-run the workflow) to trigger deployment again.
4. Confirm `docs/index.html` exists on `main` (the workflow copies `dopa-loop-share.html` there automatically). You can view the file in the repo on GitHub after pushing.
5. If Pages still shows 404 after a successful Action and `docs/index.html` exists, try clearing your browser cache or visit with a query string (e.g. `?nocache=1`).

Force a redeploy (quick):

```bash
cd /Users/tia/dopa-loop
git commit --allow-empty -m "chore: trigger pages redeploy"
git push origin main
```

If you'd like I can watch the Action run and confirm when the site is live — tell me to proceed and I'll monitor the deployment logs.
