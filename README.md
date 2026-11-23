# levimcneely.com

Personal landing page for Levi McNeely. Static, no build step.

This repo is the GitHub Pages **user site** (`levimcneely-cmyk.github.io`). Because it owns the custom domain `levimcneely.com`, every project repo under `levimcneely-cmyk` that has no CNAME of its own is automatically served under it:

| Repo | URL |
|---|---|
| scoreboard | levimcneely.com/scoreboard |
| highpoints | levimcneely.com/highpoints |
| gatecheck | levimcneely.com/gatecheck (incl. /gatecheck/nrtclogistics) |

Repos with their own CNAME (herdcoindy, bluff-road-bike-co, rbc, pgesdadsclub) are unaffected.

Note: *every* CNAME-less repo moves, so tsp27, bigacalendar, familymlbtracker and jcremcoru will also answer at levimcneely.com/<repo>. Old github.io links redirect automatically. They just aren't linked from the landing page.

## DNS (Squarespace Domains)

Apex `levimcneely.com`, A records:
185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153

`www`, CNAME: `levimcneely-cmyk.github.io`

Then in repo Settings → Pages: source = `main` / root, custom domain = `levimcneely.com`, and tick **Enforce HTTPS** once the certificate is issued.

## Editing

All content is in `index.html`. The career list, the side projects and the race log are plain HTML lists. Add a year to the race log by copying an `<li>` (use `class="dnf"` for a DNF and move `class="now"` to the latest year).
