# Eclipse release notes

## v3.0.9 - Clearer timers, favourites and alerts

Eclipse 3.0.9 makes boss timers easier to use, with favourites and alarms together in one clear view.

- Favourites & alerts opens first in Boss & timers. Compact rows put the boss name, received countdown, star and bell together; search finds a boss quickly.
- Star and bell are independent. Keep a favourite without any sound, or enable its alarm. Removing the bell keeps the favourite and stops that boss's active ringing without silencing another alarm.
- One filter: All followed bosses, Active alarms, Favourites without alarms, All bosses. Your selected filter, favourites and alarm choices are saved.
- Each user's timers come from their own received game packets and automatically detected EU server. Open Map → Exploration → Field monsters to sync; reopen that game list for changed times/status. No shared kill feed or fixed Israphel schedule. Missing times/channels are not guessed.
- Rifts/calendar and Combat timers have separate views. Options & details stay collapsed until needed. The sidebar and lists fit smaller windows without cutting off navigation.
- Existing enabled field-boss alarms migrate automatically. Observed timestamps, acknowledged reminders, history, Progression and preferences stay saved. The 10-minute, 5-minute and scheduled-time choices, bell until STOP, HUD shortcuts and original combat analysis stay available.
- English and French. English remains the initial language.

Validation: 1006 native Windows checks across 28 suites, 1534 logic checks, exact ZIP and embedded setup, isolated V1/3.0.8 upgrades and offline shutdown. Screenshots and fixtures use fictional demo data; this does not prove universal live-game coverage. Received boss times require refreshing the game list for changes. The separate regional calendar remains a community prediction with clock confirmation for European boss alerts.

FR : Une vue Favoris & alertes plus claire, avec recherche, étoile et cloche indépendantes. Filtres : tous mes suivis, alarmes actives, favoris sans alarme, tous les boss. Retirer une cloche garde le favori et arrête uniquement sa sonnerie. Les horaires proviennent des paquets reçus dans le jeu de chaque utilisateur et restent distincts par serveur EU détecté. Ouvrir Carte → Exploration → Monstres de terrain pour synchroniser, puis rouvrir cette liste pour recevoir les changements. Failles/calendrier et chronos de combat ont leur propre onglet. Anciennes alarmes, historique, progression et réglages conservés.


## v3.0.8 - Adaptive HUD, V3 guide and boss reminders

Eclipse 3.0.8 makes the overlay easier to read and adds a V3 quick-start guide, a simpler reset shortcut and controllable boss reminders.

- Compact Focus HUD: real class icons, thin damage bars and healing next to each received player. Row height, names and icons adapt to the observed roster; scroll to reach every received member. Existing full, fold, click-through, shields and support details stay available.
- Alt+R saves the current run as interrupted before clearing counters. History stays saved. Alt+F8 and Ctrl+Alt+L keep their usual actions.
- Silent Eclipse V3 opening and a shortcut guide. Close keeps the guide for next launch; Don't show again remembers your choice. Reopen it in Preferences.
- A soft boss/Rift bell repeats every three seconds until STOP in the client or HUD. The small STOP control also works in the folded, click-through HUD. Alerts retain 10-minute, 5-minute and scheduled-time choices.
- Automatic EU field-boss timers: open Map → Exploration → Field monsters once. Eclipse identifies your local server and reads the times sent in that list without manual entry. Reopen the game list for changed times/status. Timers and alert choices stay separate by server, including Israphel. Unknown times and untransmitted channels are not invented; unresolved boss names remain numbered slots. Altgard includes Deceiver Trid. This is passive game data, not a shared global live feed.
- A world-boss-only calendar filter, source links and an optional European clock reference. Community sources disagree about the Global clock: compare predicted times with the game and explicitly confirm the chosen clock before EU Abyss-boss alarms are enabled. Changing it clears that confirmation. Field bosses such as Deceiver Trid use their individual observed time rather than this regional calendar.
- English and French, Progression, DPS/healing/shield/buff analysis, history and settings remain available. No sound during the introduction.

Validation: 889 native Windows checks across 26 suites, logic regression checks, exact ZIP/embedded setup, isolated V1/3.0.7 upgrades and offline shutdown. Screenshots and packet fixtures use fictional demo data. Observed large rosters do not prove every live Force packet format. Shield capacity, absorption and destruction remain unknown.

