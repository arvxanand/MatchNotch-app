# MatchNotch

**Live football, NBA and UFC, in the MacBook notch.**

While your team plays, the score sits either side of the camera. Click the
notch and it opens into a panel with the events, stats, lineups and table.
When nothing is on, it draws nothing and the notch looks like a notch.

Follow up to six teams from the Premier League (plus the FA Cup, EFL Cup,
Champions League and Europa League) and the NBA, or every UFC card. No account,
no setup beyond picking them. The score is held back so the notch never
tells you about a goal before your stream shows it.

This repository holds the downloads only.

## Install

You need a MacBook with a notch, Apple Silicon (M1 or later), and macOS 14
Sonoma or later.

1. Download **[MatchNotch.dmg](https://github.com/arvxanand/MatchNotch-app/releases/latest/download/MatchNotch.dmg)**.
2. Open it and drag **MatchNotch** into **Applications**.
3. Open MatchNotch from Applications. macOS says it can't verify the
   developer, because the app isn't notarised (there's no paid Apple Developer
   account behind it). Close the message.
4. Open **System Settings → Privacy & Security**, scroll down to the message
   about MatchNotch, and click **Open Anyway**. Confirm with your password.
   You only do this once.
5. The notch asks which teams to follow. Pick up to six, in the order you care
   about them.

To start it when you log in: menu bar icon → **Settings… → General → Open at
login**.

### Or with Homebrew

```bash
brew install --cask arvxanand/matchnotch/matchnotch
```

The cask skips step 3 and 4.

## Using it

- **Point** at the notch to bring the score to full strength.
- **Click** the notch to open the panel; click anywhere outside it to close.
- **Swipe** sideways on the notch to change team.
- **⌥⌘A** opens and closes the panel from anywhere.
- The **menu bar icon** shows your teams and the next game, and opens
  Settings (⌘,).

## Privacy

No account, no analytics, no server of its own. It asks for:

- **ESPN's public match data** (`site.api.espn.com`, `site.web.api.espn.com`)
  for scores, schedules, events, lineups and tables, and crests and headshots
  from `a.espncdn.com`.
- **FotMob's match data** (`www.fotmob.com`, `images.fotmob.com`) for the
  pitch, player ratings, shot maps, injuries and the weather.
- **GitHub** (`api.github.com`, `github.com`), once a day, to see whether a
  newer MatchNotch is out. A new version downloads in the background and
  installs only when you click **Update**. Turn it off in Settings → General
  → Check for updates.

It polls fast only while a match is on. Your teams and settings stay on your
Mac.

## Uninstall

1. Quit MatchNotch (menu bar icon → Quit), and turn off Open at login first if
   you turned it on.
2. Drag **MatchNotch** from Applications to the Bin.
3. To remove its settings and caches too, delete these (Finder → **Go → Go to
   Folder…**):
   - `~/Library/Preferences/io.github.arvxanand.matchnotch.plist`
   - `~/Library/Caches/MatchNotch`
   - `~/Library/Application Support/MatchNotch`

With Homebrew: `brew uninstall --zap --cask matchnotch`.

## Something wrong?

[Report a bug](https://github.com/arvxanand/MatchNotch-app/issues/new/choose)
or suggest an idea.

---

MatchNotch is not affiliated with, endorsed by or connected to ESPN, FotMob,
the Premier League, the NBA, the UFC, or any league or club. Names, crests and
data belong to their owners.

Copyright © 2026 Arav Anand. All rights reserved. See [LICENSE](LICENSE).
