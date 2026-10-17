# Eclipse release notes

## 3.0.26 — 17 October 2026


## English
You reported through a bug report that DPS returned to zero as soon as combat ended. Average DPS now stays visible so you can review the fight. Thank you for the feedback.

- Personal, party and player averages use the same cumulative damage measurement since reset. Idle time after the last hit and zero-damage events do not lower the displayed average.
- Added a small Alt+R reminder beside Ctrl+Alt+L in the full and compact HUD, with an explanatory tooltip and a warning if the shortcut is already in use.
- Press Alt+R before starting a new measurement. Without a reset, the next fight continues the cumulative measurement, including the interval between fights.
- Complete run archives, replays, saved preferences and existing features are retained.

Use UPDATE when offered, or download Eclipse-Setup.exe.

## Français
Vous nous avez signalé via un rapport de bug que le DPS revenait à zéro dès la fin du combat. Le DPS moyen reste désormais visible pour vous permettre de consulter votre résultat. Merci pour ce retour.

- Les moyennes personnelles, du groupe et de chaque joueur utilisent les mêmes dégâts cumulés depuis le reset. L’attente après le dernier impact et les événements sans dégâts ne font plus baisser la moyenne affichée.
- Ajout d’un petit rappel Alt+R à côté de Ctrl+Alt+L dans les HUD complet et compact, avec une infobulle et une indication si le raccourci est déjà occupé.
- Appuyez sur Alt+R avant une nouvelle mesure. Sans reset, le combat suivant prolonge la mesure cumulée, en incluant l’intervalle entre les combats.
- Archives complètes des runs, replays, préférences et fonctions existantes conservés.

Utilisez UPDATE lorsqu’il est proposé, ou téléchargez Eclipse-Setup.exe.

## 3.0.25 — 16 October 2026


## English
You reported through a bug report that some buttons in the Eclipse client did not show an explanation when hovered. Thank you for pointing it out: this is now patched.

- Added missing hover descriptions across client controls, navigation, progression and relevant HUD actions.
- Made tooltips easier to read with a dark background, contrasting wrapped text and a short hover delay. Descriptions follow your English/French language setting.
- Improved Alt+R responsiveness: counters reset promptly while the complete previous run is archived in the background.
- Optimized network packet processing, loading of history and visual assets, and combat analysis. Full replay data and saved preferences are retained.

Use UPDATE when offered, or download Eclipse-Setup.exe. Your reports help us improve Eclipse.

## Français
Vous nous avez signalé via un rapport de bug que certains boutons du client Eclipse n’affichaient pas d’explication au survol. Merci pour ce retour : ce problème est maintenant corrigé.

- Ajout des infobulles manquantes sur les commandes du client, la navigation, la progression et les actions concernées du HUD.
- Infobulles plus lisibles : fond sombre, texte contrasté avec retour à la ligne et court délai au survol. Les descriptions suivent votre choix de langue français/anglais.
- Alt+R plus réactif : les compteurs se réinitialisent rapidement pendant que le run précédent complet est enregistré en arrière-plan.
- Optimisation du traitement des paquets réseau, du chargement de l’historique et des images, et de l’analyse des combats. Les replays complets et préférences restent conservés.

Utilisez UPDATE lorsqu’il est proposé, ou téléchargez Eclipse-Setup.exe. Vos rapports nous aident à améliorer Eclipse.

## 3.0.24 — 16 October 2026


## English
- Fixed an interruption that could keep an outdated class displayed, including Ranger shown as Spiritmaster.
- Empty, unknown or expired cooldown updates no longer discard earlier valid class observations. They do not count as a skill or extend the thirty-second evidence window.
- Two distinct, concordant local active skills after fresh character identification remain necessary to correct a known wrong class. Conflicting, stale, incomplete and different-character data still cannot confirm a correction.
- The corrected name and icon reach the client and HUD and are saved without resetting damage, the party or the current run. Clearing the identity cache is not required for this corrected path.
- Existing compact HUD, class-colored total-damage bars, readable CP, boss HP availability, status, history, timers, alarm volume/STOP and preferences are preserved.

