# Darrilla Software

The public website for Darrilla Software at https://darrilla.com, hosted by
GitHub Pages from the `main` branch of this repository.

- `/`: studio home and games.
- `/about/`: studio, mascot, and replayable publisher intro.
- `/chess-clock/`: overview, with `/support/` and `/privacy/` underneath.
- `/arrowzilla/`: overview, with matching support and privacy pages.
- `/fuzzrilla/`: beta overview, support/how-to-play and current-build privacy.
- `/monkeyrilla/`: test overview, support/how-to-play, privacy and Android enrollment.
- `/testing/`: Google Play closed-test links and enrollment help for all four games.

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
illustrations and publisher intro come from ArrowZilla. The app repositories remain the source for the originals; existing website
exports use optimized images. MonkeyRilla uses its original approved icon.
The ArrowZilla illustrations are labeled as artwork rather than screenshots.
FuzzRilla's optimized icon and crew sheet come from `games/fuzzrilla/` in the
`darrilla-games` repository. The sheet is labeled as character artwork, not a
gameplay screenshot. Its pages describe the 100-level Android/iPhone/iPad beta
chapter. Tester menus
can differ while updates roll out, so help mentions current and earlier labels.
FuzzRilla has no ads/purchases/analytics. ArrowZilla pages cover campaign and Daily
puzzles without freezing an expanding level count. Its iOS copy advertises invited
TestFlight access, not an unverified public download or a stale review status.

Chess Clock retains its public store links and adds the separate Android closed
test. All four games link to their closed test from overview/support/privacy and
the testing hub. Google account eligibility is still required. MonkeyRilla’s URL
was read from its Play console; first release 0.1.0 (2) is submitted for review.
Its TestFlight internal group matches ArrowZilla’s ten testers; the matching
one-tester external group is waiting for Beta App Review. Personal invitation
URLs and tester emails are never published.

MonkeyRilla's icon is copied byte-for-byte from
`darrilla-games/games/monkeyrilla/Assets/MonkeyRilla/Art/monkeyrilla-icon.png`.
Its source GUID `384bf57b631f94496a04e651038f6c03` is assigned to the game's
default and Android icons; the build configuration applies that same asset.
The pages describe the current 40-level gathering candidate, not the inactive
campaign or a completed store release. Preserve the approved supplied art.

ArrowZilla's privacy page distinguishes tester demo ads from SDK data handling,
local saves, platform reports and optional purchases. Keep each policy aligned
with the distributed app; a demo ad is not a no-data guarantee. `app-ads.txt` contains
the AdMob authorized-seller entry; store listings must link this developer site
before AdMob can verify it.


## Validation and release boundaries

On October 25, 2026, `bundle exec jekyll build --strict_front_matter` passed.
The generated site has 18 HTML pages with checked internal links, image sources,
anchors, all four games’ closed-test URLs and sitemap entries.
Browser checks covered the desktop homepage, MonkeyRilla at 390px and Testing at
320px, without horizontal overflow or missing images.

The MonkeyRilla Android APK was inspected with `aapt2`: its application icon is
an adaptive icon with the configured Baby Monkey artwork in the packaged
background. Default/Android Unity icon assignment and the identical website
source were verified. The subsequent 0.1.0 (2) tester release uses the same icon
on Android and Apple; both store records and uploads have now been created.

The established Google test links reach Google sign-in; this does not verify a specific
account's eligibility or enroll anyone. The user confirmed closed testing is
available. Chess Clock's public Apple listing was checked. ArrowZilla's public
iOS download could not be verified, so the copy only advertises invited testing.
Website publication uses `main` at the repository root, with `darrilla.com` as
the GitHub Pages domain. Source/status changes here do not submit app releases,
change tester lists, authorize live ads or establish device acceptance.
