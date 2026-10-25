# Darrilla Software

The public website for Darrilla Software at https://darrilla.com, hosted by
GitHub Pages from the `main` branch of this repository.

- `/`: studio home and games.
- `/about/`: studio, mascot, and replayable publisher intro.
- `/chess-clock/`: overview, with `/support/` and `/privacy/` underneath.
- `/arrowzilla/`: overview, with matching support and privacy pages.
- `/fuzzrilla/`: development overview, support/how-to-play and current-build privacy.

The site uses a shared Jekyll layout and CSS, with no external fonts, trackers,
or client-side framework. Existing Chess Clock URLs and Google verification
files are retained. `CNAME` and `_config.yml` use `darrilla.com`.

## Local preview

```sh
bundle install
bundle exec jekyll serve
```

Open http://127.0.0.1:4000. For a static build, use
`bundle exec jekyll build`.

## Assets and copy

The mascot and Chess Clock icon come from the chess-clock app. The red panda
illustrations and publisher intro come from ArrowZilla. Website copies are
optimized for size; the app repositories remain the source for the originals.
The ArrowZilla illustrations are labeled as artwork rather than screenshots.
FuzzRilla's optimized icon and crew sheet come from `games/fuzzrilla/` in the
`darrilla-games` repository. The sheet is labeled as character artwork, not a
gameplay screenshot. Its pages describe Android and iPhone/iPad tester update
0.4.6 (17): 100 finite levels, directional/double drums, Boom, anchored ice, 8×8 boards and Lightning.
The game has no ads/purchases/analytics and no public store download. Tester
availability depends on store processing/review.

ArrowZilla links to its Google Play closed test and labels the public iOS listing
as awaiting approval. Update availability when Apple approves the release.
Its privacy page covers development test ads and planned AdMob consent and
purchase features. Keep it aligned with the released app. `app-ads.txt` contains
the AdMob authorized-seller entry; store listings must link this developer site
before AdMob can verify it.
