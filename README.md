# Nicholas County the Game — playtest builds

Walk, drive and brawl around the real Nicholas County, West Virginia. Start at home in Richwood;
the whole county is out there.

**Current build: 2026.11.14.1808** — Street names: the HUD shows the road you're on, the map labels the streets as you zoom in, and green name blades stand at the intersections in town. Roads, driveways and parking lot edges meet the ground smoothly instead of standing up as a ledge (a road up on a bank has a gentle gravel slope down to the grass, and a street above a driveway no longer sits on a cliff), and cars and you on foot roll or step up over a small lip instead of catching on it. Townsfolk stay on the sidewalks inside town and village limits: they keep to their side of the street and only rarely cross at an intersection (never kids mid-block), and nobody wanders into a lake, walks through a building or steps off a bank. Outside town there are no random walkers on the highway — only the odd person standing at a camp, park, marina, store or gas lot, or a hitchhiker at a pull-off. Pond owners stop at the water's edge. The Richwood and Craigsville GoMarts sell gas on the phone's Maps app, the same as the pumps out front. 4 Seasons Outfitters is in the phone's Maps app with its hours, just outside Richwood past the GoMart. Summersville Family Medicine goes by its real name. A smaller download: string lights, wires and thin rails in the yards use fewer pieces.

These are early playtest builds. The launcher installs the game, adds it to Steam, and pulls the newest build every
time you start it, so you only install once. Each start shows a small status window first: *Checking for updates…*,
then *Up to date: 2026.11.11.0532* (gone in a second or two), or the download with its progress and *Installed …*. With
no internet it says so and plays the build you have. The build before each update is kept, so if a new one misbehaves
the launcher menu can go back to it.

## Windows (desktop, laptop, ROG Ally)

1. Download **[Install-Nicholas-County.cmd](https://github.com/carterisanartist/nicholas-county/releases/latest/download/Install-Nicholas-County.cmd)** and double-click it.
   (If Windows SmartScreen warns about it: *More info → Run anyway*.)
2. The launcher opens and downloads the game (about 2.9 GB), then puts **Nicholas County** on your Desktop, in the Start
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
tar.gz unpack to a `NicholasCounty` folder you can run directly (no auto-updates that way). A build over 1.5 GB comes in
parts (`.001`, `.002`, ...) because GitHub limits the size of each file; join them first:
`copy /b NicholasCounty-Windows-x64.zip.001 + NicholasCounty-Windows-x64.zip.002 NicholasCounty-Windows-x64.zip` in a
Command Prompt, or `cat NicholasCounty-Linux-x64.tar.gz.0* > NicholasCounty-Linux-x64.tar.gz` on Linux. `SHA256SUMS.txt`
next to them checks a download (parts and the joined file): `sha256sum -c --ignore-missing SHA256SUMS.txt` on Linux,
or compare with `Get-FileHash NicholasCounty-Windows-x64.zip` in PowerShell.