## Français
- Correction d’un blocage pouvant conserver une ancienne classe, notamment Ranger affiché Spiritmaster.
- Les actualisations de délais vides, inconnues ou expirées n’effacent plus les observations valides précédentes. Elles ne comptent pas comme une compétence et ne prolongent pas la fenêtre de trente secondes.
- Deux compétences locales actives, distinctes et concordantes après une identification récente restent nécessaires pour corriger une classe connue erronée. Les données contradictoires, anciennes, incomplètes ou d’un autre personnage ne confirment aucune correction.
- Nom et icône corrigés dans le client et le HUD, avec sauvegarde de la classe sans reset des dégâts, du groupe ou du run. Ce chemin corrigé ne nécessite pas de vider le cache d’identité.
- HUD compact, barres de dégâts totaux aux couleurs des classes, CP lisibles, PV de boss disponibles, statut, historique, timers, volume/STOP et préférences conservés.

This corrects a reproduced code path; it does not confirm resolution of every individual player report or every regional packet format.

Use UPDATE when offered, or download Eclipse-Setup.exe. Utilisez UPDATE lorsqu’il est proposé, ou téléchargez Eclipse-Setup.exe.

## 3.0.23 — 16 October 2026

### English
- Redesigned party HUD with existing class colors and bars proportional to total damage. Live DPS remains a separate value.
- More transparent compact surfaces and bars, high-contrast text with a subtle shadow and larger CP. Ctrl+Alt+L click-through lock and the saved HUD position remain available.
- Health section reserved for recognised bosses, excluding training dummies; hitting an add keeps the boss selected for this section.
- Corrected decoding of received HP fields. Percentages require current HP and a consistent received maximum; missing, stale or inconsistent data is labelled without an assumed percentage.
- Status message scrolls in the client header; click for a complete anchored message bubble instead of a modal dialog.
- Preserves existing combat, healing, history, timers, alarm volume, preferences and updates.

### Français
- HUD du groupe remanié : couleurs des classes conservées et barres proportionnelles aux dégâts totaux. Le DPS reste une valeur séparée.
- Fonds et barres du compact plus transparents, texte contrasté avec ombre discrète et CP agrandis. Verrouillage des clics Ctrl+Alt+L et position enregistrée conservés.
- Section de vie réservée aux boss reconnus, hors mannequins ; frapper un monstre secondaire conserve le boss dans cette section.
- Lecture corrigée des champs de PV reçus. Le pourcentage nécessite des PV actuels et un maximum reçu cohérent ; les données manquantes, anciennes ou incohérentes sont signalées sans pourcentage supposé.
- Statut défilant dans l’en-tête du client ; un clic affiche le message complet dans une bulle ancrée.
- Combat, soins, historique, timers, volume des alarmes, préférences et mises à jour conservés.

Available HP fields and boss recognition depend on the received game data; this release does not establish universal regional compatibility or confirm resolution of an individual player report.

## v3.0.22 - Live status and verified repairs

- Live creator announcements in the client: normal, orange or red, with a dated last message when the status service is unavailable. Public status can be changed by the creator without a client release.
- Cleric Benevolence is classified as healing without adding that healing to DPS.
- Received ally damage is retained across a confirmed departure and return, including between interface refreshes.
- Invalid local history fields are recovered while keeping valid data and an original-file backup.
- Combat duration, charts and boundaries use elapsed instants across daylight saving changes.
- Updates reject ambiguous Windows paths that could bypass local data protection.
- Existing timers, alarm volume/STOP, WAIT, pinned patch notes, class corrections, history, progression and preferences are retained.

Français