FR : HUD compact adaptatif avec icônes de classe et soins par joueur, Alt+R avec conservation du run interrompu, accueil V3 et guide des raccourcis. Cloche répétée toutes les trois secondes jusqu’à STOP sur le client ou le HUD. Timers de boss de terrain récupérés automatiquement depuis la liste du jeu, distincts par serveur EU. Ouvrir Carte → Exploration → Monstres de terrain pour synchroniser, puis Eclipse poursuit les comptes à rebours. Les prévisions communautaires des Abysses demandent de vérifier l’horloge ; aucun canal ou horaire manquant n’est inventé. Historique, progression et réglages conservés.

Schedule reference: https://aion2hub.com/tools/world-bosses . Passive field-boss protocol reference: https://github.com/cyberbadger6969/aion2-dps-meter#field-boss-respawn-timers . The map packet supplies timestamps; a published cycle alone cannot identify a current server spawn.


## v3.0.7 - Progression and a clearer client

Eclipse 3.0.7 adds Progression to the client: keep your daily activities, weekly checklist and long-term goals together, with a separate list for each character.

- Tick completed activities, add personal objectives or counters, and hide completed tasks. The compact layout uses shorter labels and removes repeated instructions.
- Recognized dungeon victories can complete the dungeon objective automatically when Eclipse has the matching character and server identity. Other activities are manual reminders, not official reward quotas. Teleports, interrupted runs and manual finishes never imply victory.
- Keep permanent goals across resets and enter your own Gear Score target. Gear Score is a manual value, separate from received party Combat Power.
- Choose the reset time zone, hour and weekly day. Automatic resets stay off until you check the schedule against the game and confirm it. An optional visual reminder appears ten minutes before the daily reset.
- Progression saves locally in the background with a previous backup. Burst edits are grouped, lists do not rebuild on idle ticks, and startup archive reconciliation saves once. Known characters still update when the profile limit is reached.
- English is default, French is available, including reset weekday names. Run history, settings, HUD shortcuts and existing damage/healing/shield/buff measurements are retained.

Getting started: update Eclipse, open Progression, choose your character and tick your finished activities. Use Set reset schedule only after comparing the settings with your game. No account is required.

Validation: 870 logic checks, 420 native Windows interface checks in 17 suites, isolated upgrades from V1 and 3.0.6, saved-progression preservation, embedded setup and offline shutdown checks. Interface/packet fixtures are fictional, not universal live-game dungeon coverage. The existing selected-skill support measurement limits remain unchanged.

FR : nouvel onglet Progression avec checklist quotidienne et hebdomadaire par personnage, objectifs personnels, compteur et Gear Score manuel. Interface plus concise et filtre pour masquer les tâches terminées. Les victoires de donjons reconnues et identifiées se valident automatiquement ; les autres activités restent manuelles. Horaires de reset configurables et désactivés jusqu’à votre confirmation dans le jeu. Rappel visuel facultatif, sauvegarde locale en arrière-plan, historique et réglages conservés.

Checklist inspiration: https://guidemmo.com/checklist-aion-2/ . These are concise personal reminders, not official reward limits or a universal server reset schedule.


## v3.0.6 — Shields and support buffs

Eclipse 3.0.6 expands support analysis in the original compact and full HUD, and retains your local runs and preferences on update.

- Improved detection of selected shield skills across Templar, Cleric, Chanter, Sorcerer, Ranger and Spiritmaster, including verified self effects and specialization requirements.
- Blue shield bars show observed activations and received duration ranges. Skill and recipient details are retained in new run histories. Companion notices and near-simultaneous group applications are grouped.
- New violet support-buff bars for selected Cleric and Chanter skills: Light of Protection, Yustiel’s Power, Prayer of Amplification, Sprint Mantra, Undefeated Mantra, Power of the Storm, Guardian Blessing and Barrier Spell. Analysis lists casters, skills and recipients.
- Repeated overlapping aura/mantra refreshes form one observed sequence instead of inflating activation counts. Selected pre-combat support still active by its received lifetime is retained at the first accepted damage event.
- Self healing, shields and buffs remain optional and off by default. Existing healing totals are not counted twice. English is default; French is available in Preferences.
- DPS, run totals, party Combat Power, original HUD controls, Alt+F8, Ctrl+Alt+L, collapse/restore and return after Alt+Tab are retained.

