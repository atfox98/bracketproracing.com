# bracketproracing.com

The public website for Bracket Pro and the Timeslip Scanner app: the support page and the
privacy policy that the App Store listing links to, and the scanner's how-to.

Plain HTML and one stylesheet, served as is by GitHub Pages (no build step). It's a submodule
of the Bracket Pro repo at `site/`.

- `scanner/` is adapted from the User's Manual's "Timeslip scanner" chapter, and `support/` from
  its "When the scanner doesn't connect" section. Update them when the manual changes.
- The screenshots in `images/scanner-*.png` are copies of the manual's. After
  `pnpm run docs:screenshots` in Bracket Pro, refresh them from the Bracket Pro repo's root:
  `cp docs/manual/images/scanner-*.png site/images/`
- `privacy/` is the Timeslip Scanner's privacy policy (the app links to `/privacy`). Change its
  date when it changes, and keep it in step with the app's privacy manifest and App Store
  privacy answers.
- Nothing confidential goes here: this repo is public.

Preview: `python3 -m http.server 8000` in this folder, then open http://localhost:8000.
