# Coveo Challenge

Simple static search page built with [Coveo Atomic](https://docs.coveo.com/en/atomic/latest/).

## Run locally

Because this project is static, you can open `index.html` directly in your browser.

For best results, run a local server from the project root:

```bash
python3 -m http.server 8000
```

Then open: `http://localhost:8000`

## Deploy on GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Set **Source** to **Deploy from a branch**.
4. Select branch **main** and folder **/ (root)**.
5. Save and wait for deployment.

Your site URL will look like:

`https://<your-username>.github.io/coveo_challenge/`

## Notes

- Static assets should use relative paths (e.g. `static/charlie-meme.jpg`) so they work on GitHub Pages.
- GitHub Pages can take 1–3 minutes to publish updates after each push.