- Statut du créateur en direct dans le client : normal, orange ou rouge, avec le dernier message daté si le service est indisponible. Le créateur peut changer le statut sans republier l’application.
- Benevolence du clerc est comptabilisé dans les soins sans ajouter ce soin au DPS.
- Les dégâts reçus d’un allié restent conservés quand il quitte puis revient, même entre deux actualisations de l’interface.
- Les champs invalides de l’historique local sont récupérés en gardant les données valides et une copie du fichier original.
- Durées, courbes et limites des combats restent cohérentes lors d’un changement d’heure.
- La mise à jour rejette les chemins Windows ambigus contournant la protection des données locales.
- Timers, volume/STOP, WAIT, notes fixes, corrections de classe, historique, progression et réglages conservés.

Use UPDATE when offered, or download Eclipse-Setup.exe. Utilisez UPDATE lorsqu’il est proposé, ou téléchargez Eclipse-Setup.exe.

## v3.0.21 - Keep your party and dungeon damage

- Partial, empty or transitional party updates retain known allies until a complete update or confirmed leave is received.
- Old party and character messages cannot replace newer identity information. Name capitalization changes preserve the same character and counters.
- Late boss identification enriches the current run instead of resetting its damage. Numbered boss copies in the same dungeon mode stay in the same run.
- Confirmed party leaves still clear the party without erasing personal damage. Real character changes, real run boundaries and manual reset retain their behavior.
- Existing class corrections, alarm volume/STOP, WAIT, pinned patch notes, history, progression and EN/FR controls are retained.

Français

- Les mises à jour incomplètes, vides ou transitoires conservent les alliés connus jusqu’à une liste complète ou une sortie confirmée.
- Les anciens messages du groupe et du personnage ne remplacent plus une identité récente. Un changement de casse du pseudo conserve le personnage et ses compteurs.
- Un boss identifié tardivement enrichit le run en cours sans remettre ses dégâts à zéro. Les copies numérotées d’un boss du même mode restent dans le même run.
- Une sortie confirmée vide toujours le groupe sans effacer les dégâts personnels. Changements réels de personnage, véritables fins de run et reset manuel conservent leurs comportements.
- Corrections de classe, volume/STOP, WAIT, notes fixes, historique, progression et interface FR/EN conservés.

Use UPDATE when offered, or download Eclipse-Setup.exe. Utilisez UPDATE lorsqu’il est proposé, ou téléchargez Eclipse-Setup.exe.

## v3.0.20 - Correct character class

- Fixed PlayerInfo class decoding: the job code follows both server bytes. A server byte is no longer mistaken for Assassin or another playable class on unlisted servers.
- A stale known local class can now be corrected by two distinct, recognized active skill cooldowns from the same class within 30 seconds, after fresh local identification.
- Replayed skills, mixed classes, incomplete batches, zero durations, stale timestamps and changed identities cannot confirm a class correction.
- Corrected class names and icons reach the party row, client, HUD and saved preferences without resetting damage or the current run. Noisy teleport job bytes cannot undo the correction.
- All existing boss timers, alarm volume/STOP, WAIT, pinned patch notes, history, progression and EN/FR controls are retained.

Français

- Correction de la lecture de la classe dans PlayerInfo : le code suit les deux octets du serveur. Un octet de serveur n’est plus confondu avec Assassin ou une autre classe sur les serveurs absents de l’ancien catalogue.
- Une ancienne classe locale erronée peut désormais être corrigée par deux compétences actives distinctes, reconnues et concordantes, observées en moins de 30 secondes après une identification locale reçue du jeu.
- Les compétences répétées, classes mélangées, trames incomplètes, durées nulles, données anciennes et changements d’identité ne confirment pas de correction.
- Nom et icône actualisés dans le groupe, le client, le HUD et les préférences enregistrées, sans remise à zéro des dégâts ou du run. Un code incohérent lors d’une téléportation ne défait pas la correction.
- Timers de boss, volume/STOP, WAIT, notes fixes, historique, progression et interface FR/EN conservés.