Measurement limits: durations are received lifetimes, not measured active uptime or a shield-destruction countdown. Shield HP capacity, absorbed damage, destruction, buff potency and damage gained are not measured. Selected skills and identified party data only; unavailable metrics stay hidden. Old runs do not invent missing support details.

Validation: 812 logic checks, 390 native Windows interface checks across 16 suites, isolated upgrades from V1 and 3.0.5, standalone setup and shutdown checks. Packet/interface fixtures are fictional; these checks do not establish universal live-game skill coverage.

FR — Détection de boucliers améliorée sur six classes, activations observées et durées reçues. Buffs sélectionnés du Cleric et de l’aède, barres violettes et détails par compétence/destinataire dans l’analyse. Les rafraîchissements de mantras sont regroupés. Détail sur soi en option ; historique et réglages conservés. Les durées ne mesurent pas l’uptime réel. PV des boucliers, absorption, destruction et gain de dégâts des buffs restent inconnus.


## v3.0.5 — HUD support, Combat Power and skill icons

Eclipse 3.0.5 corrects missing skill icons and adds optional self-support details and party Combat Power to the compact and full HUD.

- 97 missing skill icons added, including Murderous Burst and Destructive Impulse. Known skill variants use their matching base icon.
- Preferences → HUD DISPLAY → Show self healing and self shields (off by default). The separate self-healing detail is already included in the healing total and is not added twice. Shields show recognized applications; capacity and absorbed damage are unknown.
- Show party Combat Power (on by default, optional). Group values are matched to the player's identity and server. Missing CP is shown as “—”.
- Existing damage totals, run history, preferences, Alt+F8, click-through, collapse/restore and return after Alt+Tab are retained. English remains the default; French is available in Preferences.

Validation: 637 logic checks, complete native Windows interface checks, isolated upgrades from V1 and 3.0.4, standalone setup and shutdown. The interface and packet checks use fictional fixtures. CP and all self-support skill coverage still need live-game tester comparison; self support uses the existing recognized skills. This update adds no exclusive-fullscreen renderer.

FR — 97 icônes manquantes corrigées, soins/boucliers sur soi en option et CP du groupe dans le HUD compact/complet. Aucun double comptage des soins. Boucliers = applications reconnues, sans capacité ou absorption mesurée. CP absent : —. Historique, réglages et raccourcis conservés. Les tests locaux passent ; la comparaison des nouvelles valeurs en jeu reste à faire.


## v3.0.4 — HUD return after Alt+Tab

Eclipse 3.0.4 improves HUD visibility when returning to AION 2 after **Alt+Tab**.

- A visible HUD is automatically brought back above the game window, without taking keyboard focus or moving/resizing it. No need to toggle Alt+F8 just to restore its order.
- A HUD deliberately hidden with **Alt+F8** or **Ctrl+Alt+H**, or closed with ×, stays hidden. Alt+F8 remains available to reopen it.
- Compact/full, folded header, click-through, live damage/healing/allied-shield counters, run history and settings are retained. This update does not reset the current run when game focus changes.
- **UPDATE** is available from 3.0.3 and older. The installed 3.0.4 does not offer the same update again.

**Download Eclipse-Setup.exe below** for the complete application and runtime. English is default; French is selectable. Missing Npcap is offered through its official consent wizard.

Validation: 615 logic checks, 44 native Windows foreground/order checks, live-engine HUD and existing interface checks, six previous-version migration paths, standalone setup and shutdown verification. Gallery combat values are fictional. Live-game visual Alt+Tab confirmation has not been explicitly recorded; native fixtures do not establish exclusive-fullscreen compatibility. This correction uses the existing Windows HUD.

---

**Français** — La 3.0.4 remet automatiquement un HUD visible devant la fenêtre d'AION 2 au retour après **Alt+Tab**, sans prendre le focus clavier ni changer sa taille ou sa position. Un masquage volontaire reste respecté ; **Alt+F8** permet toujours d'afficher ou de rouvrir le HUD. Modes compact/complet, en-tête replié, clics, mesures, historique et réglages conservés. **UPDATE** proposé depuis la 3.0.3 et les versions précédentes.


## v3.0.3 — Live HUD and Alt+F8

Eclipse 3.0.3 connects the original transparent HUD directly to the client's combat engine and adds **Alt+F8**.

