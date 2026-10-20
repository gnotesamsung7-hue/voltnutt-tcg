# Voltnutt: Road to the Origin Press

A trading card game set in the world of Voltnutt, Ampera and Unit 7. Battle the eight elemental toy factories on the road to the Origin Press.

## Get the APK

Every push to `main` builds the app on GitHub Actions.

1. Open the **Actions** tab and wait for **Build APK** to turn green (about 3 to 5 minutes).
2. Open **Releases** on the repo's main page and download `voltnutt-tcg.apk` from the newest build.
3. Open the file on your phone and allow installing from this source if Android asks.

New builds install over the old one and keep your saved decks and progress.

## Where things live

- `app/src/main/assets/www/index.html`: the whole game (cards, art, battle system)
- `app/src/main/assets/www/voice/`: your recorded voice lines (see `VOICE_SCRIPT.md`)
- `app/src/main/assets/www/fonts/`: Bungee and Barlow Semi Condensed (SIL Open Font License, see `OFL.txt`)
- `.github/workflows/build-apk.yml`: the build

## Adding voice lines

Record the lines in `VOICE_SCRIPT.md`, name each file exactly as listed (for example `voltnutt_win.m4a`), upload them into `app/src/main/assets/www/voice/`, and commit. A new APK builds automatically.

## Battle music

Battles have built-in music that changes with each factory. To use your own track, add `battle.mp3` (or a factory name like `fire.mp3`) to `app/src/main/assets/www/music/`. See the README in that folder.
