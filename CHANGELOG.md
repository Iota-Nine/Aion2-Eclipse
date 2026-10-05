# Eclipse release notes

## v3.0.1 — Live HUD healing and allied shields

### Overlay fold correction — 5 October 2026, same version 3.0.1

The **−** button now folds the overlay to its visible, draggable header. Press **+** to restore the meter. It works in compact and full views; the selected mode, width and position are retained. Live measurements and cumulative damage/healing/shield totals continue while folded. Closing the overlay still leaves the main client running.

**Already on 3.0.1?** Download the current **Eclipse-Setup.exe** and reinstall to receive this same-version correction. **UPDATE** detects higher versions, so it will not appear for an existing 3.0.1 installation. Saved runs and settings are preserved.

Validation: 56 native fold checks in English/French and compact/full modes, existing HUD support/shortcut/analysis/history checks, isolated shutdown and ZIP/setup migrations including a previous 3.0.1 installation. Screenshot uses fictional demo data.

![Folded Eclipse HUD — header stays visible, English, fictional demo encounter](https://raw.githubusercontent.com/Iota-Nine/Aion2-Eclipse/main/docs/images/eclipse-hud-folded-en.png)


Eclipse 3.0.1 brings party support into the live HUD, in compact and full modes.

- **Healing under the damage bars:** green rows show each player's observed healing total and average HPS over the run. Healers remain visible even with zero damage.
- **Shields to allies:** blue rows count recognized shield applications to other party members. Healing and shielding can appear together for the same player, including Cleric. Self-shields are excluded from these allied HUD rows.
- **More accurate shield classification:** block bonuses and protection from death no longer count as shields. Six direct shield families and five specialization-dependent families are recognized; conditional effects require the specialization flag in the received data. Selected coverage spans multiple classes, including Cleric.
- **Cleaner click-through HUD:** the large “Grab mouse back” button is removed. Press **Ctrl+Alt+L** to toggle mouse interaction; a discreet hint stays inside the HUD. If the shortcut is occupied, the HUD stays clickable. Closing the overlay keeps the main client running.

Support totals stay cumulative when live DPS returns to zero after 2 seconds without positive damage. A new run clears the support totals. English is the default; French remains available.

**Measurement limits:** shields are application counts, not damage amounts. Shield capacity, damage absorbed or blocked, effective healing and overheal remain unknown. The support decoder covers selected packet families and skills; automated checks do not establish exhaustive live-game or regional coverage.

**Install/update:** download **Eclipse-Setup.exe** below, or use **UPDATE** when it appears in Eclipse. Runtime is included; the official Npcap consent wizard is offered if its driver is missing. Existing history and preferences are preserved. The ZIP is also available for a complete extracted installation.

Validation: 615 logic checks, 26 native HUD support checks and 24 shortcut checks, plus existing analysis/history checks, isolated client shutdown, final ZIP migrations from V1 and 3.0.0, and standalone setup verification. Screenshots use fictional demo data.

![Compact HUD with healing and allied shield bars — English, fictional demo data](https://raw.githubusercontent.com/Iota-Nine/Aion2-Eclipse/main/docs/images/eclipse-hud-support-compact-en.png)

## v3.0.0 — Party healing and shield applications

Eclipse 3.0.0 adds reported party healing and observed shield applications to the Glass client's run analysis.

- **Party healing and HPS:** see received healing totals, each caster's contribution, average HPS over the full run, skill details, healing-over-time ticks and recipients. The local user can play any class; healers with zero damage remain identified in the party.
- **Shield applications:** count observed applications of selected shield skills, with companion notifications deduplicated. Shield capacity and damage absorbed are **unknown**.
- **Identity corrections:** healing and recipients remain attached to the same character across internal teleports and session-ID changes. Reused IDs do not transfer old support totals to another player.
- **Saved runs:** new archives retain support details. Earlier archives show **Not recorded**, rather than pretending they contained zero healing. Support is kept separate from DPS and total damage.
- **Diagnostics:** Preferences → Export diagnostics includes counts of recognized support candidates, accepted events and rejection reasons. Export during the affected run; these counters reset with it. The support diagnostic contains no player names, packet payloads or credentials.

**Measurement limits:** support decoding currently covers eight recognized healing families and five named shield families. Effective healing and overheal are not determined. Automated packet, identity and UI checks do not establish complete live-game or regional protocol coverage; real comparisons by users remain necessary.

The existing features stay available: independent live overlay, party DPS returning to zero after 2 seconds without positive received damage, cumulative run damage, direct history analysis with contribution bars and Back navigation, full skill/hit details, saved builds, comparisons, Rift/event timers and optional favourite-boss alerts. Internal dungeon teleports preserve runs; 22 activity entries are recognized, with automatic final-boss completion limited to 7 dungeons. Startup stays silent.

**Install or update:** download **Eclipse-Setup.exe**, or use **UPDATE** when it appears in Eclipse. Runtime is included; the official Npcap consent wizard is offered if its driver is missing. Existing history, language and HUD preferences are preserved. English is the default; French is selectable. No Eclipse account is required.

Validation: 577 logic checks including synchronized and fragmented TCP, LZ4 compressed batches and all nine local classes; 14 native support checks, 22 history-analysis checks, English/French/compact support views, isolated lifecycle, V1/2.1.10 migrations and standalone setup verification. Gallery values are fictional demo data.

## v2.1.10 — Direct run analysis and overlay fixes

Eclipse 2.1.10 makes reviewing a dungeon run faster and fixes overlay and client closure.

- Click a dungeon in **Run history** to open its analysis directly.
- See **every party member's total damage**, sorted by contribution, with a thin class-coloured bar. Players who left the party remain in the saved run.
- Keep the existing skill breakdown, hits and timeline underneath. Time-range selection changes the details while the recap keeps the whole run's totals.
- **Back to run history** restores your search, filters and scroll position; the same run can be opened again.
- Closing the **overlay** leaves the desktop client and damage capture running. Use the Overlay button to reopen it.
- Closing the **main client** hides both windows promptly, finishes pending saves and stops capture before exiting.

The 2.1.9 DPS and dungeon corrections are included: live party DPS returns to zero after 2 seconds without received positive damage, while run totals remain cumulative. Internal teleports preserve runs. Activity recognition covers 22 catalogue entries; automatic final-boss completion remains limited to 7 dungeons.

**Install:** download **Eclipse-Setup.exe**, or click **UPDATE** when it appears in Eclipse. The complete application runtime is included; the official Npcap consent wizard is offered if the driver is missing. Existing history, language and HUD settings are preserved. English is the default; French is selectable. Startup remains silent.

Validation: 500 logic checks, 22 native history-analysis checks, English/French and compact layouts, both client close paths with an existing Npcap driver and isolated local API, migrations from V1 and 2.1.9, and standalone payload verification. Gallery values are labelled demo data. This release does not extend dungeon or regional protocol coverage.

## v2.1.9 — DPS and dungeon-run corrective update

Eclipse 2.1.9 is a corrective update to V2.

- Live party DPS returns to **0 after 2 seconds without received positive party damage**. The next hit starts a fresh DPS window; run totals and archived averages are retained.
- Internal dungeon teleports preserve the same run. Supported final-boss deaths archive its last hits and reset live totals. Interrupted runs retain their summary.
- Fix the permanent no-DPS state after a closed run and a later world load into an activity missing from the catalogue. Unknown combat remains measurable without claiming dungeon recognition.
- Protect old targets from late hits; handle reused player/target IDs and delayed NPC identity.
- Recognize 22 catalogue activities, including three sealed dungeons and Flauke Legion Outpost. Automatic completion is limited to verified final bosses in seven dungeons; other finishes use **Finish run / Interrupt run**.

**Install:** download **Eclipse-Setup.exe** below, or click **UPDATE** in your current installation. The standalone EXE includes the complete application; guided Npcap consent remains available if needed. Existing language, HUD settings and history are preserved. English is the default; French remains selectable. The app intro is silent.

Validation: 500 logic checks, native Windows interface and update controls, ZIP migrations from V1 and 2.1.8, standalone extraction/install verification. The owner confirmed the original no-DPS fix in game. The two-second cutoff is verified with timed fixtures; complete coverage of every dungeon/region is not claimed.

## v2.1.8 — Live official website and bug report link

- Direct Eclipse-Setup.exe download: complete application payload embedded and SHA-256 checked before extraction. No manual ZIP extraction; guided Npcap consent retained. Standalone installation verified in an isolated folder.
- Report a bug opens the published production website with the installed version. Updated README links and screenshots to 2.1.8.
- Conditional UPDATE, real download progress, regional schedules, favourite reminders and silent app intro retained.
- Website presentation uses one gallery with distinct client views and tighter section spacing.

Validation: 436 logic checks, native UI, final ZIP migrations from V1 and 2.1.7, 424 original files unchanged. The private report table is accessible only through the owner's Sites account.

## v2.1.7 — Corrected regional schedules, conditional UPDATE and official website

- AION2Hub replaces the former timer sources. Global EU/NA/SA/JP and Korea use fixed UTC+9, Taiwan UTC+8. Region-specific Rift openings convert to the device timezone without following US DST.
- Travel Rift entry/lifetime is unspecified by the new source. Removed the unconfirmed five-minute entry and one-hour activity phases; show the server clock and next opening instead.
- Corrected regional Kaira intervals, executor weekdays, Abyss Event, siege bosses and KR/TW-only activities. Removed unsupported matchmaking offsets. Each card links to its dated community source.
- Boss favourite keys, Rift selection, language and reminder timing are preserved. Alert delivery IDs include the service; former-source receipts do not suppress corrected openings.
- UPDATE appears in the full client only when a newer release is detected, matching the overlay. A glass progress panel shows the real download percentage and animated verification/preparation phases. Report a bug opens the new official website form with the installed version.
- Version 2.1.7 replaces the current BETA labels in client, overlay, intro and promotional screenshots. This branding change does not guarantee every future regional protocol.
- English/French website, native English screenshots, optional original ambient music, guided download and private persistent bug reports with JSON export. No automatic player-log upload.

Validation: 436 logic checks, native regional/FR/EN/reminder/update/close checks, final ZIP migrations from V1 and 2.1.6, 424 original files unchanged. Website form persistence, JSON download, language and mobile layout checked locally.

## v2.1.6 — Rift entry and event timers

The schedules and portal durations in this historical release were superseded by the corrected 2.1.7 source below.

- Dedicated Rift panel at the top of Rifts & events, with waiting, scheduled portal-open and event-active/entry-closed phases.
- Separate five-minute entry and one-hour event clocks, progress bars and next four local/UTC openings.
- Dated Talentbuilds regional reference for EU, NA, SA, JP, TW and KR, using the site’s America/New_York clock including DST and the TW one-hour difference.
- Independent favourite reminders at 10 minutes before, 5 minutes before or opening; saved region and timing, minimized operation, restart deduplication and no missed-alert replay after sleep.
- English default and translated French controls. Existing boss schedules, language choices and preferences are retained; new Rift alerts start disabled.
- Source and verification date visible. Talentbuilds’s five-minute entry differs from the separate 6sword KR reference; neither source is presented as live portal detection or a confirmed global schedule.

Validation: 432 logic checks, native Rift phases and FR/EN/regional control checks, favourite audio timings and minimized notification checks. Actual ZIP migration verified from copied V1 and 2.1.5 installations with existing data preserved.

## v2.1.5 — Eclipse V2 BETA, the main update

V2 replaces V1 on the official download and update channel. This is the full Glass client release for existing Eclipse users and new installations.

- Native Glass desktop client with animated AION artwork, movable/resizable window and second-monitor use.
- Entirely silent Eclipse logo/loading intro. English by default; French remains selectable.
- Overlay enabled on first launch, sharing the client's live party data.
- Party DPS, observed damage, received levels, skill breakdowns, critical/back attacks and received deaths.
- Teleport-driven run boundaries: reset totals and DPS, archive the previous run including hits received before the last UI refresh, preserve party identity and levels, reject stale old-world damage and duplicate identity bursts. Other teleports also reset; exhaustive dungeon names are not inferred.
- Expedition summary, target segments, timeline range analysis, burst windows, run history, notes, favourites, interrupted-run recovery and retention controls.
- Personal build snapshots, contextual MetaRoad tier lists, dated community build links, local ranking and compatible-run A/B comparisons.
- Dated Korean boss/event calendar, local-time conversion and matchmaking groups. Other regions remain pending official schedules.
- Favourite reminders at 10 minutes before, 5 minutes before or the scheduled instant; enabled reminders continue while minimized and are deduplicated. No intro or navigation sound.
- Exports, share cards, restricted diagnostics, transparency and performance controls; visual effects stop while minimized.
- Guided setup with included runtime and official Npcap consent wizard when needed.
- Same Aion2-Eclipse.exe identity and public update manifest as V1; update engine preserves installed data. UPDATE is available in both the full client and HUD.
- Complete shutdown through the client close button or window close.

Validation: 397 logic checks; native seven-page Windows UI checks including FR/EN, silent intro, overlay startup and all three boss reminder timings. The actual public ZIP was installed by the update engine over a copied v1.0.30 executable and validated by the setup engine in isolated folders. Original production files were retained. Live capture compatibility for every region and exact dungeon names remain BETA limitations.

[Download V2 BETA](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest). If an old V1 updater loops, extract the latest ZIP and run Eclipse.Setup.exe once.

## v1.0.30 — Update recovery and complete shutdown (superseded)

- Fixed UPDATE reopening an older executable after access-denied errors, with retries, rollback and installed-version checks.
- Used the verified release ZIP's updater and readiness handshake.
- Fixed background processes after closing Eclipse; capture and history cleanup were bounded.
- Setup recovered invisible older instances.

Validation reported for V1: 254 checks. [Historical release](https://github.com/Iota-Nine/Aion2-Eclipse/releases/tag/v1.0.30).
