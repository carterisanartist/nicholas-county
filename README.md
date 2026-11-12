# Nicholas County the Game — playtest builds

Walk, drive and brawl around the real Nicholas County, West Virginia. Start at home in Richwood;
the whole county is out there.

**Current build: 2026.11.12.1305** — You have a bank account: everyone starts with checking and savings at Hemlock Savings Bank in Richwood (older saves get theirs on the next load). Counters take cash first and your debit card when cash runs short; AC's Lounge is cash only. The HUD shows cash and bank, and every dollar in or out is recorded with who, why and when. Days and weekdays: the county keeps a calendar. Stores, bars and restaurants keep their real weekly hours, and a locked door tells you when it opens next ("Opens Monday at 9 AM"). The Par Mar is open 24 hours. The map calls Mansfield Motors a car dealer (it said doctor's office), and the banks and clinics carry their in-game names. Admin menu Give tab: give or take money (presets or any amount, set an account exactly), give any item in the county by searching for it, set the time, skip days, full heal. On in development builds; in release builds switch it on under Debug (or launch with -ncAdmin), and online guests need the host to allow it. A save that used it is marked "admin used". The build number ("build 2026.11.11.0532 Linux player") is on the map menu and in the admin menu, for bug reports. Reset saves now clears everything (money, bank, calendar, cars, fishing and hunting records, and anything added later) except your settings, photos and songs. Two drinks ordered back to back both count now (the second used to cut the first one short). Carter's pick of a Richwood house: the back yard is its natural slope again (the leveled yard behind it is gone), a gravel driveway comes in from the street behind up to a parking pad beside a new walk-out basement door (the house sits high on its hill, so the back shows a stone basement wall with the door and two windows at ground level), and there are grown yard trees and stone-edged flower beds (black-eyed Susans, daylilies, coneflowers, phlox) along the back wall and the drive. The corner house stays gone.

These are early playtest builds. The launcher installs the game, adds it to Steam, and pulls the newest build every
time you start it, so you only install once. Each start shows a small status window first: *Checking for updates…*,
then *Up to date: 2026.11.11.0532* (gone in a second or two), or the download with its progress and *Installed …*. With
no internet it says so and plays the build you have. The build before each update is kept, so if a new one misbehaves
the launcher menu can go back to it.

## Windows (desktop, laptop, ROG Ally)

1. Download **[Install-Nicholas-County.cmd](https://github.com/carterisanartist/nicholas-county/releases/latest/download/Install-Nicholas-County.cmd)** and double-click it.
   (If Windows SmartScreen warns about it: *More info → Run anyway*.)
2. The launcher opens and downloads the game (about 1.2 GB), then puts **Nicholas County** on your Desktop, in the Start
   menu, and in your Steam library.

Or from PowerShell:

```powershell
iex (New-Object Net.WebClient).DownloadString('https://github.com/carterisanartist/nicholas-county/releases/latest/download/install.ps1')
```

## Steam Deck (and Linux)

1. Switch to **Desktop Mode** (Steam button → Power → Switch to Desktop).
2. Open **Konsole** and run:

   ```bash
   curl -fsSL https://github.com/carterisanartist/nicholas-county/releases/latest/download/install.sh | bash
   ```

3. Switch back to Game Mode. **Nicholas County** is in your library under *Non-Steam*. Starting it updates it first
   (the status window shows over Game Mode). **Nicholas County Launcher** on the desktop has *Check for updates*, the
   installed and newest versions, and *Go back to the previous build*.

## Playing together

Needs Steam open and signed in. In the game press the **Menu** button (F1 on a keyboard) → **Online**. One person
hosts and reads out the 6-letter code (or invites Steam friends); everyone else joins. Works over the internet with no
port forwarding, up to 8 players. Steam shows you as playing "Spacewar" while online — that's normal for playtest
builds.

## Controls

Keyboard + mouse or any controller (Xbox, Steam Deck, ROG Ally); the on-screen prompts follow whatever you touched
last. **F** / **Y** gets in and out of cars, **M** / **View** opens the travel map, **F1** / **Menu** opens the menu.

## Manual downloads

Every build is on the [Releases](https://github.com/carterisanartist/nicholas-county/releases) page: the Windows zip and the Linux
tar.gz unpack to a `NicholasCounty` folder you can run directly (no auto-updates that way). `SHA256SUMS.txt` next to
them checks a download: `sha256sum -c --ignore-missing SHA256SUMS.txt` on Linux, or compare with
`Get-FileHash NicholasCounty-Windows-x64.zip` in PowerShell.