Use UPDATE when offered, or download Eclipse-Setup.exe. Utilisez UPDATE lorsqu’il est proposé, ou téléchargez Eclipse-Setup.exe.

## v3.0.19 - Field-boss sync across servers

- Removed the EU-only restriction from received field-boss lists, saved maps, catalog favourites and alarms. Tracking uses the exact positive server ID received from the game.
- Timer identity now uses the same name boundary and encoding decoder as the DPS meter, including supported Asian UTF-16 names, terminated strings and unflagged name lengths.
- A delayed old map list cannot acquire a newly switched server identity, even when the connection is reused.
- Game timestamps remain unchanged; each server keeps separate favourites, alarms and receipts. Unknown names and times remain unknown.
- EN/FR, capture, damage/healing/support, history, progression, saved alarm volume, STOP, WAIT, pinned patch notes and HUD shortcuts are preserved.

Français

- Retrait de la restriction aux serveurs européens pour les listes de boss reçues du jeu, les cartes enregistrées, les favoris du catalogue et les alarmes. Le suivi utilise l’identifiant exact du serveur transmis par le jeu.
- Les timers utilisent désormais le même décodage des pseudos que le DPS, y compris les noms asiatiques UTF-16 pris en charge, les chaînes terminées et les variantes de longueur sans indicateur.
- Une ancienne liste reçue en retard ne peut plus être attribuée au nouveau serveur après un changement d’identité, même si la connexion est réutilisée.
- Les horaires du jeu restent inchangés ; favoris, alarmes et reçus restent séparés par serveur. Les noms et horaires inconnus restent inconnus.
- Français/anglais, capture, dégâts/soins/support, historique, progression, volume enregistré, STOP, WAIT, notes fixes et raccourcis du HUD conservés.

Use UPDATE when offered, or download Eclipse-Setup.exe. Utilisez UPDATE lorsqu’il est proposé, ou téléchargez Eclipse-Setup.exe.

## v3.0.18 - Adjustable alarm volume

- Set alarm volume from 0 to 100% directly in Preferences, for all client and HUD alarms.
- The saved setting applies immediately to current audio and stays for the next launch. Existing users retain the original 55% default.
- At 0%, audio is silent while current alarm sources and future reminders remain enabled. STOP and the alarm shortcut keep working.
- If the choice cannot be saved, the slider and audio retain the previous saved setting.
- EN/FR, capture, damage/healing/support, run history, progression, boss timers, favourites, HUD placement and shortcuts are preserved.

Français

- Réglez le volume des alarmes de 0 à 100 % directement dans les Préférences, pour le client et le HUD.
- Le réglage enregistré s’applique immédiatement au son en cours et reste au prochain lancement. Le volume initial de 55 % est conservé pour les utilisateurs existants.
- À 0 %, le son est coupé ; les sources d’alarme actives et les futurs rappels restent activés. STOP et son raccourci conservent leur fonctionnement.
- Si le choix ne peut pas être enregistré, le curseur et le son conservent le réglage précédent.
- Français/anglais, capture, dégâts/soins/support, historique, progression, timers, favoris, placement du HUD et raccourcis conservés.

Use UPDATE when offered, or download Eclipse-Setup.exe. Utilisez UPDATE lorsqu’il est proposé, ou téléchargez Eclipse-Setup.exe.

## v3.0.17 - WAIT tip and accessible patch notes

- A small WAIT card appears at the first overlay opening, once per Eclipse launch. It explains how teleporting somewhere in the dungeon or on the map may refresh character identity when personal damage is absent.
- The card is silent, keeps keyboard focus intact, has a close button and disappears automatically after 12 seconds. Hiding or recreating the overlay does not repeat it during the same launch.
- Patch notes stay directly below Show HUD, outside the scrolling menu, including at the minimum supported window size.
- In-app patch notes list released changes only. Ongoing reports are no longer mixed with completed fixes.
- Capture, damage/healing/support, character identity, run history, progression, boss timers, favourites, alarms, HUD placement and shortcuts are preserved.

