# AION 2 · Eclipse

Yo.

Eclipse is a small DPS meter that sits on top of AION 2. Party damage, your damage, levels, fight timer — the stuff you glance at mid-fight without alt-tabbing into a giant window.

It watches the game’s network packets (Npcap). It does **not** read AION’s memory and it doesn’t click anything for you. Overlay only.

I only put the **ready-to-run Windows build** here. No source code in this repo. That’s on purpose.

---

## What you get

- Your row + your party when the game sends the group list
- DPS for the current fight (resets after you stop hitting for a bit)
- **Total damage** that stays until you hit the reset button (↺)
- Levels when we get them from party packets
- Click-through mode so you can play through the HUD (purple strip / Ctrl+Shift+L to grab the mouse back)
- Auto-update: when I drop a new build, Eclipse notices and shows a little **UPDATE** chip up top — you click it, it downloads, restarts. Done.

Not included / not magic: it won’t tell you the perfect rotation, it won’t invent party members the game didn’t send, and exclusive fullscreen can hide overlays (use windowed / borderless).

---

## Install (2 minutes)

1. Grab the zip from [Releases](https://github.com/Iota-Nine/Aion2-Eclipse/releases/latest) — the big `.zip`, **not** “Source code”
2. Extract the folder somewhere you can write
3. Install [Npcap](https://npcap.com/#download) with **WinPcap API-compatible Mode** checked
4. Run `Aion2-Eclipse.exe`, then enter the world in AION 2

No .NET install needed. No account. Free for personal use — don’t sell it or shove it in a paid pack ([LICENSE](./LICENSE)).

---

## Controls

| Thing | How |
|---|---|
| Move it | Drag the Eclipse header |
| Hide / show | Ctrl + Shift + H |
| Click-through | ◇ or Ctrl + Shift + L |
| Mouse back on HUD | Purple strip or Ctrl + Shift + L |
| Reset totals | ↺ or Ctrl + Shift + R |
| Class skill list | Build |

---

## About updates (read this)

When I ship a new version, I write **what actually changed** in that Release — not just “update available”.

Your Eclipse checks GitHub every couple of minutes. If there’s something newer, you get a gold **UPDATE** button in the header. Click it → it pulls the zip → restarts on the new build. Keep `Eclipse.Updater.exe` next to the main exe (it’s in the zip).

Fresh install? Always take the **latest** Release.

---

## If something’s weird

- No numbers → Npcap / driver / run as a normal user with write access to the folder
- Overlay missing → don’t use exclusive fullscreen
- Settings & logs live in `data/` next to the exe — don’t share that folder
- Game patches break packet layouts sometimes. If meters go stupid after a patch, wait for a new Release from me

Not affiliated with NCSOFT. Made this for my own runs; sharing the build so other people don’t have to reinvent the same HUD.

— Iota-Nine
