# Block Jai — official website (static GitHub Pages)

This is a **complete drop-in replacement** for the public website at:
https://samueldmchung.github.io/block-jai/

## V1.2 — What's new (2026-10-16)

- Homepage now advertises **free shape rotation in all three modes** as Block Jai's headline feature.
- Removed claims that rotation is an unlockable tool or an Impossible-only ability.
- Updated perks card to show real Dice, Hammer and God’s Eye art from the V1.443 game project.
- Replaced confusing “Big / Boss battles” stat with **GLOBAL / Leaderboards**.
- Added a worldwide **Game Center leaderboards** promotional section for Classic, Impossible and Challenges, including friends and global rankings. The visual is illustrative, not live scores.
- Updated metadata, mode descriptions and navigation to match.
- Preserved Support, Privacy Policy wording, live app links, and **exact app-ads.txt publisher line**. No iOS source changes.

## Publish using GitHub's website

1. Open https://github.com/SamuelDMChung/block-jai
2. Choose **Add file → Upload files** (or edit your existing files on the `main` branch).
3. **Extract this ZIP first.** Upload **the contents inside** `BlockJai_Website_V1_2_GLOBAL_RANKINGS_FULL` (not the ZIP itself): `index.html`, `privacy.html`, `support.html`, `styles.css`, `app-ads.txt`, and the whole `assets/` folder, preserving the folder structure.
4. Commit the changes to `main` and let GitHub Pages publish them. If you cannot drag a folder, upload its files into `assets/` via the GitHub browser or use GitHub Desktop.
5. Visit https://samueldmchung.github.io/block-jai/ and also check `/support.html` and `/privacy.html`.

**Important:** Keep the existing site at the same GitHub Pages URL. There is no need to change the Apple App Store Marketing URL, Support URL, or Privacy Policy URL.

## Important: Google AdMob app-ads.txt verification

The `app-ads.txt` file is included in this release and contains:

```text
google.com, pub-9867609214209513, DIRECT, f08c47fec0942fa0
```

**This `block-jai` repository is a project site**, hosted under `/block-jai/`. Uploading its `app-ads.txt` file here will create `https://samueldmchung.github.io/block-jai/app-ads.txt`, **but AdMob looks at the hostname root**: `https://samueldmchung.github.io/app-ads.txt`. Publishing only to this project repository will NOT satisfy AdMob.

To publish the required root file using GitHub Pages, create a second PUBLIC GitHub repository called **`samueldmchung.github.io`** (or use it if it already exists), and upload the exact same `app-ads.txt` into its repository root. In Settings → Pages, set **Deploy from a branch**, **main**, **/(root)**. Verify that `https://samueldmchung.github.io/app-ads.txt` shows the snippet in a browser. A small ready-to-upload separate root-site ZIP is provided as `BlockJai_AdMob_GitHubRoot_FULL.zip`.

Additionally, AdMob requires the Apple App Store listing to expose **Developer Website**, sourced from App Store Connect **Marketing URL**, for example `https://samueldmchung.github.io/block-jai/`. If the link is absent from the public App Store listing, add it with the next editable app version. Allow time for Apple/AdMob updates before retrying verification. **The support URL by itself is not a substitute.**

## Contents

- `app-ads.txt` — AdMob publisher snippet (also must be published on GitHub Pages hostname root)
- `index.html` — responsive marketing landing page
- `support.html` — same existing support email and support instructions, restyled
- `privacy.html` — same existing privacy policy wording and last-updated date, restyled; no legal changes claimed
- `styles.css` — all site styles, including mobile layouts and reduced-motion accessibility
- `assets/` — app icon, banners, monster art, perk icons, Game Center trophy, locally hosted font, favicon, and share image extracted/derived from the supplied V1.443 Godot game project

## Links

- App Store: https://apps.apple.com/us/app/block-jai/id6814092749
- Support email: blockjaisupport@gmail.com

## Notes

- No build system, npm, backend, analytics, cookies, or external dependencies are required.
- The stylized 9×9 board in the homepage hero is **a decorative illustration, not a screenshot or a playable game**. It uses CSS/HTML and imagery from the real app; real screenshots can be added later.
- Uses current public product information as of October 16, 2026. This website project makes no changes to the V1.443 iOS game code, saved data, native frameworks, or App Store submission.
