# Four-Plate Week

A 4-day, under-60-minute strength, cardio and mobility program, built as an installable web app (PWA). It works offline once it has been opened.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole app: program, home routines, exercise library, review |
| `manifest.webmanifest` | Lets phones install it with a name and icon |
| `sw.js` | Offline cache |
| `icons/` | Home-screen icons |

## Publish on GitHub Pages (one time)

1. Sign in at github.com (create a free account if you don't have one).
2. Click **+** → **New repository**. Name it `four-plate-week`, set it to **Public**, and click **Create repository**.
3. On the new repo page, click **uploading an existing file**. Drag in `index.html`, `manifest.webmanifest`, `sw.js` and the `icons` folder, then click **Commit changes**.
4. Go to **Settings** → **Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main** and folder to **/ (root)**, then click **Save**.
5. After about a minute your app is live at `https://YOUR-USERNAME.github.io/four-plate-week/`.

## Install on your iPhone

Open the URL in **Safari** → tap **Share** → **Add to Home Screen** → **Add**. It opens full-screen from its own icon, keeps the screen awake on the Train tab, and works without signal at the gym.

## Updating the app later

1. Edit `index.html`.
2. In `sw.js`, bump `VERSION` (for example `fpw-v1` → `fpw-v2`) so phones fetch the new copy.
3. Upload both files to the repo again (**Add file** → **Upload files**). Pages redeploys in about a minute.
4. On the phone, close and reopen the app (twice if the change doesn't show the first time).

Your checkmarks and last-viewed day are stored on the phone only.
