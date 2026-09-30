# Eclipse — free AION 2 DPS meter

**See your party’s damage while you fight. No signup. No paywall. Download the exe and go.**

[⬇️ **Download free (Windows)**](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest)

Grab the big `.zip` on that page — **not** “Source code”. Extract → run `Aion2-Eclipse.exe`.

---

## What Eclipse does

You’re mid-dungeon. Somebody’s carrying. Somebody’s not. Eclipse puts a thin overlay on top of AION 2 so you can **see live party damage** without alt-tabbing or opening a second app.

| You get | Why it matters |
|---|---|
| **You + your party** on one meter | Know who actually hits when the boss dies |
| **Fight DPS** (resets when combat idles) | Clean number for the pull you just did |
| **Total damage** (until you hit ↺) | Session totals that don’t vanish mid-run |
| **Levels** when the game sends them | Roster that looks like your group UI |
| **Click-through HUD** | Play through the overlay; purple strip / hotkey when you need the mouse |
| **Auto-update** | Gold **UPDATE** chip when I ship — one click, restart, done |

Built for people who want the meter **and nothing else** in the way. No account. No Discord login. No “Pro” tier. Free for personal use.

---

## Why this one

Most meters want you to install half a toolkit, make an account, or bury the download under a website. Eclipse is the opposite:

- **Exe only** in this repo — ready to run
- **Npcap packets** — reads combat traffic the game already sends. No memory reading, no injecting, no clicking for you
- **Stays on top** of borderless / windowed AION 2
- **Updates itself** when I push a Release

If you just want “who did how much damage in this dungeon,” this is that.

---

## Install (about 2 minutes)

1. **[Download the latest Release](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest)** → the `.zip`
2. Extract somewhere you can write (Desktop folder is fine)
3. Install [Npcap](https://npcap.com/#download) and check **WinPcap API-compatible Mode**
4. Run `Aion2-Eclipse.exe`, then enter the world in AION 2

No .NET desktop runtime to hunt down. Keep `Eclipse.Updater.exe` next to the main exe (it’s in the zip).

**Free.** Don’t sell it, don’t put it in a paid pack — see [LICENSE](./LICENSE).

---

## Controls

| Action | How |
|---|---|
| Move | Drag the Eclipse header |
| Hide / show | `Ctrl + Shift + H` |
| Click-through | ◇ or `Ctrl + Shift + L` |
| Mouse back on HUD | Purple strip or `Ctrl + Shift + L` |
| Reset totals | ↺ or `Ctrl + Shift + R` |
| Compact / Full | Toggle in the header |

---

## Updates

Every Release has **real notes** (what broke, what I fixed) — not “misc improvements.”

While Eclipse is open it checks GitHub often. Newer build → gold **UPDATE** in the header → click → download → restart. Always prefer the [latest Release](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest) for a fresh install.

---

## If numbers don’t show

- Reinstall Npcap with WinPcap API-compatible mode
- Don’t use exclusive fullscreen (borderless / windowed)
- Give the folder write access — settings live in `data/` next to the exe (don’t share that folder)
- After a big game patch, packet layouts can shift — wait for a new Release from me

Not affiliated with NCSOFT. I built this for my own groups and publish the build so other players can use it free.

**Start here → [Download Eclipse](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest)**

— Iota-Nine
