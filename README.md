# Nicholas County the Game — playtest builds

Walk, drive and brawl around the real Nicholas County, West Virginia. Start at home in Richwood;
the whole county is out there.

**Current build: 2026.11.11.0532** — Neighborhoods look lived in: yard trees, shrubs and rhododendrons, mailboxes at the road, propane tanks, woodpiles and picket fences around the houses. Parking lots are striped, and the lots and streets in Summersville, Richwood and Craigsville are full of parked cars (busier toward the middle of town). Towns follow the clock: more people and cars at the morning and after-work rushes and lunchtime, nearly empty streets at 3 AM. The county sounds alive: birds by time of day (cardinals, chickadees, wood thrushes at dusk, a hawk overhead), crickets and katydids at night, spring peepers by ponds, creeks and rivers you can hear, wind up on the ridges, dogs barking in town, all quieter indoors and in a car. Fishing: a real fight on the line. Hold to reel, let up when the line goes red or the fish runs, keep it from going slack. 17 kinds of local fish with real sizes, a species log, and a catch card for every fish (first catch, new species, personal bests). Hunting: bucks carry antlers (4 to 10 points), hit deer leave a blood trail to follow, deer blow and bears huff when they spot you, and a trophy card for every tag (best rack, biggest yet). Your records show on the map screen. Summersville Lake is busy: bass boats and jet skis with people aboard run the open water, idle through the marina's no-wake zone, stop to fish, and steer around you. The Summersville Lake Lighthouse stands on the ridge over the lake (104 ft, white with a black lantern and double gallery), and after dark its beacon sweeps the lake. Summersville Lake's sandstone cliffs: the steep shores of the lower lake rise out of the water in stepped ledges of tan and grey rock, with fallen boulders at the waterline and scattered along the rest of the shore. You can climb out onto them and run a boat into them. Lakes, ponds and rivers have moving water: wind ripples, the sun glinting off it, and the sky and shoreline reflected at a low angle. Summersville Lake's shore is wooded down to the water instead of a bare tan strip, with rhododendron and laurel thickets under the trees and along the cliff tops, and stones and cobbles along the waterline; no more trees growing out of the cliff faces. The lake cliffs break into jutting and overhanging blocks with a water-darkened band at the waterline, and the rock reads as bedded sandstone instead of brickwork. Sun glint on the water no longer burns out to a white sheet when you look down-sun from a ridge or the helicopter. Traffic in town drives past parked cars instead of stopping behind them, and Summersville's downtown streets have curb parking again. Cars no longer clip the bumper of the first or last car in a parked row. After fast travel, the town you land in fills with traffic in a second or two instead of trickling in one car at a time. Store and church parking lots are paved: most mapped lots had their stripes painted on bare ground (the lot surface was never laid), and they were missing from the map. They're dark asphalt now, and town yards have more and bigger shade trees.

These are early playtest builds. The launcher installs the game, adds it to Steam, and pulls the newest build every
time you start it, so you only install once.

## Windows (desktop, laptop, ROG Ally)

1. Download **[Install-Nicholas-County.cmd](https://github.com/carterisanartist/nicholas-county/releases/latest/download/Install-Nicholas-County.cmd)** and double-click it.
   (If Windows SmartScreen warns about it: *More info → Run anyway*.)
2. The launcher opens and downloads the game (about 1.3 GB), then puts **Nicholas County** on your Desktop, in the Start
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

3. Switch back to Game Mode. **Nicholas County** is in your library under *Non-Steam*. Starting it updates it first.

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
tar.gz unpack to a `NicholasCounty` folder you can run directly (no auto-updates that way).
