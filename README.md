# VERSEDEX

A free, mobile-first Star Citizen ship and vehicle reference.

**Live:** https://versedex.netlify.app

## What it does

- Full ship and vehicle roster, pulled live from the community wiki API
- Spec sheets: hardpoints, flight performance, cargo, crew, dimensions
- Compare up to 4 ships side by side with a radar chart
- Personal hangar tracker with fleet value and paste-import
- In-game aUEC prices plus the terminals that sell each ship
- Tools: cargo efficiency, ROI, rent-vs-buy break-even, affordability, live trade routes
- Deep filters: seats, medbed tier, cargo grid, hardpoint size, components, flight minimums
- Installable as a PWA, works offline, shareable per-ship links

## Structure

Everything is a single self-contained `index.html` — no build step, no dependencies,
no bundler. Open it in a browser and it runs.

## Data sources

- [star-citizen.wiki API](https://api.star-citizen.wiki) — ships, specs, images
- [UEX](https://uexcorp.space) — in-game prices and trade routes

Both are community-run and can lag behind live game patches.

## Deploying

Netlify is connected to this repo. Any push to `main` deploys automatically.
To change the site, edit `index.html`, commit, and push.

## Known limitations

- Capital ships often have sparse data upstream (flagged in-app)
- Very newly announced ships may not appear until the wiki API catches up
- Non-USD currency conversions are approximate, not live FX
- Hangar data is per-device; there is no account or sync
- Loaner ship data field is unconfirmed and may not populate

## Not affiliated with Cloud Imperium Games

Fan-made reference tool. Star Citizen®, Roberts Space Industries® and associated
logos are property of Cloud Imperium Rights LLC. No game assets are redistributed.
