# Fox App Support

Support, privacy, and license pages for the iOS app Fox. The copy is German first, with an English section for App Store review.

The site lives in [`docs/`](docs/).

## URLs for App Store Connect

- Support URL: https://trakowskymarcel-pixel.github.io/fox-app-support/
- Privacy Policy URL: https://trakowskymarcel-pixel.github.io/fox-app-support/privacy.html
- License notes: https://trakowskymarcel-pixel.github.io/fox-app-support/terms.html

Use Apple’s [Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/) in App Store Connect. `terms.html` only links that agreement and adds short notes about the app. It is not a custom EULA.

## Turn GitHub Pages on once

A repository admin has to enable Pages. The GitHub Actions token cannot create the site. After this setting is saved, pushes to `main` keep the site up to date.

Open [Settings → Pages](https://github.com/trakowskymarcel-pixel/fox-app-support/settings/pages) and pick one:

1. **Deploy from a branch** (simplest): branch `main`, folder `/docs`, then Save.
2. **GitHub Actions**: Source **GitHub Actions**. The workflow [`.github/workflows/pages.yml`](.github/workflows/pages.yml) publishes `docs/`.

Do not use raw.githack.com or another raw-file host. Apple rejects those as the Support URL.