Français

- Une petite carte WAIT apparaît au premier affichage de l’overlay, une seule fois par lancement d’Eclipse. Elle explique comment une téléportation dans le donjon ou sur la carte peut rafraîchir l’identification du personnage lorsque ses dégâts sont absents.
- Le conseil est silencieux, ne prend pas le focus, comporte une croix de fermeture et disparaît automatiquement après 12 secondes. Masquer ou recréer le HUD ne le répète pas pendant le même lancement.
- Les notes restent directement sous Afficher le HUD, hors du menu qui défile, même dans une petite fenêtre.
- Les notes du client affichent uniquement des changements publiés ; les signalements en cours ne sont plus mélangés aux corrections.
- Capture, dégâts/soins/support, identité, historique, progression, timers, favoris, alarmes, placement du HUD et raccourcis conservés.

Use UPDATE when offered, or download Eclipse-Setup.exe. Utilisez UPDATE lorsqu’il est proposé, ou téléchargez Eclipse-Setup.exe.

## v3.0.16 - Reliable startup damage and in-app patch notes

- Retain observed character and party frames while detecting the capture adapter. Only the selected game stream is replayed, with TCP sequence ordering and retransmission rejection, so already received startup data is not discarded or counted twice.
- Recover an obsolete connection when real game keepalives stop. TCP acknowledgements alone no longer keep it selected.
- Keep same-name characters on different servers distinct in party parsing and HUD filtering. Ambiguous names cannot replace a confirmed local identity.
- New Patch notes tab inside Eclipse, in English and French, with player-reported problems, released changes and clearly identified pending confirmations.
- Preserve death/resurrection continuity, cumulative damage, history, progression, healing/support, boss timers, alarms, HUD position and existing shortcuts.

Français

- Les informations du personnage et du groupe reçues pendant la détection réseau sont conservées. Seul le flux du jeu retenu est relu, avec ordre TCP et rejet des retransmissions pour éviter les doublons.
- Une ancienne connexion est récupérée lorsque les vrais messages de maintien du jeu cessent. Les simples accusés de réception TCP ne suffisent plus à la maintenir.
- Les personnages de même pseudo sur des serveurs différents restent distincts dans le groupe et le HUD. Un nom ambigu ne remplace pas une identité locale confirmée.
- Nouvel onglet Notes de mise à jour dans Eclipse, en français et en anglais, avec les retours des joueurs et les confirmations encore attendues.
- Compteurs après résurrection, dégâts cumulés, historique, progression, soins/support, timers, alarmes, placement du HUD et raccourcis conservés.

Use UPDATE when offered, or download Eclipse-Setup.exe. Utilisez UPDATE lorsqu’il est proposé, ou téléchargez Eclipse-Setup.exe.
Validation covers 1754 logic checks, the exact client, EN/FR native previews, ZIP and embedded setup, isolated saved-data migrations and shutdown. Synthetic fixtures reproduce the corrected code paths; confirmation of the affected TW player's exact case remains pending. The older Ranger/Assassin report is still under investigation.

## v3.0.15 - Keep your run, follow bosses more easily

- Preserve the current run and individual damage when the old local session ID is reused before resurrection PlayerInfo arrives. Optional identity metadata during that gap no longer clears the displayed personal total.
- The supported boss catalog is visible before game times arrive. Direct All bosses, Following, Favourites, Alarms and No alarm buttons replace the dropdown; search, zone filters and saved choices remain available.
- Stars and bells stay independent. Removing an alarm keeps the favourite. Unknown times remain unknown, and received world-boss times remain isolated by the exact detected server.
- Keep run history, progression, language, HUD position, healing, shields, selected support buffs and existing shortcuts. Idle live DPS still returns to zero without clearing cumulative damage.

Français

