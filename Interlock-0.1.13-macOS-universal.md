# Interlock 0.1.13

This is the Sparkle bridge release for macOS automatic updates.

- Rotates the embedded Sparkle public update key.
- Restores signed appcast publication using the regenerated local Sparkle key.
- Keeps chart-alert delivery and macOS notification bridge changes from the current benchmark work.
- Adds release preflight checks so future appcast publishing fails before a long notarized build when the Sparkle signing key is unavailable.

Install this build manually once if your current Interlock copy cannot update itself. Future updates should then be available through **Interlock → Check for Updates…**.
