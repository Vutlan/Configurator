# Vutlan Configurator

Plan a [Vutlan](https://www.vutlan.com) monitoring system on the real controller panels. Press **+ / −** at each port to connect sensors, CAN extensions, Modbus meters, LoRaWAN sensors and outputs. The Configurator enforces every controller limit. It produces a parts list, a connections list, checks, and Excel / PDF exports.

**Open it:** https://configurator.vutlan.com

Controllers: VT825, VT855 (all power versions), VT335G, VT336t, VT225t, LR800 (LoRaWAN).

## Planning with an AI assistant
Give your AI assistant (Claude, ChatGPT, …) the file [`llms.txt`](llms.txt) first: https://configurator.vutlan.com/llms.txt. It lists every controller, port, sensor, limit and rule the Configurator uses, and how to lay out a project.

## Your data
Projects are saved only in your own browser (localStorage). Nothing is sent to Vutlan or anyone else. Use **Export** to keep a copy as Excel or PDF.

## Run it offline
Download this repository (**Code → Download ZIP**), unzip it and open `index.html` in your browser. Everything works without an internet connection.

## How this site is built
Plain static files: `index.html` (the whole app), `images/` (WebP panel and product pictures), `fonts/` and `lib/` (self-hosted, no external requests). The site is served by GitHub Pages on the custom domain in `CNAME`; `.nojekyll` makes Pages serve the files as they are.

## Third-party components
- SheetJS Community Edition 0.18.5 (Apache 2.0): `lib/xlsx.full.min.js`
- html-to-image 1.11.11 (MIT): `lib/html-to-image.js`
- jsPDF 2.5.1 (MIT): `lib/jspdf.umd.min.js`
- Barlow, Barlow Condensed, JetBrains Mono fonts (SIL Open Font License), via Fontsource

## Licence
© Vutlan. All rights reserved, except the third-party components listed above, which keep their own licences. See [LICENSE](LICENSE).

Questions and corrections: https://www.vutlan.com
