# MDI Soft — Developer Website

Official static developer website for **MDI Soft**.

## Products

- **Jamtronome:** nearby synchronized Android metronome for solo and group practice. Google Play production release is being prepared.
- **Stem Lab:** Windows stem separation, analysis and music practice tools. [Stem Lab Free releases](https://github.com/Mankko/stem-lab-releases).

## Publishing through GitHub Pages

1. Open [Settings → Pages](https://github.com/Mankko/mdisoft/settings/pages).
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Choose **main** and **/(root)**, then **Save**.
4. After GitHub Pages finishes publishing, check https://mankko.github.io/mdisoft/.

The URL above is a **temporary project-site address**, not a company-owned domain.

## Google AdMob app-ads.txt

The repository includes `app-ads.txt`, with the publisher ID derived from the Jamtronome release configuration.

**Important:**
- Verify the file's seller line against the exact one shown in AdMob.
- Google's app-ads.txt validation normally discovers the file at the **root of the developer website's domain**.
- A project URL like `https://mankko.github.io/mdisoft/app-ads.txt` alone is not equivalent to `https://mankko.github.io/app-ads.txt`, and should **not** be treated as a completed AdMob verification.
- To establish MDI Soft branding and a suitable root URL, connect a **company-owned custom domain** to this GitHub Pages repository. A domain must be registered separately; this has not been done or verified here.
- After configuring the domain and DNS, verify `https://YOUR_DOMAIN/app-ads.txt` returns HTTP 200 with the exact seller line. Register `https://YOUR_DOMAIN/` as the Google Play developer website and check AdMob status.

## Repository contents

- `index.html` — official site home page (Korean + English)
- `app-ads.txt` — AdMob authorized seller declaration
- `.nojekyll` — disable Jekyll processing for GitHub Pages
- `README.md` — these instructions

No Android application source code, credentials, or private personal data should be committed here.
