# dancinggorillagames.github.io

The Dancing Gorilla Games website: plain HTML and CSS, published with GitHub Pages. No build step, no third-party scripts, fonts or trackers.

| Path | What it is |
|---|---|
| `/` (`index.html`) | Studio home page |
| `/tidybelt/` | Tidy Belt page |
| `/tidybelt/privacy/` | Tidy Belt privacy policy. Its URL goes into the game (`GameConfig.privacyPolicyUrl`) and the Play Console listing |
| `/app-ads.txt` | Authorised ad sellers (AdMob). Must stay at the domain root |
| `404.html` | Shown for missing pages |
| `assets/` | Stylesheet, icons, Fredoka font (SIL OFL 1.1, licence in `assets/fonts/OFL.txt`) |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

## Publish

1. Create a free GitHub organization for the studio (github.com → your avatar → **Your organizations → New organization → Free**), for example `DancingGorillaGames`.
2. In it, create a **public** repository named exactly `<organization name, lowercase>.github.io`, for example `dancinggorillagames.github.io`. Leave it empty (no README).
3. Push this folder to it (`main` branch).
4. Repository **Settings → Pages → Build and deployment**: Source **Deploy from a branch**, branch **main**, folder **/ (root)**, **Save**. The site appears at `https://dancinggorillagames.github.io` within a few minutes.
5. Check `https://dancinggorillagames.github.io/app-ads.txt` and `https://dancinggorillagames.github.io/tidybelt/privacy/` open.

## Before launch

- Replace the `[CONTACT EMAIL]` and `[POSTAL ADDRESS OR COUNTRY]` placeholders (highlighted on the pages).
- Put the Play Store link on the Tidy Belt page and the home page once the listing is public.
- In Play Console, set the **website** to the site's address, so ad networks find `app-ads.txt`.

## Custom domain (optional, later)

Buy the domain, add a `CNAME` file containing just the domain (for example `dancinggorillagames.com`), set the DNS records GitHub lists under **Settings → Pages → Custom domain**, and tick **Enforce HTTPS**. Then update the privacy policy URL in the game and in Play Console.

## Keeping the privacy policy in step

The game repository keeps the draft in `Docs/privacy-policy.html`. This site's `tidybelt/privacy/index.html` carries the same text inside the site layout. Change both together, and update the "Last updated" date.