- Le run et les dégâts personnels restent conservés quand l’ancien identifiant local est réattribué avant les informations de résurrection. Les métadonnées reçues pendant cet intervalle ne masquent plus le total personnel.
- Le catalogue des boss pris en charge est visible dès le départ. Boutons directs Tous les boss, Suivis, Favoris, Alarmes et Sans alarme, avec recherche, zones et choix mémorisés.
- Favoris et cloches restent indépendants. Les horaires absents restent inconnus et les horaires reçus restent propres au serveur détecté.
- Historique, progression et préférences conservés. Le DPS instantané peut revenir à zéro pendant une pause sans effacer les dégâts cumulés.

Use UPDATE when offered, or download Eclipse-Setup.exe. Utilisez UPDATE lorsqu’il est proposé, ou téléchargez Eclipse-Setup.exe.
Validation includes 1716 logic checks and native EN/FR fixtures, exact ZIP/embedded setup, isolated migrations and shutdown. Fictional fixtures reproduce the confirmed code paths; they do not establish the affected player’s exact live-game case.

## v3.0.14 - Damage counters after resurrection

Eclipse 3.0.14 fixes individual damage totals after resurrection.

- A character receiving a new session ID after resurrection keeps the damage already dealt in the current run. A zero-damage first hit no longer hides the previous individual total in the HUD or client.
- Hits received late under the former session ID are credited once to the same character, including your own character. Party totals, skills and death counts stay consistent.
- Death and resurrection do not reset or archive the dungeon. Idle DPS still returns to zero after two seconds without clearing cumulative damage.
- Server-scoped identity protections, healing, shields, boss names and timers, favourites, alarms, shortcuts, run history, progression and preferences are retained. English is the initial language; French is available in Preferences.
- The website bug-report titles remain fixed and readable.

Use **UPDATE** when offered, or download the latest **Eclipse-Setup.exe**.
Validation: 1674 logic checks, including 21 counter regression checks, and 1226 native Windows checks in 34 suites. Exact ZIP and embedded setup, isolated upgrades from V1 and 3.0.8 through 3.0.13, saved data and quick offline shutdown checked. Fictional offline fixtures reproduce the confirmed identity-transition bug; they do not establish universal live-game coverage.

Français

- Les dégâts individuels restent conservés quand un personnage reçoit un nouvel identifiant après résurrection. Un premier coup à zéro ne masque plus le total précédent dans le HUD ou le client.
- Les coups reçus en retard sous l'ancien identifiant sont attribués une seule fois au même personnage, y compris votre propre personnage. Totaux du groupe, compétences et morts restent cohérents.
- La mort et la résurrection ne remettent pas le donjon à zéro. Le DPS instantané revient toujours à zéro après deux secondes d'inactivité, sans effacer les dégâts cumulés.
- Identités par serveur, soins, boucliers, boss et timers, favoris, alarmes, raccourcis, historique, progression et préférences conservés. Choix anglais/français inchangé.
- Les titres des rapports de bugs restent corrigés sur le site.

Mise à jour via **UPDATE** ou le dernier **Eclipse-Setup.exe**. Vérifications hors ligne avec données fictives ; la trace du joueur ayant signalé le problème n'a pas été reçue.


## v3.0.13 - Individual boss names and timers

Eclipse 3.0.13 gives each supported world boss its own name and timer.

- English and French names for 56 verified game-map entries: 24 in Verteron, 24 in Altgard and 8 in the Abyss. Argo, the Spirit King and Executor Argo are separate; Guardian Lord Nahma's three locations remain distinct.
- Individual calendar cards for Executor Argo, Kaira and Tamasa, plus named Watcher Kaira and Guardian Lord Nahma. Regional schedules are retained. KR/TW middle-zone calendar bosses also have individual cards.
- Stars and bells stay independent on each timer. Existing grouped favourites, muted alarms and acknowledged reminders migrate without arming quiet choices or repeating an acknowledged alarm.
- Search English or French boss names, including Argo in either language. Renaming keeps the original received times, detected EU server and saved tracking keys.
- Unrecognised maps or slots remain unresolved. Game-map timers require opening the monster list in game to synchronise; calendar times remain community predictions with the existing EU clock confirmation. No shared cross-server feed or invented spawn time.
- Damage, healing, shields, identities, history, progression, shortcuts and preferences are preserved. English remains the initial language; French is available in Preferences.

