# Interlock 0.1.31

- Keep desktop Sign out available when only the Cloud session expires; offer a separate Cloud reconnect link.
- Correct the local MT5 candle timestamp helper so charts display in the device timezone.
- Organize broker accounts with device/Cloud filters, explicit connection labels, a single Add action and a collapsed archive.
- Preserve local profile management for accounts also connected through Cloud.
- Move account commands into a Brokers menu; register the macOS Window menu and add Control-Command-F for full screen.

The Windows Cloud worker source also normalizes candle timestamps; existing Cloud workers require a separate deployment to receive that change. No running MT5 terminals are closed or reconfigured by this update.
