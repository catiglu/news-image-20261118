# The World in One Page — 18 November 2026

A single-image summary of the day's world news, built as a premium newspaper front-page poster.

## The design
A typography-first broadsheet layout: a centered masthead ("The World in One Page") with dateline, a hero story on the historic Trump–Xi–Putin trilateral at the APEC summit in Shenzhen, a two-column grid of secondary stories (Gaza "yellow line" incursion, Crimea Bridge attack, ICJ Rohingya verdict, Anthropic IPO, Van Gogh record, Jeffers nomination, EU Ukraine loan, South Florida floods), and a thin "Also Today" ticker. Restrained paper-and-ink palette with a single oxblood accent, thin rules, small-caps section labels, system serif/sans fonts only.

## How it works
`main.ts` copies the static `entry.png` to `/output/entry.png` (or `$MAKEFUN_OUTPUT_DIR/entry.png` when testing locally). The entry is deterministic by construction: the image is a fixed asset, so every run produces a byte-identical copy — no network, no randomness, no time dependence.

## Credits
News facts from BBC News & The Guardian, 18 Nov 2026. Image rendered from `news_page.html` via Playwright + Chromium.
