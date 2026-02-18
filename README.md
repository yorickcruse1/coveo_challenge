# Coveo Challenge

Simple static search page built with [Coveo Atomic](https://docs.coveo.com/en/atomic/latest/).

## Run locally

Because this project is static, you can open `index.html` directly in your browser.

For best results, run a local server from the project root:

```bash
python3 -m http.server 8000
```

Then open: `http://localhost:8000`

## Deploy on GitHub Pages (with GitHub Secrets)

This project deploys with a GitHub Actions workflow and injects values at deploy time.

1. Push this repository to GitHub.
2. In your repo, go to **Settings → Secrets and variables → Actions**.
3. Add these repository secrets:
	- `COVEO_ACCESS_TOKEN`
	- `COVEO_ORGANIZATION_ID`
	- `COVEO_PIPELINE`
4. Go to **Settings → Pages**.
5. Set **Source** to **GitHub Actions**.
6. Push to `main` (or run the workflow manually in **Actions**).

Your site URL will look like:

`https://<your-username>.github.io/coveo_challenge/`

## Notes

- Static assets should use relative paths (e.g. `static/charlie-meme.jpg`) so they work on GitHub Pages.
- GitHub Pages can take 1–3 minutes to publish updates after each push.
- Secrets keep credentials out of the repository history, but values injected into client-side HTML are still visible in the browser at runtime.
