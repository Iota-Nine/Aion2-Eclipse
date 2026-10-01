# Eclipse release notes

## v1.0.30 — Update recovery and complete shutdown

- Fixes UPDATE closing Eclipse and reopening the old version after access-denied errors.
- Moves previous installed files aside, retries temporary Windows locks, handles read-only files and restores old files if installation fails.
- Uses the update tool from the verified release ZIP, waits for its readiness signal and checks the installed executable version.
- Displays download progress and retains failure details after restart.
- Fixes the close button leaving Eclipse in the background. Capture stops, combat history is saved and auxiliary windows close.
- Guarantees termination within eight seconds if driver, server or storage cleanup blocks.
- Setup closes older Eclipse instances, including invisible instances left behind by previous versions.

Validation reported in the release: 254 checks, updater tests and offline HUD shutdown checks. [Full release notes and Windows download](https://github.com/Iota-Nine/Aion2-Eclipse/releases/tag/v1.0.30).

If your older updater is stuck, install the latest ZIP once with `Eclipse.Setup.exe`.

## Eclipse V2 — unpublished prototype

Development work is isolated from the public release. The prototype includes a glass client, live local capture, expedition summaries, target timers, selectable timeline analysis, explicit A/B comparisons, favourites and notes, declared build context, dated meta sources, performance modes and connection diagnostics.

No V2 binary is available in the current public release. Prototype screenshots and offline demonstrations must not be interpreted as a released feature list or live player measurements.
