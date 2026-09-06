# chirp-site

The public face of [Parlour Games](https://github.com/garethbirduk/mobile-games):
a landing page and the privacy policy its Google Play listing points at.

This is a separate repo for one reason — the app's repo is private, and GitHub
Pages on a free plan only serves public ones. The policy is meant to be public
anyway, so nothing is lost.

- **Serves at** `https://garethbirduk.github.io/chirp-site/` via the `pages`
  workflow, on every push to main.
- **The intended home is `https://apps.chirp.me.uk/`** — one DNS CNAME
  (`apps` → `garethbirduk.github.io`) and then the custom domain set in this
  repo's Pages settings. Domain second, DNS first: setting the domain makes the
  github.io address redirect to it, so doing it early breaks the site.
- Hand-written static HTML, no build step, relative links throughout so both
  addresses work. The app's own web build is intended to move in beside these
  pages later — see `docs/RELEASE.md` in the app repo, which is also where the
  release process this site is part of is written down.
