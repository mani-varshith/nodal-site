# Nodal Website

Static website copy for Nodal with additional pages:
- Privacy Policy
- Support
- Terms and Conditions
- Data Safety

## Run locally

Open `index.html` directly in browser, or run a simple server:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Deploy on GitHub Pages

This folder is already a git repo on branch `main` with an initial commit.

### Option A: GitHub CLI (fastest)

1. Log in once (opens browser):

   ```bash
   gh auth login
   ```

2. From this directory, create the repo on your account and push:

   ```bash
   cd /Users/venkatavarshithsivapuram/Documents/dailyos-site
   gh repo create nodal-site --public --source=. --remote=origin --push
   ```

   Use another name if `nodal-site` is taken, e.g. `gh repo create nodal-website --public --source=. --remote=origin --push`.

3. On GitHub: **Settings → Pages → Build and deployment → Deploy from a branch** → branch **main**, folder **/ (root)** → Save. Your site will be at `https://<username>.github.io/<repo>/`.

### Option B: GitHub website

1. Create a new empty repository (no README) on GitHub.
2. Run:

   ```bash
   cd /Users/venkatavarshithsivapuram/Documents/dailyos-site
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```

3. Enable **Pages** as in step 3 of Option A.
