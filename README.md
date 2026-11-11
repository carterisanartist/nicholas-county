# Nicholas County the Game — playtest builds

Walk, drive and brawl around the real Nicholas County, West Virginia. Start at home in Richwood;
the whole county is out there.

**Current build: 2026.11.11.1341** — Roads drive smooth: no more invisible bumps that stopped the car dead. Road surfaces follow one smooth height line, the ground never pokes up through the pavement, and houses that stood out in the street (the house outlines and the road lines in the map data didn't agree) have been moved back to the roadside. Porches and front steps no longer reach into the street either: a house close to the road gets a shallower porch, steps that come down along the wall, or its door round the side. Side streets meet the road they leave level, instead of ending in a ledge over its lane on hillsides: across the whole intersection, on hills too, and at offset crossings where a street's two halves meet the cross street a few meters apart. Streets that stopped just short of the road they meet now reach it. Guardrails along drop-offs, bridge approaches and hillside curves, and you can hit them. Carter's pick of a Richwood house is rebuilt from its photos: red, two stories, full front porch, the driveway climbing up the side to a level back yard. The house crowding it on the corner is gone. Richwood City Pool: jump in and swim. Steps into the shallow end, a deep end with a diving board, lifeguard chair, bath house and a fenced deck. Backyard pools around the county are swimmable too (no fishing in them). Richwood's skate park beside the pool: two quarter pipes, a funbox, a grind rail and a manual pad. Ball fields: Richwood's diamonds and the rest of the county's have skinned infields, bases, a mound, dugouts, backstops, outfield fences, bleachers and lights. The high school football field has its lines, goalposts and scoreboard, and the basketball and tennis courts, soccer fields and playgrounds are built where they really are. They're all on the map. The launcher says what it's doing every time you press Play, on the Steam Deck (Game Mode too) and on Windows: "Checking for updates", then "Up to date" with the build number, or the download with its progress and "Installed". With no internet it says so and plays the build you have. The build before each update is kept, and the launcher can go back to it if a new one misbehaves. If GitHub doesn't answer, updates come from carterware.net instead.

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
