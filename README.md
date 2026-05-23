# tablein-web

Marketing landing for [jointablein.com](https://jointablein.com).

Single-file static site (`index.html`) deployed via GitHub Pages with a
custom `CNAME` mapping the repo to `jointablein.com`.

## Bits

- Bilingual TR / EN with a soft locale toggle (browser default → user
  override persisted in localStorage).
- Waitlist form POSTs to Supabase's `public.waitlist` table via the
  anon key + an INSERT-only RLS policy.
- Legal links point at the existing `bilaltuylu.github.io/tablein-legal`
  repo (privacy, terms, CSAE, account deletion).

## Local preview

Open `index.html` directly in a browser; there's no build step.

## Deploy

`git push` to `main` and GitHub Pages picks it up. The `CNAME` file
ensures the custom domain stays bound after each rebuild.
