# Privacy

Short version: **nothing is sent to the developer.** Katofli has no telemetry, no
crash reports, no account and no keystroke logging. Update files are downloaded
from GitHub, which counts downloads; the developer sees only those totals, no
personal data. Katofli also talks to a few public
services to do its job, listed below.

## 1. Update check

Katofli looks for a newer version by reading a small file (`latest.json`) from
the releases page on GitHub. If GitHub does not deliver that file, Katofli reads
the same file from katofli.app instead. The first check runs about 2 minutes
after start, then once a day. By default it only tells you an update exists.
GitHub sees your IP address, as any website does; so does Cloudflare, which
serves katofli.app, when that address is read. Portable copies check too but do
not install updates themselves.

## 2. Weather

While the weather module is on and you have added a location, Katofli asks
Open-Meteo (open-meteo.com) for the forecast for your saved locations: the main one about every 30 minutes while the
weather module is on, the others when you open the weather panel. The requests
contain the coordinates of those locations. With no location, nothing is sent. When you search for a place name, the text you type is sent to Open-Meteo's
place search service.

## 3. Game covers

The game bar can fetch cover art from GOG and Steam through two settings, both
on by default and both can be turned off in the game bar's settings:

- "Covers from GOG" (`online-art`) sends store game ids to GOG.
- "Search covers by name" (`online-art-search`) sends game names to Steam and GOG.

Nothing else about your library is sent.

## 4. What stays on your PC

Settings, caches (apps, weather, game library, cover art) and logs are kept in
your user folders; a portable copy keeps them in its own `data` folder. Pinned
clipboard entries are stored as plain text in `clipboard-pins.json`; do not pin
secrets. Stronger protection for pins is planned.

## 5. Links you click

Web searches, store pages and the sign-in page of a public network open in your own browser. What that site learns is
governed by that site.

## 6. Downloads and changes

Download pages are hosted by GitHub. If this note changes, the new text ships
with the next version.

## Contact

Questions or concerns: open an issue at
<https://github.com/lidatheo/katofli-releases/issues>.
