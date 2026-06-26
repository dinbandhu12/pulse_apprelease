# Pulse — Download Page

A one-page site for the team to download the Pulse Android app (`.apk`).

## Files
- `index.html` — the landing page (glass UI, Android download + Windows "coming soon").
- `icon.png` — the app icon.

## Set the download link (one line)
Open `index.html` and edit the `--apk-url` line near the top of the `<style>`:

```
--apk-url: "https://github.com/YOUR_USERNAME/YOUR_REPO/releases/latest/download/pulse.apk";
```

Use the **`releases/latest/download/<file>`** form — it always points to the newest
release and downloads the APK directly (no GitHub page). Make sure the asset you upload
to the GitHub Release is named **`pulse.apk`** (or change the filename in the URL to match).

## Publish (free options)
- **GitHub Pages:** push this folder to a repo → Settings → Pages → deploy. 
- Or drag the folder into **Netlify** / **Vercel** / **Cloudflare Pages**.

## Update for a new build
1. Build a new APK and upload it to a new GitHub **Release** as `pulse.apk`.
2. Done — the page's `latest` link auto-points to it (no edits needed).
