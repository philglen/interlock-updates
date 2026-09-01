# Interlock 0.1.22

This authentication repair prevents a mistyped username from silently creating
a second local administrator during password recovery.

- Resets only an existing, case-sensitive local administrator username.
- Explains an unknown username instead of reporting a misleading successful
  reset.
- Clears failed-login lockout state and revokes earlier sessions after a valid
  reset.
- Restores Interlock's single-administrator invariant by removing accidental
  secondary login records created by the older reset workflow.

The macOS application remains Developer ID signed, notarized and distributed
through its signed Sparkle update feed.
