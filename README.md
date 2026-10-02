# Eclipse V2 BETA — Free AION 2 DPS Meter & Combat Analyzer

![Eclipse V2 BETA — AION 2 party DPS meter, Glass client and combat analysis for Windows](docs/images/eclipse-banner.svg)

[![Latest release](https://img.shields.io/github/v/release/Iota-Nine/Aion2-Eclipse?label=Download&color=75bdcf)](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/Iota-Nine/Aion2-Eclipse/total?color=9384d0)](https://github.com/Iota-Nine/Aion2-Eclipse/releases)
![Public BETA](https://img.shields.io/badge/V2-PUBLIC%20BETA-d8bd88)
![Windows x64](https://img.shields.io/badge/Windows-x64-507cab)
![English and French](https://img.shields.io/badge/Language-EN%20%2F%20FR-75bdcf)

**See your party's DPS while you play. Understand the whole run when you finish.**

Eclipse is a free AION 2 damage meter for Windows with a live party overlay and a full Glass desktop client. Follow damage, inspect skills, review dungeon runs and compare your builds in one place. Keep it on a second monitor, minimize it during the fight, then come back to your expedition summary.

**[Download Eclipse V2 BETA for Windows](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest)** · [Français](docs/README.fr.md) · [What's new](CHANGELOG.md) · [Report an issue](https://github.com/Iota-Nine/Aion2-Eclipse/issues/new/choose)

**V2 BETA is the main Eclipse update and replaces V1.** Existing users can use **UPDATE**; new users get the same V2 ZIP. English is the default language. French is available in Preferences. No Eclipse account or signup is required.

![AION 2 DPS meter — Eclipse V2 BETA English combat overview with party damage and skill analysis](docs/images/eclipse-combat-en.png)

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
| **Dedicated Rift timers** | Prominent portal countdown, a separate five-minute entry window and one-hour event timer, next four openings in local time and UTC. Select EU, NA, SA, JP, TW or KR from the dated Talentbuilds community reference. |
| **Rift reminders** | Favourite the Rift and enable its independent alert at 10 minutes before, 5 minutes before or opening. Region, favourite and timing are saved; reminders continue while minimized. |
| **Boss and event timers** | A dated Korean-server calendar with server time, local time, upcoming events and matchmaking groups; personal monster reminders and target segments are also available. |
| **Favourite boss alerts** | Star the event, enable **Notify me** and choose **10 minutes before**, **5 minutes before** or **at the scheduled time**. Reminders work while minimized and avoid duplicate alerts. |
| **English / Français** | English on first launch; switch client, overlay and setup labels to French. Your language choice is saved. |
| **Performance controls** | Adjust transparency, animation quality and always-on-top behaviour. Visual effects stop when minimized while capture, timers and saving continue. |
| **Exports and diagnostics** | Export run data and a share card; create a restricted diagnostic report for support. Logs and authentication tokens are excluded from that report. |
| **Guided setup and updates** | Included application runtime, automatic prerequisite check, official Npcap installation with consent when needed, shortcuts and verified in-app update downloads. |
| **Complete shutdown** | Minimize to keep collecting. Close Eclipse to quit its client, overlay and capture process. |

## Dedicated Rift timers

**Catch the entry window. Keep track of the event after the portal closes.** The Rift panel leads the Rifts & events page, works without game capture and shows your next four openings. Its countdown distinguishes a waiting portal, an open entry window and an ongoing event with entry closed.

![AION 2 Rift timer — Eclipse English Spacetime Rift portal countdown, event duration and regional favourite alerts](docs/images/eclipse-rifts-en.png)

Choose your **game server** in the Rift panel, star it and enable the reminder. Rift alerts have their own timing, separate from boss favourites. The new settings leave existing language and boss reminders intact and do not enable audio automatically.

The bundled [Talentbuilds event timeline](https://talentbuilds.com/aion2/events-timeline) reference was checked on **2 October 2026**. Its EU/NA/SA/JP/KR schedules share one clock; TW is one hour later. The site actually calculates openings in **America/New_York (EST/EDT)**, which Eclipse converts per opening to your local time. It lists a **5-minute entry window** and a **1-hour event**. The separate 6sword KR reference lists 15-minute entry. Both sources remain visible: these are attributed scheduled reminders, not confirmation from game packets or an official global timetable. Check the source and in-game notices if the schedules disagree.

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

1. Open the **[latest release](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest)** and download **`Aion2-Eclipse-v2.1.6-win-x64.zip`** under Assets. GitHub's “Source code” archives are not the application.
2. **Extract the entire ZIP** to a folder on your PC.
3. Run **`Eclipse.Setup.exe`**. Choose your language. If Npcap is missing, setup downloads its official installer, asks for Windows permission and lets you accept the installation wizard. Eclipse continues when it finishes.
4. Open AION 2. If you were already in the world, teleport or change channels once to receive your character identity. Join or refresh your party after starting Eclipse.
5. The **overlay is enabled by default**. Use the desktop client on the same display or a second monitor. Open Preferences for French, transparency and performance settings.

Setup creates Desktop and Start menu shortcuts and installs Eclipse for your Windows account. The application runtime is included; no separate .NET installation is required. Internet is needed for downloads, external sources and updates. The download targets **Windows x64**; native interface checks were performed on Windows 11.

## Upgrade from V1 or an earlier V2

**Click UPDATE in Eclipse to install the latest V2 BETA in the same folder.** V2 uses the same executable name and public update channel. Existing `data` and HUD preferences are preserved; V2 creates its own client history there. The updater verifies the release and checks the installed executable version before restarting it.

If an older updater keeps reopening V1, download the latest ZIP, extract it fully and run **`Eclipse.Setup.exe`** once. V1 is superseded; historical release pages remain available. An already downloaded V1 executable does not disable itself remotely.

## How the numbers work

**Are these real damage values?** In normal mode, Eclipse uses damage events received from AION 2 network traffic. Demo mode is explicitly marked. Values that have not arrived remain unknown; player levels are shown only when received. Capture started late, missing packets or a changed game protocol can affect completeness.

**Why doesn't DPS reset every second?** DPS is a rate calculated from damage over a duration. The HUD shows the current fight's average, the full client shows the run average, and the timeline and five-second burst view show short windows. Total damage accumulates until the run is ended or reset.

**Does it detect every dungeon name?** Automatic boundaries currently rely on the recognized local teleport / login packet, including instance transitions. Other teleports also reset the run. V2 does not claim a complete dungeon-name database, and a transition without that packet cannot be guaranteed. Party queue changes alone do not erase combat.

**Is there an official AION API?** Combat capture uses local network packets through Npcap. Eclipse also exposes its own authenticated, loopback-only local API for local integrations; that is separate from an official game API. Meta and build sources are fetched over HTTPS.

**Will it work from another country?** Your physical location and interface language do not choose the game protocol. Windows configuration, network adapters and the AION 2 server/client version matter. Choose the appropriate source region in Preferences and use the connection page to diagnose capture. BETA compatibility is not guaranteed for every machine or future regional patch.

**Are boss timers live spawn detection?** They are scheduled reminders. The built-in timetable is a dated transcription for **Korean servers**, converted to your local time, based on [6Sword's AION 2 timers](https://6sword.com/en/aion2/timers) and the linked official notices. Other regions remain pending official schedules; Eclipse does not substitute Korean times for Europe or North America. The favourite alarm is optional; the intro stays silent.

**Is the class meta universal?** No. [MetaRoad's contextual tier list](https://metaroad.gg/aion2/getting-started/aion-2-class-tier-list-before-global-launch-best-classes-for-pve-pvp) and [community builds](https://metaroad.gg/aion2/community-builds) are dated community sources. The app refreshes them at launch and periodically, shows cached dates if unavailable and keeps regional uncertainty visible. Local rankings reflect only your saved runs, not all players.

## Feedback and project information

Found a capture, update or interface problem? **[Open a bug report](https://github.com/Iota-Nine/Aion2-Eclipse/issues/new/choose)** with your Eclipse version, Windows version, game region and reproduction steps. Use the diagnostic export in Preferences and review what you share.

Eclipse is maintained by **Iota-Nine** as an independent AION 2 community project. This repository distributes prebuilt Windows releases and their documentation. Personal data, API tokens and local combat archives are not part of the public download.

AION, AION 2, NCSOFT artwork and game data belong to their respective owners. Eclipse is not affiliated with or endorsed by NCSOFT. Community packet-capture lineage and third-party components are acknowledged in the project; see [distribution terms](LICENSE).
