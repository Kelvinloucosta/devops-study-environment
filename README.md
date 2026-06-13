# DevOps on macOS M5 — Isolated Study Environment

A static site guide for setting up a fully isolated DevOps study environment on macOS M5 (Apple Silicon), covering Docker, Kubernetes, Linux VMs, CI/CD, and clean removal.

## How to publish on GitHub Pages

### 1. Create a new GitHub repository

Go to [github.com/new](https://github.com/new) and create a public repo.
Name suggestion: `devops-mac-m5` or `devops-study-guide`.

### 2. Push these files

```bash
cd devops-mac-m5
git init
git add .
git commit -m "initial: devops study guide for macOS M5"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repo on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Source**, select **Deploy from a branch**
4. Choose branch: `main`, folder: `/ (root)`
5. Click **Save**

Your site will be live at:
```
https://YOUR_USERNAME.github.io/YOUR_REPO/
```

It usually takes 1–2 minutes for the first deploy.

## What's included

- `index.html` — the full site (single file, no dependencies, no build step)

## Tools covered

| Tool | Purpose |
|------|---------|
| Homebrew | Package manager — install everything through it |
| OrbStack | Docker + Kubernetes for Apple Silicon |
| UTM | Free ARM Linux virtual machines |
| mise | Per-project tool version management |
| direnv | Per-folder environment variables |
| act | Run GitHub Actions workflows locally |