- **Alt+F8** shows or hides the HUD automatically once Eclipse is running. It works with the desktop client minimized and can reopen an overlay closed with ×. Showing the HUD does not activate it over the game. If another app owns Alt+F8, the client reports the conflict and its HUD button stays available.
- The production overlay reads the same in-process damage, party identity, healing and allied-shield counters as the client. It requires no separate preview helper or API connection. Reset refreshes the displayed counters immediately.
- The original appearance and controls remain: compact/full, header fold, move, click-through with **Ctrl+Alt+L**, **Ctrl+Alt+H**, **Ctrl+Alt+R**, Build, and UPDATE only when an update is detected.
- Live DPS returns to zero after 2 seconds without positive damage; cumulative run damage and received support totals remain. Existing dungeon, history, build, timer and language features are retained.
- **UPDATE** is available from 3.0.2 and older. History and settings are preserved; the installed 3.0.3 does not repeatedly ask for the same update.

**Download:** **Eclipse-Setup.exe** below includes the application and runtime. English is default; French is selectable. If Npcap is missing, its official consent wizard is offered.

Compatibility: this release uses the standard Windows overlay. It does not integrate into Steam or add exclusive-fullscreen rendering. Shield values still describe observed allied applications; capacity and absorbed damage remain unknown.

Validation: 615 logic checks; native damage/healing/shield display and Alt+F8 lifecycle checks; existing compact/full EN/FR, fold, mouse shortcut, history, analysis and update UI checks; isolated shutdown; ZIP upgrades from V1, 3.0.0, both 3.0.1 builds and 3.0.2; standalone setup verification. Combat fixtures and gallery values are fictional. These checks do not replace exhaustive live-game protocol validation.

![Eclipse compact overlay — English, fictional demo encounter](https://raw.githubusercontent.com/Iota-Nine/Aion2-Eclipse/main/docs/images/eclipse-hud-support-compact-en.png)

---

**Français** — La 3.0.3 relie directement le HUD original au moteur de combat du client et ajoute **Alt+F8** pour afficher/masquer l'overlay, même lorsque le client est réduit, ou le rouvrir après ×. Les compteurs se rafraîchissent après RESET. Apparence, fonctions, historique et réglages conservés. UPDATE proposé depuis la 3.0.2 et les versions précédentes. Cette version conserve l'overlay Windows habituel ; l'intégration Steam et le plein écran exclusif restent hors de cette release. Les boucliers restent un nombre d'applications observées, sans capacité en PV ni absorption inventée.


## v3.0.2 — Overlay fold update

Eclipse 3.0.2 delivers the overlay fold correction through **UPDATE**, including for users already on 3.0.1.

- Press **−** to fold the overlay to its visible, draggable header. Press **+** to restore the meter.
- Compact/full mode, width and position are retained. Live measurements and cumulative damage, healing and allied-shield application counts continue while folded.
- **UPDATE** appears in both the client and overlay when the new version is detected. Installing 3.0.2 clears the prompt; existing run history, language and HUD settings are preserved.
- The existing healing/HPS and allied-shield bars remain available in compact and full modes. Shield capacity and absorbed damage are still unknown.

**Install/update:** use **UPDATE** when it appears, or download **Eclipse-Setup.exe** below. English is the default; French is selectable. Runtime is included. The official Npcap consent wizard is offered if the driver is missing. No manual reinstallation is required just because you have 3.0.1.

Validation: 615 logic checks, 56 native fold checks in English/French and compact/full modes, existing support/shortcut/history/analysis checks, isolated shutdown, final ZIP upgrades from V1, 3.0.0 and both 3.0.1 builds, plus standalone setup verification. Screenshots use fictional demo data; automated UI checks are not an exhaustive live-game protocol test.

![Folded Eclipse overlay — English, fictional demo encounter](https://raw.githubusercontent.com/Iota-Nine/Aion2-Eclipse/main/docs/images/eclipse-hud-folded-en.png)

---

**Français** — La 3.0.2 rend le correctif du repli disponible via **UPDATE**, y compris depuis la 3.0.1. **−** conserve l'en-tête visible et déplaçable ; **+** réaffiche les compteurs. Les mesures continuent, le format compact/complet et la position sont conservés. Historique et réglages préservés. Mise à jour depuis le client ou l'overlay, ou via **Eclipse-Setup.exe**. Les limites de mesure des boucliers restent inchangées.


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
