# 🌎✈️ McBoris World Tour

A single-page trip planner: route calendar, flights, transport, lodging stays, and
day-by-day plans. No build step, no dependencies to install — it's one static
`index.html` file.

## How to put it online with GitHub Pages

1. **Create a repository**
   - Go to [github.com/new](https://github.com/new)
   - Name it whatever you like (e.g. `mcboris-world-tour`)
   - Set it to **Public** (required for free GitHub Pages)
   - Click **Create repository**

2. **Upload the file**
   - On the new repo's page, click **"Add file" → "Upload files"**
   - Drag in `index.html` from this folder
   - Click **Commit changes**

3. **Turn on GitHub Pages**
   - Go to **Settings → Pages** (left sidebar)
   - Under **Build and deployment → Source**, choose **Deploy from a branch**
   - Branch: `main`, folder: `/ (root)` → **Save**
   - Wait about a minute, then reload the Pages settings page — you'll see a link like:
     `https://your-username.github.io/mcboris-world-tour/`

4. Open that link — the app is live.

## Important: how your data is saved

This app was originally built inside Claude, which provides an automatic
per-account storage API. A normal website doesn't have that, so this version
uses the browser's own storage (`localStorage`) instead. That means:

- Your trip data is saved **in the browser you're using**, not in an account.
- It won't show up if you open the site on a different browser or device.
- Clearing your browser's site data/cookies will erase it.
- It's private to your own browser — nobody else visiting the link sees your data
  (each visitor gets their own separate local copy).

If you want the data to sync across your devices, you'd need to add a real
backend (e.g. Firebase, Supabase) — that's a bigger step and not included here.

## Updating the app later

Any time you want to change something, edit `index.html` and upload the new
version through **Add file → Upload files** again (or use `git push` if you're
comfortable with Git). GitHub Pages updates automatically within a minute or two
of a new commit.
