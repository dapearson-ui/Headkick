# HEADKICK ⚽

Soccer scores dashboard + arcade headball game.

## Local Development

```bash
npm install
npm run dev
```

Then open http://localhost:5173

## Deploy to GitHub + Cloudflare Pages

### Step 1 — Push to GitHub

```bash
# One-time setup (run from inside this folder)
git init
git add .
git commit -m "Initial commit — HEADKICK"

# Create a new repo on github.com called "headkick", then:
git remote add origin https://github.com/YOUR_USERNAME/headkick.git
git branch -M main
git push -u origin main
```

### Step 2 — Connect to Cloudflare Pages

1. Go to https://dash.cloudflare.com
2. Click **Workers & Pages** → **Create application** → **Pages** → **Connect to Git**
3. Authorise GitHub and select the **headkick** repo
4. Set these build settings:
   - **Framework preset:** Vite
   - **Build command:** `npm run build`
   - **Build output directory:** `dist`
5. Click **Save and Deploy**

Cloudflare will build and publish it. Every `git push` to `main` will auto-redeploy.

## Controls

| Key | Action |
|-----|--------|
| ← → / A D | Move |
| ↑ / W | Jump |
| ↑ / W × 2 (in air) | Bicycle kick 🤸 |
| SPACE (hold) | Power shot 💥 |
| R (near ball) | Rainbow flick 🌈 |
