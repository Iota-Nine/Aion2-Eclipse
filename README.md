# Eclipse 2.1.8 — Free AION 2 DPS Meter & Combat Analyzer

![Eclipse 2.1.8 — AION 2 party DPS meter, Glass client and combat analysis for Windows](docs/images/eclipse-banner.svg)

[![Latest release](https://img.shields.io/github/v/release/Iota-Nine/Aion2-Eclipse?label=Download&color=75bdcf)](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/Iota-Nine/Aion2-Eclipse/total?color=9384d0)](https://github.com/Iota-Nine/Aion2-Eclipse/releases)
![Version 2.1.8](https://img.shields.io/badge/Version-2.1.8-d8bd88)
![Windows x64](https://img.shields.io/badge/Windows-x64-507cab)
![English and French](https://img.shields.io/badge/Language-EN%20%2F%20FR-75bdcf)

**See your party's DPS while you play. Understand the whole run when you finish.**

Eclipse is a free AION 2 damage meter for Windows with a live party overlay and a full Glass desktop client. Follow damage, inspect skills, review dungeon runs and compare your builds in one place. Keep it on a second monitor, minimize it during the fight, then come back to your expedition summary.

**[Download the Windows installer (.exe)](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest/download/Eclipse-Setup.exe)** · [Français](docs/README.fr.md) · [What's new](CHANGELOG.md) · [Report an issue](https://github.com/Iota-Nine/Aion2-Eclipse/issues/new/choose)

**Eclipse 2.1.8 is the main Eclipse update and replaces V1.** Existing users can use **UPDATE**; new users download **Eclipse-Setup.exe**, which includes the complete application. English is the default language. French is available in Preferences. No Eclipse account or signup is required.

![AION 2 DPS meter — Eclipse 2.1.8 English combat overview with party damage and skill analysis](docs/images/eclipse-combat-en.png)

*Native screenshot of the released client. All gallery combat values are explicitly labelled demo data.*

## A clearer view of every fight

| Feature | What you get |
|---|---|
| **Live party DPS overlay** | Your party's observed DPS, total damage, contribution and received player levels. The HUD starts enabled and shares the client's measurements. |
| **Glass desktop client** | Translucent panels, animated AION artwork, Eclipse branding and an entirely silent startup intro. Move, resize or place the client on another monitor. |
| **Dungeon / teleport reset** | A recognized local teleport packet ends the previous run and resets damage and DPS. The previous summary is archived before the next hits are counted. |
| **Party and skill analysis** | Inspect each member's damage, skill breakdown, critical hits, back attacks, maximum hits and received death counts. Nearby players outside the identified party are excluded. |
| **Expedition summary** | Total damage, duration, party contribution, burst windows, gaps between hits and target segments, together with the declared build used for that run. |
| **Interactive damage timeline** | Select a time range, inspect individual hits and find strong five-second burst windows. Large runs keep complete totals and mark partial timeline coverage when relevant. |
| **Run history** | Local archives, search and filters, favourites, notes, interrupted-run recovery and configurable retention. Reopen a previous encounter after the dungeon. |
| **A/B build comparisons** | Compare completed runs with matching target, region, declared difficulty and personal class. See observed DPS, critical-hit and back-attack changes. |
| **Personal build profiles** | Save class skill selections, notes, activity and region. Your run keeps a snapshot of the selected profile for later review. |
| **Dated class meta and community builds** | Refresh MetaRoad's contextual class rankings and links to community builds. Source, update date and regional uncertainty stay visible. Your own runs also form a separate local class ranking. |
| **Dedicated Rift timers** | Regional AION2Hub openings, fixed server clock and four future local/UTC times. Global/KR UTC+9; Taiwan UTC+8. Unknown travel portal durations stay unspecified. |
| **Rift reminders** | Favourite the Rift and enable its independent alert at 10 minutes before, 5 minutes before or opening. Region, favourite and timing are saved; reminders continue while minimized. |
| **Boss and event timers** | Regional AION2Hub calendar, corrected Kaira and executor times, Abyss events, Beritra and KR/TW PvP activities. Personal monster reminders and target segments remain available. |
| **Favourite boss alerts** | Star the event, enable **Notify me** and choose **10 minutes before**, **5 minutes before** or **at the scheduled time**. Reminders work while minimized and avoid duplicate alerts. |
| **English / Français** | English on first launch; switch client, overlay and setup labels to French. Your language choice is saved. |
| **Performance controls** | Adjust transparency, animation quality and always-on-top behaviour. Visual effects stop when minimized while capture, timers and saving continue. |
| **Exports and diagnostics** | Export run data and a share card; create a restricted diagnostic report for support. Logs and authentication tokens are excluded from that report. |
| **Guided setup and updates** | Included application runtime, automatic prerequisite check, official Npcap installation with consent when needed, shortcuts and verified in-app update downloads. |
| **Complete shutdown** | Minimize to keep collecting. Close Eclipse to quit its client, overlay and capture process. |

## Dedicated Rift timers

**Know the next opening in your local time.** Select your game service, star the Rift and enable its own reminder at 10, 5 or 0 minutes. The panel shows the fixed server clock and the next four local/UTC openings.

![AION 2 Rift timer — Eclipse English regional opening countdown and fixed server clock](docs/images/eclipse-rifts-en.png)

The bundled [AION2Hub timer](https://aion2hub.com/tools/event-timer) reference was checked on **3 October 2026**, replacing the previous sources and New York clock. Global EU/NA/SA/JP uses **UTC+9** with 00:00/03:00/06:00/09:00/12:00/15:00/18:00/21:00 server openings. KR uses **UTC+9** and TW **UTC+8**, both at 02:00/05:00/08:00/11:00/14:00/17:00/20:00/23:00 server time. Local daylight saving changes the display, never the server schedule.

Travel portal entry/lifetime is **not confirmed by this source**, so Eclipse no longer presents five-minute entry or one-hour event phases as established. Domination and Abyss Rift Zone have separate sourced activity durations and are KR/TW only. Regional [boss schedules](https://aion2hub.com/tools/world-bosses) are also corrected, including Kaira's interval and executor weekdays. Unverified matchmaking offsets have been removed. These are dated community schedules, not live spawn detections or official NCSOFT confirmation.

## Official website and bug reports

**[Open the Eclipse website](https://eclipse-aion2-dps-meter.koayo.chatgpt.site)** for downloads, English/French features, client screenshots and optional ambient music. **Report a bug** in the client opens the private website form with your version filled in. Submitted fields are stored for support; JSON export is available. Combat logs and tokens are not uploaded automatically. GitHub Issues remain available for public discussions.

## Screenshots — English interface

The images below come from the native Windows application. Combat data is simulated for the gallery; no real player records are published.

### Party analysis

![Eclipse AION 2 party DPS analysis — English player damage, critical hits and skill breakdown](docs/images/eclipse-analysis-en.png)

### Expedition summary

![AION 2 dungeon run summary — total party damage, burst DPS and target segments in Eclipse](docs/images/eclipse-summary-en.png)

### Run history

![Eclipse AION 2 combat history — English saved runs, favourites and build comparison](docs/images/eclipse-history-en.png)

### Builds and dated meta

![Eclipse AION 2 builds and meta — English personal profiles and dated community sources](docs/images/eclipse-builds-en.png)

### Boss and event reminders

![AION 2 boss timers in Eclipse — English Korean-server event calendar and favourite alerts](docs/images/eclipse-timers-en.png)

### Overlay

![Eclipse AION 2 English DPS overlay — party damage, player levels and compact live HUD](docs/images/eclipse-overlay-en.png)

## Install Eclipse

1. **[Download Eclipse-Setup.exe](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest/download/Eclipse-Setup.exe)** directly. The full application, images, game data and runtime are included.
2. **Run the installer** and choose English or French. No ZIP extraction is needed.
3. If Npcap is missing, setup downloads its official installer, asks for Windows permission and lets you accept the installation wizard. Eclipse continues when it finishes.
4. Open AION 2. If you were already in the world, teleport or change channels once to receive your character identity. Join or refresh your party after starting Eclipse.
5. The **overlay is enabled by default**. Use the desktop client on the same display or a second monitor. Open Preferences for French, transparency and performance settings.

Setup creates Desktop and Start menu shortcuts and installs Eclipse for your Windows account. The application runtime is included; no separate .NET installation is required. Internet is needed for downloads, external sources and updates. The download targets **Windows x64**; native interface checks were performed on Windows 11.

## Upgrade from V1 or an earlier V2

**UPDATE appears in the full client only when a newer version is detected, just like the overlay.** A luminous progress panel shows the real download percentage, then verification and installation preparation. **Click UPDATE in Eclipse to install Eclipse 2.1.8 in the same folder.** V2 uses the same executable name and public update channel. Existing `data` and HUD preferences are preserved; V2 creates its own client history there. The updater verifies the release and checks the installed executable version before restarting it.

If an older updater keeps reopening V1, run **`Eclipse-Setup.exe`** once. The complete ZIP remains available in release assets for portable installation and in-app updates. V1 is superseded; historical release pages remain available. An already downloaded V1 executable does not disable itself remotely.

## How the numbers work

**Are these real damage values?** In normal mode, Eclipse uses damage events received from AION 2 network traffic. Demo mode is explicitly marked. Values that have not arrived remain unknown; player levels are shown only when received. Capture started late, missing packets or a changed game protocol can affect completeness.

**Why doesn't DPS reset every second?** DPS is a rate calculated from damage over a duration. The HUD shows the current fight's average, the full client shows the run average, and the timeline and five-second burst view show short windows. Total damage accumulates until the run is ended or reset.

**Does it detect every dungeon name?** Automatic boundaries currently rely on the recognized local teleport / login packet, including instance transitions. Other teleports also reset the run. V2 does not claim a complete dungeon-name database, and a transition without that packet cannot be guaranteed. Party queue changes alone do not erase combat.

**Is there an official AION API?** Combat capture uses local network packets through Npcap. Eclipse also exposes its own authenticated, loopback-only local API for local integrations; that is separate from an official game API. Meta and build sources are fetched over HTTPS.

**Will it work from another country?** Your physical location and interface language do not choose the game protocol. Windows configuration, network adapters and the AION 2 server/client version matter. Choose the appropriate source region in Preferences and use the connection page to diagnose capture. Compatibility is not guaranteed for every machine or future regional patch.

**Are boss timers live spawn detection?** They are dated AION2Hub scheduled reminders, converted to your local time. Choose the actual service: Global, Korea and Taiwan have different schedules. Favourite audio is optional; the intro stays silent.

**Is the class meta universal?** No. [MetaRoad's contextual tier list](https://metaroad.gg/aion2/getting-started/aion-2-class-tier-list-before-global-launch-best-classes-for-pve-pvp) and [community builds](https://metaroad.gg/aion2/community-builds) are dated community sources. The app refreshes them at launch and periodically, shows cached dates if unavailable and keeps regional uncertainty visible. Local rankings reflect only your saved runs, not all players.

## Feedback and project information

Found a capture, update or interface problem? **[Open a bug report](https://github.com/Iota-Nine/Aion2-Eclipse/issues/new/choose)** with your Eclipse version, Windows version, game region and reproduction steps. Use the diagnostic export in Preferences and review what you share.

Eclipse is maintained by **Iota-Nine** as an independent AION 2 community project. This repository distributes prebuilt Windows releases and their documentation. Personal data, API tokens and local combat archives are not part of the public download.

AION, AION 2, NCSOFT artwork and game data belong to their respective owners. Eclipse is not affiliated with or endorsed by NCSOFT. Community packet-capture lineage and third-party components are acknowledged in the project; see [distribution terms](LICENSE).
