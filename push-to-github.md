# Push Synthetic Souls to GitHub

Repo: **https://github.com/aerovista-us/synthetic_souls**

Run these commands from the **synthetic-souls** folder (use a local copy or mapped drive if the project lives on a network path; git push often fails from UNC paths).

```bash
cd /path/to/synthetic-souls

# One-time setup
git init
git branch -M main
git remote add origin https://github.com/aerovista-us/synthetic_souls.git

# Stage and commit
git add .
git commit -m "Initial commit: Synthetic Souls page, visualizers, player"

# Push (requires push access to the repo)
git push -u origin main
```

If `origin` already exists and points elsewhere, fix it:

```bash
git remote remove origin
git remote add origin https://github.com/aerovista-us/synthetic_souls.git
```

If the repo has a README or license and Git says "refusing to merge unrelated histories":

```bash
git pull origin main --allow-unrelated-histories
# resolve any conflicts, then:
git push -u origin main
```

For HTTPS, Git will prompt for your GitHub username and a **Personal Access Token** (not your password). Create one at: GitHub → Settings → Developer settings → Personal access tokens.
