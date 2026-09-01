# Interlock 0.1.17

This macOS reliability release fixes service lifecycle handling after an automatic update.

- Restarts stale UI and gateway services when their embedded build revision differs from the newly installed application.
- Pins packaged Interlock to its production profile and ports 8765/8766, keeping the side-by-side browser test profile isolated on 8875/8876.
- Prevents a new frontend from receiving an older in-memory account-summary schema, which could hide Balance, Equity, Floating, Stops, and Target totals while other live data continued updating.
- Waits for the previous Wine/launchd gateway listener to stop before loading its replacement.
- Preserves broker accounts, Telegram configuration, trade history, authentication, and chart settings.
