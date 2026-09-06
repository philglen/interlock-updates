Interlock 0.1.27
================

This macOS release fixes the desk's order ticket losing track of newly added
broker accounts, adds per-account execution location control shared with the
mobile companion, and brings the companion API's position commands online.

Changes
-------

- Fixed the New Order broker list not updating after a broker account was
  added, restored or archived. The ticket now follows the live accounts
  panel, and falls back to the first account if the selected one is removed.
- Added per-account execution location: each broker account can execute on
  Local MT5 or Cloud MT5 but not both. The gateway refuses order submission
  for local accounts whose execution is switched off, so a signal copied by
  the cloud engine cannot also be placed by the desktop bot.
- Added `POST /v1/trading/positions/{ticket}/close` and `/modify` to the
  companion API with command receipts and audit records. Close supports
  partial volume. The gateway records these commands in the execution ledger
  whenever an idempotency key is supplied, so a companion retry after a lost
  acknowledgement never closes a position twice.
- Position snapshots now include `opened_at` (broker clock corrected to UTC).
- Mobile companion: tapping an open position opens a position sheet with
  partial close, close, stop to break-even and stop/target editing. Stop
  changes apply immediately; closing asks for confirmation.

Verification
------------

- Full Python unit suite passes (282 tests).
- Frontend type-check passes.
- Mobile type-check, unit tests and production build pass.
