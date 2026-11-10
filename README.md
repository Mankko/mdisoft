# MDI Soft — Developer Website

Official bilingual developer website for **MDI Soft**, published at https://mdisoft.pages.dev/.

## Products

- **Jamtronome:** Android metronome for individual practice and nearby synchronized rehearsals. Released on Google Play. [Google Play](https://play.google.com/store/apps/details?id=com.mankko.jamtronome).
- **ScoreBinder:** Android offline PDF/image sheet music viewer, album library, flexible page layouts and Bluetooth HID page turning. **Preparing for Google Play release**.
- **Stem Lab:** Windows stem separation, analysis and music practice tools. [Stem Lab Free releases](https://github.com/Mankko/stem-lab-releases).

## Deployment

The website is deployed through the existing **Cloudflare Pages** project `mdisoft` at https://mdisoft.pages.dev/, connected to the `main` branch of `Mankko/mdisoft`. The website is static and has no application compilation step.

Source files:
- `index.html`: company homepage and product summaries.
- `app-ads.txt`: AdMob authorized seller declaration (do not modify without verifying the publisher account).
- `.nojekyll`: compatibility with GitHub Pages.
- `README.md`: site documentation.

The prior instructions describing GitHub Pages as the primary deployment site are historical and have been superseded by Cloudflare Pages.

## Google AdMob app-ads.txt

The public seller declaration is served at https://mdisoft.pages.dev/app-ads.txt. Verify that its content continues to match AdMob when advertising settings change.

## Safety and release operations

- Do not commit passwords, signing keys, private data, or AdMob account secrets to this repository.
- **Android APK/AAB builds and tests are local-only** in their respective Windows development folders; no GitHub Actions Android builds may be introduced for ScoreBinder.
- Updating this static homepage through Git does not constitute building, signing, or publishing an Android app.
- ScoreBinder's Play link will be added after its public store listing is actually available.
