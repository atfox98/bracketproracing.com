# bracketproracing.com

The public website for Bracket Pro and the Timeslip Scanner app: what Bracket Pro does, the
scanner's how-to, and the support page and privacy policy that the App Store listing links to.

Plain HTML and one stylesheet, served as is by GitHub Pages (no build step). It's a submodule
of the Bracket Pro repo at `site/`.

- `software/` is adapted from the User's Manual's chapters on weather, Run Entry, Run Selection,
  Predict and Pager; `scanner/` from its "Timeslip scanner" chapter, and `support/` from that
  chapter's "When the scanner doesn't connect". Update them when the manual changes.
- The screenshots in `images/` are copies of the manual's. After `pnpm run docs:screenshots` in
  Bracket Pro, refresh them from the Bracket Pro repo's root:
  `cp docs/manual/images/{run-entry,weather,weather-graphs,run-selection,predict,formulas,pager,scanner-card,scanner-check,scanner-photo,scanner-run-entry}.png site/images/`
- **Not** `scanner-pairing.png` or `scanner-flow.png`: they show a real pairing QR code, and the
  pairing data is confidential. Here those codes are covered with one for a YouTube link.
  Cover the code again before replacing either.
- `privacy/` is the Timeslip Scanner's privacy policy (the app links to `/privacy`). Change its
  date when it changes, and keep it in step with the app's privacy manifest and App Store
  privacy answers.
- Nothing confidential goes here: this repo is public.

Preview: `python3 -m http.server 8000` in this folder, then open http://localhost:8000.
