Interlock 0.1.29
================

This release unifies desktop and mobile Cloud sign-in and makes both apps
first-class controls for the same MT5 accounts.

Changes
-------

- Desktop now signs in with the same Interlock Cloud email identity as mobile,
  with a one-time link to an existing local desktop administrator.
- Cloud MT5 accounts and open positions now appear in the desktop trading desk.
- Orders, position changes, and closes from desktop and mobile travel directly
  to the owning MT5 engine over short-lived, capability-scoped WebSockets.
- Each terminal now keeps one writable MT5 attachment alive for low-latency
  execution instead of reconnecting for every trade.
- Added a durable per-terminal idempotency ledger. Interrupted or ambiguous
  commands are quarantined as unknown outcomes and are never silently retried.
- Fixed mobile native project synchronization in the release gate.

Verification
------------

- 323 Python tests pass.
- 18 desktop frontend tests and 9 mobile tests pass.
- Desktop and mobile production builds and native Capacitor sync pass.
