# AION 2 · Eclipse

Hey. This is a small overlay HUD I built for AION 2 — party DPS, personal totals, level column, skill suggestions, the usual meter stuff, but as a compact always-on-top panel instead of a giant window.

I ship **binaries only** here. No source tree in this repo on purpose. Grab the latest build from **Releases** (the zip), extract it somewhere you can write to, and run `Aion2-Eclipse.exe`.

**License (short version):** free for personal use. **Do not sell it, rebrand it, or slap it in a paid pack.** Full terms in [`LICENSE`](./LICENSE). If you find a paid mirror of my build, it’s unauthorized — tell me.

---

## Download

1. Open the [latest Release](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest)
2. Download `Aion2-Eclipse-*-win-x64.zip` (not “Source code”)
3. Extract the whole folder
4. Install [Npcap](https://npcap.com/#download) if you don’t already have it — tick **WinPcap API-compatible Mode**
5. Launch `Aion2-Eclipse.exe`, then log into AION 2 (windowed or borderless)

That’s it. .NET is baked into the exe. No account, no paid API key.

---

## What it actually does

Eclipse reads the game’s network traffic with Npcap (same general idea as RATmeter / packet meters). It does **not** open the AION process and poke memory.

You’ll get:

- One row per party member when the game sends the party list (name, class, DPS, total damage, level)
- Solo row for you if you’re not grouped
- Fight DPS that resets after idle · **total damage that only resets when you hit ↺** (or Ctrl+Shift+R)
- Sticky character id after the first identification so you don’t need to teleport every login just to see your row
- Party clear when you leave / get an empty list (no more ghost allies hanging around)
- Optional click-through so mouse clicks go to the game; purple strip or Ctrl+Shift+L brings the mouse back to the HUD

Skill suggestions are “what I observed hit hard + what’s off cooldown,” not a perfect rotation bot. Stigmas, combo conditions, range — that’s still on you.

---

## Hotkeys

| What | How |
|---|---|
| Move HUD | Drag the Eclipse header |
| Show / hide | Ctrl + Shift + H |
| Click-through | ◇ button or Ctrl + Shift + L |
| Grab mouse back | Purple strip at the bottom of the HUD, or Ctrl + Shift + L again |
| Reset totals | ↺ or Ctrl + Shift + R |
| Compact suggestions | ▤ |
| Class build panel | Build |

---

## Updates

On startup Eclipse checks this repo’s **Releases**. Newer zip → downloads → `Eclipse.Updater.exe` swaps files → relaunch.

I don’t push source here. When I ship a fix I just cut a new Release tag. You keep playing; next time you open Eclipse it should update itself (needs the updater exe from the original zip, and internet).

---

## Notes / honesty box

- Exclusive fullscreen can hide overlays. Windowed / borderless works.
- If capture fails, check Npcap install + that you’re not blocking the driver.
- Logs and settings live in a `data/` folder next to the exe after first run. Don’t zip that folder when sharing.
- Local read-only API on `127.0.0.1:18942` if you want to script something. Token in `data/api-token.txt`. Not an official NC API.
- Community project, not affiliated with NCSOFT / AION. Icons and names belong to their owners.
- Packet layout changes when the game patches — if numbers look wrong after an update, wait for a new Release from me.

Built this for my own sessions, figured other people might want the same compact meter. If something’s broken, open an Issue on the Release page or yell at me wherever you found the link.

— Iota-Nine
