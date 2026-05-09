# DeckSide Releases

Public release artifacts (Windows installer + electron-updater feeds) for [DeckSide](https://deckside.app), the swim-meet day desktop app for EBSL coaches.

- **Latest release**: see [Releases](https://github.com/sportside-app/deckside-releases/releases)
- **Source code**: the actual DeckSide source code lives in a **separate private repository** and is **not** in this repo

## What's in this repo

Only this README. Each tagged release on the [Releases](https://github.com/sportside-app/deckside-releases/releases) page has the following compiled artifacts attached:

- `DeckSide-Setup-X.Y.Z.exe` — Windows NSIS installer
- `DeckSide-Setup-X.Y.Z.exe.blockmap` — delta-update map for electron-updater
- `latest.yml`, `latest-beta.yml`, `latest-alpha.yml` — electron-updater feed manifests

Installed DeckSide clients fetch the `.yml` files on launch to check for updates and pull new installers from here — no GitHub token required because the repo is public.

## ⚠️ About the "Source code" links on each Release page

GitHub automatically attaches **Source code (zip)** and **Source code (tar.gz)** links to every release page. **These do not contain DeckSide source code.** They contain only this README, because that is the only file in this repo. The actual DeckSide source code is in a separate private repository (`ronnierosal/deckside`) and never gets distributed publicly.

GitHub provides no way to disable those auto-attached source links, so they will appear on every release. Ignore them.
