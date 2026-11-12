# Nicholas County the Game — playtest builds

Walk, drive and brawl around the real Nicholas County, West Virginia. Start at home in Richwood;
the whole county is out there.

**Current build: 2026.11.11.2258** — Smoother hills: wherever a road changes grade (cresting a hill, bottoming out in a dip, or a side street climbing away from the road it leaves) it now rounds over like a real road instead of bending sharply where the car would jolt or launch. In Richwood, Cemetery Road and Edgewood Avenue leave Main Street without the twist and hump they had, and Main Street itself rides flat. Bumps where one road meets another are down by more than two thirds county-wide. Bridges drive like part of the road: no more ramp up onto the deck. A bridge carries on at the same grade as the road leading onto it, the little hump over the middle is gentle (short bridges are nearly flat), and a bridge between two banks at different heights climbs gently instead of being one steep ramp (Trout Valley's was 29%). The lip where a road bends onto a bridge is gone, a bridge that turns off a road at an intersection stays level with that road until you're off it, gravel shoulders and driveways no longer stick up onto bridge decks, and a short street between an intersection and a bridge no longer dives down to the riverbank (Oakford Avenue in Richwood).

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
