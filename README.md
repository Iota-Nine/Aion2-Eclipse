# Eclipse â€” Free AION 2 DPS Meter for Windows

![Eclipse AION 2 DPS meter â€” live party damage overlay for Windows](docs/images/eclipse-banner.svg)

[![Latest release](https://img.shields.io/github/v/release/Iota-Nine/Aion2-Eclipse?label=Download&color=75bdcf)](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/Iota-Nine/Aion2-Eclipse/total?color=9384d0)](https://github.com/Iota-Nine/Aion2-Eclipse/releases)
[![Windows x64](https://img.shields.io/badge/Windows-x64-507cab)](#installation)

**Eclipse is a free AION 2 damage meter with a live party DPS overlay, total damage, player levels and a movable HUD.** Follow your group's combat performance while playing. No account or signup required.

**[Download Eclipse for Windows](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest)** Â· [FranÃ§ais](docs/README.fr.md) Â· [What's new](CHANGELOG.md) Â· [Report a bug](https://github.com/Iota-Nine/Aion2-Eclipse/issues/new/choose)

Download the **Windows `.zip` asset**, not GitHub's â€œSource codeâ€ archive. This repository distributes prebuilt binaries; application source code is not published here.

## Available now

| Feature | What it does |
|---|---|
| **Live party DPS meter** | Shows received damage and average damage per second for your party. |
| **Total combat damage** | Keeps damage totals across targets until the encounter is reset. |
| **Player levels** | Displays levels when identity packets provide them; missing levels remain unknown. |
| **Movable, click-through overlay** | Position the compact HUD on your game screen and let clicks pass through. |
| **Guided Windows setup** | Detects prerequisites, opens the official Npcap installer when needed and creates shortcuts. |
| **In-app updates** | Verifies downloads, installs the release and reports failures. |
| **Complete shutdown** | Closing Eclipse quits its auxiliary windows and capture process. |

## Installation

1. Open **[the latest release](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest)** and download `Aion2-Eclipse-â€¦-win-x64.zip`.
2. Extract the **entire ZIP** to a writable folder, such as Documents.
3. Run **`Eclipse.Setup.exe`**.
4. Accept the Windows permission prompt. If Npcap is missing, setup downloads and opens its official installer: review and accept its installation wizard.
5. Open AION 2, enter the world and use a skill. If Eclipse was started after entering the world, teleport or change channels once. Join your party after starting Eclipse so its identity information can be received.

Setup installs Eclipse in your Windows user account and creates Desktop and Start menu shortcuts. The .NET runtime is included. Internet access is required for downloads and for fetching [Npcap](https://npcap.com/#download) when absent.

**Windows 11 x64 is recommended.** Existing portable installations can continue to run; missing prerequisites also trigger setup guidance at first launch.

## Updates and recent fixes

Click **UPDATE** in Eclipse. The release download is checked before Eclipse closes; the client restarts after installation.

**v1.0.30 fixes the update loop and processes left running after closing the window.** It also improves recovery from locked or read-only files and exposes update failures. See the [changelog](CHANGELOG.md) and [release notes](https://github.com/Iota-Nine/Aion2-Eclipse/releases/tag/v1.0.30).

**Stuck on an older version?** Close Eclipse, download the latest ZIP, extract it and run **`Eclipse.Setup.exe` once**. This replaces the old update tool; subsequent updates can use UPDATE normally.

## Controls

| Action | Shortcut |
|---|---|
| Hide / show the HUD | `Ctrl+Shift+H` |
| Toggle click-through | `Ctrl+Shift+L` |
| Reset the encounter | `Ctrl+Shift+R` |

## Frequently asked questions

**Does it work in Europe or with a different Windows language?**

There is no country or Windows-language restriction. Compatibility depends on the AION 2 client protocol, capture driver and PC configuration. Every region and machine has not been validated; a country alone does not establish compatibility.

**Does Eclipse use an official AION 2 API?**

Combat values come from locally received network events. Eclipse does not obtain damage from an official NCSOFT combat API. Its local API is a separate interface for reading Eclipse's own state.

**Why doesn't DPS reset to zero every second?**

Encounter DPS is **total received damage Ã· encounter duration**. It is an average, so it does not reset each second. A rolling burst measurement answers a different question: damage over a recent time window.

**Are the damage values real?**

Live damage values are calculated from received combat events. Missing packets, incomplete identity information or a game protocol change can limit coverage. Unknown levels and missing information are not invented. A DPS ranking alone does not measure tanking, healing or support quality.

**Npcap missing, no party or unknown levels?**

Run `Eclipse.Setup.exe`, finish the Npcap wizard if offered, then start Eclipse before entering the world. Teleport or change channels once and rejoin the party. If it persists, [report the problem](https://github.com/Iota-Nine/Aion2-Eclipse/issues/new/choose) with your Eclipse version, Windows version, game region and reproduction steps.

## Eclipse V2 â€” prototype in development

A separate, unpublished V2 prototype is being tested: a glass desktop client for a second monitor, expedition summaries, per-player and per-skill analysis, selectable timelines, A/B run comparison, personal build profiles, dated meta sources and monster combat timers with personal respawn reminders.

**These V2 features are not included in the current public v1.0.30 ZIP.** Respawn reminders use a user-declared delay and server/channel context; they are not a verified universal spawn schedule. Demonstration screenshots contain fictional data. Meta sources are dated and region-specific; a KR ranking is not presented as a validated European meta.

![Eclipse V2 prototype â€” glass AION 2 party DPS client with fictional demonstration data](docs/images/eclipse-v2-prototype-combat.png)

![Eclipse V2 prototype expedition summary â€” party damage and peak burst using fictional data](docs/images/eclipse-v2-prototype-summary.png)

Prototype interface previews; **not the released v1 client**. AION 2 artwork: NCSOFT, from the official AION 2 website. These are demonstration captures, not player-performance benchmarks.

## Support and project terms

[Report a bug](https://github.com/Iota-Nine/Aion2-Eclipse/issues/new/choose), include useful reproduction details, and avoid sharing API tokens or account credentials. If Eclipse helps your party, starring the repository helps other players discover it.

Free for personal use under the [binary distribution terms](LICENSE). Eclipse is an independent community tool and is not affiliated with NCSOFT. AION 2 and related artwork belong to their respective owners.