Use **UPDATE** when offered, or download the latest **Eclipse-Setup.exe**.
Validation: 1653 logic checks and 1215 native Windows checks in 34 suites, exact ZIP and embedded setup, isolated V1/3.0.8/3.0.9/3.0.10/3.0.11/3.0.12 upgrades, grouped-follow migration and quick offline shutdown. Fixtures use explicitly fictional data and do not establish universal live-game coverage.

Français

- Noms individuels en anglais et en français pour 56 entrées vérifiées : 24 à Verteron, 24 à Altgard et 8 dans les Abysses. Les deux variantes d'Argo sont séparées ; les trois emplacements de Nahma restent distincts.
- Cartes séparées pour Agro exécuteur, Kaira exécutrice et Tamasa l'exécuteur. Kaira la veilleuse et Nahma le seigneur gardien sont nommés. Les horaires régionaux existants sont conservés.
- Favoris et cloches indépendants pour chaque timer. Les anciens suivis groupés, choix silencieux et rappels acquittés migrent sans activer une alarme silencieuse ni répéter un rappel déjà reçu.
- Recherche des noms EN/FR ; les horaires reçus du jeu, le serveur EU détecté et les choix sauvegardés sont conservés. Les cartes inconnues restent non identifiées.
- Ouvrez la liste des monstres dans le jeu pour synchroniser les timers du serveur détecté. Le calendrier reste une prévision communautaire avec confirmation de l'horloge EU. Aucun horaire inventé ni flux partagé entre serveurs.
- Compteurs, soins, boucliers, identités, historique, progression, raccourcis et préférences conservés. Mise à jour via **UPDATE** ou **Eclipse-Setup.exe**.


## v3.0.12 - Support visible by default

Eclipse 3.0.12 makes personal support visible from the start.

- Self healing, shields and support buffs are enabled by default. Existing HUD settings are updated once; you can still hide personal detail in Preferences, and that later choice is remembered.
- Compact Support now shows a small shield icon with separate counts for allies and self, even when its details are collapsed. Open Support for each player's bars and received durations.
- Healing remains included once in its original totals. Shield counts reflect recognised packet observations; shield HP, absorption and destruction are not measured.
- Combat capture, damage, server identity, saved runs, progression, favourites, alarms and HUD shortcuts are retained. English is the initial language; French remains available.

Use **UPDATE** when offered in Eclipse, or download the latest **Eclipse-Setup.exe**.
Validation: 1600 logic checks and 1185 native Windows checks in 33 suites; exact ZIP and embedded setup; isolated upgrades from V1/3.0.8/3.0.9/3.0.10/3.0.11, default-setting migration and quick offline shutdown. Offline fixtures use fictional data and do not establish universal live-game coverage.

FR : les soins, boucliers et buffs personnels sont activés par défaut, également avec les anciens réglages. Une désactivation choisie ensuite reste mémorisée. Le mode compact affiche un résumé des boucliers sur alliés et sur soi sans ouvrir Support. Les détails et durées reçues restent accessibles, les soins ne sont pas comptés deux fois. Compteurs, identités, historiques, progression, alarmes et préférences conservés.


## v3.0.11 - Character identity fix and alarm shortcut

Eclipse 3.0.11 corrects character identity across servers and adds a quick way to stop boss alarms.

