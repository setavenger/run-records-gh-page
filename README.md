# RunRecords — public site

Static GitHub Pages site for RunRecords (privacy, support, Impressum). Hosted from the public repo [setavenger/run-records-gh-page](https://github.com/setavenger/run-records-gh-page) because GitHub Pages on private repos requires a paid plan.

| Page | Path | URL |
|------|------|-----|
| Home | `/` | `https://runrecords.app/` |
| Privacy | `/privacy/` | `https://runrecords.app/privacy` |
| Support | `/support/` | `https://runrecords.app/support` |
| Impressum | `/impressum/` | `https://runrecords.app/impressum` |

## Deploy on GitHub Pages

Deployment is automated by [`.github/workflows/pages.yml`](.github/workflows/pages.yml).

### One-time setup

1. Push this repository to GitHub (`setavenger/run-records-gh-page`).
2. In the repo: **Settings → Pages**.
3. Set **Source** to **GitHub Actions**.
4. Push to **`master`** (or run the workflow manually).

### Custom domain

Domain: **`runrecords.app`** (`CNAME` in repo root).

1. Add `runrecords.app` under **Settings → Pages → Custom domain**.
2. Point DNS at your registrar to GitHub Pages (A/AAAA for apex, or CNAME for `www`).
3. Enable **Enforce HTTPS** after DNS propagates.

App Store Connect:

- **Privacy Policy URL:** `https://runrecords.app/privacy`
- **Support URL:** `https://runrecords.app/support`

## Local preview

```bash
python3 -m http.server 8080
```

Open `http://localhost:8080/` and check `/privacy/`, `/support/`, and `/impressum/`.

## Related repo

The iOS app lives in the private [workout-app](https://github.com/setavenger/workout-app) repository.
