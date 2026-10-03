# Eclipse release notes

## v2.1.8 — Live official website and bug report link

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
