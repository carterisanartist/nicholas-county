# Nicholas County the Game — playtest builds

Walk, drive and brawl around the real Nicholas County, West Virginia. Start at home in Richwood;
the whole county is out there.

**Current build: 2026.11.11.1649** — Kids can never be hurt. Swing at one and they jump out of the way and run off; a car coming at a kid gets a comedic hop out of its path (and traffic gives them extra room); rounds pass them by and you can't raise a rifle with a kid in the line of fire; dogs and wildlife leave them be. Playing as a kid, nobody picks a fight with you either. Fewer lips where one road meets another: guardrails, gravel shoulders and bridge walls stop at side roads, lanes and driveways instead of running across them (the ledge on Greenbrier Road in Richwood is gone), switchbacks and kinks in the map are rounded into proper curves, and a short road between two streets at different heights climbs smoothly from one to the other. Bridges line up with their roads: every bridge deck starts exactly level with the road leading onto it, and where the road bends onto a bridge the pavement turns with it instead of leaving a gap at the corner, so you can drive across every bridge in the county (Richwood's Cherry River bridges, the long one at Curtin, all of them).

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
