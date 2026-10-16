# My Offer Is Coming: put it on your phone

This folder is a small web app. Once it's on GitHub Pages you can add it to your home screen, and it opens full-screen with its own icon like a normal app. It also works offline.

## 1. Put it on GitHub Pages (about 5 minutes, free)

1. Sign in at https://github.com and click **New repository**.
2. Name it `my-offer` and choose **Public** (free GitHub Pages needs a public repo). Click **Create repository**.
3. Click **uploading an existing file**. Drag in everything from this folder: `index.html`, `manifest.webmanifest`, `sw.js` and the whole `icons` folder. Click **Commit changes**.
4. Go to **Settings → Pages**. Under "Build and deployment", set Source to **Deploy from a branch**, Branch to **main** and folder to **/(root)**. Click **Save**.
5. Wait 1–2 minutes and refresh. Your link appears at the top: `https://<your-username>.github.io/my-offer/`

Or from a terminal:

```bash
cd offer-app
git init && git add . && git commit -m "My Offer app"
git branch -M main
git remote add origin https://github.com/<your-username>/my-offer.git
git push -u origin main
```

Then turn on Pages as in step 4.

## 2. Install it on your phone

**Android (Chrome):** open your link, tap the **⋮** menu, then **Add to Home screen** (or **Install app**), then **Install**.

**iPhone (Safari):** open your link, tap **Share**, then **Add to Home Screen**, then **Add**.

The "My Offer" icon is now on your home screen.

## 3. Good to know

- **Your data stays on your phone.** Ticks, your own tasks, "Learned today" notes and your affirmation count are saved in the app on that phone. They don't sync with the Claude page or other devices.
- **Back up now and then.** Scroll to the bottom and tap **Download backup**. On a new phone, install the app and tap **Restore from backup**.
- **Bedtime alarm:** a web app can't ring an alarm at a set time, so set a daily 10:30 PM alarm in your Clock app labelled "Read all manifestations".
- **Updating the app:** upload a new `index.html` to the repo. To make sure phones pick it up, change `my-offer-v1` to `my-offer-v2` in `sw.js` and upload that file too.
