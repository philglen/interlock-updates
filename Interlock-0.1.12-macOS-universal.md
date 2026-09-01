# Interlock 0.1.12 Private Alpha

This release packages the large portability and charting benchmark update.

- Chart alerts now use browser and native macOS notification adapters with explicit delivery feedback.
- The chart workspace, indicators, pattern scoring, EMA controls and chart data polling have been refactored into smaller tested modules.
- Broker account management now supports display-name updates, default account selection, MT5 verification, safe archive and restore while preserving history.
- The app now has stronger runtime identity reporting so source browser testing and the installed app can run side by side without silently sharing stale state.
- Mutable broker, Telegram, quota and runtime state now goes through one transactional owner with revision checks.
- Mixed-currency account totals are grouped by currency instead of being incorrectly labelled as GBP.
- The app has new frontend accessibility, visual regression and E2E coverage for broker onboarding, order review, archive/restore and halt/resume.
- macOS packaging now includes native command dispatch, Sparkle wiring and notification bridge verification.

Existing broker passwords remain outside Interlock. After installing, use **Manage broker account** and **Verify MT5 connection** if MT5 credentials were changed directly in MT5.
