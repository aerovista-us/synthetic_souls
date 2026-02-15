# Push Synthetic Souls to GitHub

Repo: **https://github.com/aerovista-us/synthetic_souls**

## If Git says "dubious ownership" (network/UNC path)

Trust this directory once (run from any folder):

```bash
git config --global --add safe.directory '%(prefix)///100.115.9.61/NXDrive/EchoVerse/Music/player/app/pages/synthetic-souls'
```

Then retry `git add` / `git commit`.

---

## First-time push (from synthetic-souls folder)

```bash
cd "\\100.115.9.61\NXDrive\EchoVerse\Music\player\app\pages\synthetic-souls"

# One-time setup
git init
git remote add origin https://github.com/aerovista-us/synthetic_souls.git
git add .
git commit -m "Initial commit: Synthetic Souls page, visualizers, player"

# Use main branch (Git may have created master)
git branch -M main

# Push via HTTPS (prompts for username + Personal Access Token)
git push -u origin main
```

---

## If you get "Permission denied (publickey)" (SSH)

You added `origin` as SSH (`git@github.com:...`) but this machine has no SSH key for GitHub. Use HTTPS instead:

```bash
git remote set-url origin https://github.com/aerovista-us/synthetic_souls.git
git push -u origin main
```

When prompted: **Username** = your GitHub username, **Password** = a [Personal Access Token](https://github.com/settings/tokens) (not your account password).

---

## If you get "src refspec main does not match any"

Your first commit created branch `master`. Rename it to `main` then push:

```bash
git branch -M main
git push -u origin main
```

---

## If the repo already has a README and Git refuses to push

```bash
git pull origin main --allow-unrelated-histories
# fix any conflicts if needed, then:
git push -u origin main
```
