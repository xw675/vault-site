# 🚀 Publish Your Vault Website

Your site is built with [Quartz 4](https://quartz.jzhao.xyz). It includes your 6 unit MOCs + all concept notes, with working wikilinks, LaTeX, Mermaid diagrams, callouts, search (Ctrl/Cmd+K), graph view, backlinks, and dark mode.

## ⚠️ First: unzip OUTSIDE your Obsidian vault
Extract `monash-cs-notes.zip` to somewhere like `~/Documents/monash-cs-notes` — NOT inside your Obsidian folder, or Obsidian will index the duplicated notes and break your wikilinks.

## 1. One-time setup (≈10 minutes)

**a. Install Node.js** (if not installed): download the LTS from https://nodejs.org

**b. Create the GitHub repo:**
1. Go to https://github.com/new
2. Name it `monash-cs-notes` (public), don't add any files, click **Create repository**

**c. Set your site URL:** open `quartz.config.ts` and replace `GITHUB-USERNAME` on the `baseUrl` line with your actual GitHub username.

**d. Push the code** — in Terminal:
```bash
cd ~/Documents/monash-cs-notes
git init
git add -A
git commit -m "initial site"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/monash-cs-notes.git
git push -u origin main
```

**e. Enable GitHub Pages:** on the repo page → **Settings → Pages** → under *Build and deployment*, set **Source: GitHub Actions**.

Wait ~2 minutes for the Action to finish (green tick under the **Actions** tab), then your site is live at:

**https://YOUR-USERNAME.github.io/monash-cs-notes/**

## 2. Updating the site when your notes change

```bash
cd ~/Documents/monash-cs-notes
./sync-content.sh          # copies latest notes from your vault
git add -A && git commit -m "update notes" && git push
```
GitHub rebuilds and republishes automatically.

## 3. Preview locally (optional)

```bash
cd ~/Documents/monash-cs-notes
npm ci          # first time only
npx quartz build --serve
```
Then open http://localhost:8080

## Notes
- Only `10_Units`, `20_Concepts`, and `90_Attachments` are published. Projects/Skills/Inbox stay private.
- The site is **public** — anyone with the URL can read it.
- To change the site name/colours, edit `quartz.config.ts`.
