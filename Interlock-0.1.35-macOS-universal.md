# Interlock 0.1.35

## Fixed

- Restore the desktop Cloud session automatically from the macOS Keychain after app and service restarts, without showing a reconnect prompt.
- Support Cloud-first, standalone-desktop and combined desktop/mobile authentication flows.
- Route Cloud instrument search, quote assessment and chart history through the selected Cloud broker connection.
- Subscribe the desktop order ticket and current chart candle to the direct MT5 WebSocket feed instead of presenting queued snapshots as live prices.
- Keep explicit sign-out authoritative by clearing the saved device session.
- Prevent Python bytecode caches from modifying the signed application bundle.

## Changed

- Cloud quote status now distinguishes direct MT5 `connecting`, `live` and `offline` states and reports the age of the last broker tick.
