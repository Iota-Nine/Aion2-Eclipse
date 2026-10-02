# Eclipse release notes

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