- Characters with the same nickname on different servers keep their own class and profile. Server switches no longer reuse the first character's class. Missing class data stays unknown until received.
- **Alt+M** stops all current alarms, even with Eclipse minimized or the HUD hidden, folded or closed. It leaves combat counters, game focus and future reminders alone.
- Choose **Alt+M**, **Alt+F9** or **Ctrl+Alt+M** in Preferences. The choice is saved. An occupied shortcut is reported; a failed save retains the previous working choice. Client and HUD STOP buttons remain available.
- A short, softly levelled **Reflection** notification replaces the previous boss cue. It repeats every3seconds until acknowledged. The startup intro remains silent. Recording provenance is included in the audio credits.
- The V3 quick-start guide and STOP hints show the chosen shortcut in English and French. English remains the initial language.
- Existing history, preferences, character progression, per-server game boss observations, calendar favourites and independent alarms are preserved.

Install with the latest **Eclipse-Setup.exe**, or click **UPDATE** when offered in Eclipse. Validation: 1583 logic checks and 1133 native Windows checks in32 suites; exact ZIP and embedded setup; isolated upgrades from V1/3.0.8/3.0.9/3.0.10 and quick offline shutdown. Native fixtures use fictional data and do not prove universal live-game coverage.

FR : correction des personnages ayant le même pseudo sur plusieurs serveurs. **Alt+M** arrête les alarmes en cours, même avec Eclipse réduit ou le HUD masqué, sans remettre les compteurs à zéro ni couper les futurs rappels. Raccourci modifiable dans les préférences, choix enregistré, conflit signalé et boutons STOP conservés. Nouveau son Reflection adouci, intro silencieuse. Guide EN/FR, historique, progression, favoris et réglages conservés.


## v3.0.10 - Direct timer bells and visible favourites

Eclipse 3.0.10 puts alarm bells directly where you use them: on the calendar boss timers and Next Rift card.

- Click a timer's bell to enable its alarm. Click it again to remove the alarm while keeping the favourite. A star alone stays silent; turning on one bell leaves other quiet favourites silent.
- Calendar and Rift favourites now appear in the shared Favourites & alerts list, alongside your own received game-boss timers. Search, active-alarm and silent-favourite filters include them.
- The same-region Rift card and calendar entry share their favourite and alarm. Different regions stay separate. Alarm choices are saved and a failed save rolls back the choice.
- Keep the 10-minute, 5-minute and scheduled-time choices. The bell repeats until STOP in the client or HUD; removing one alarm leaves unrelated ringing active.
- Calendar timers remain regional community predictions. European calendar boss alarms require clock confirmation in game. Field-boss times still come from each user's own game list and detected EU server; no guessed or shared server times.
- English and French, with English as the initial language. Existing HUD placement, shortcuts, combat counters, saved history, Progression and settings remain available.

Validation: 1077 native Windows checks across 31 suites, 1534 logic checks, exact ZIP/embedded setup, isolated V1/3.0.8/3.0.9 upgrades and offline shutdown. Screenshots and fixtures use fictional demo data and do not prove universal live-game coverage.

FR : Les cloches sont directement sur les cartes des boss du calendrier et de la prochaine faille. Activer une cloche ajoute le suivi ; retirer l'alarme garde le favori. Les favoris du calendrier et des failles apparaissent dans Favoris & alertes, avec les filtres habituels. Étoile seule silencieuse, choix enregistrés, délais 10/5/0 et STOP conservés. Prévisions du calendrier distinctes des données reçues de votre serveur dans le jeu. Historique et réglages conservés.


## 3.0.9 HUD placement correction - 9 October 2026

- HUD starts at bottom-right of the primary screen with a 12px logical margin; untouched legacy defaults migrate automatically.
- Growing content remains on-screen while default placement is active. Dragging remembers your chosen position; folding keeps the header in place.
- Version stays3.0.9. Existing3.0.9 users can run the newest setup again; UPDATE from earlier versions uses the corrected 3.0.9 package. History and preferences stay saved.

FR : Le HUD démarre en bas à droite avec une petite marge. Une position déplacée reste sauvegardée ; le repli conserve l’en-tête en place. Version3.0.9 inchangée : les utilisateurs déjà en 3.0.9 doivent relancer le dernier setup pour recevoir ce correctif.

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
