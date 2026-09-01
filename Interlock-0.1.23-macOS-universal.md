# Interlock 0.1.23

This corrective update restores sign-in after changing the local Interlock
password.

- Fixes the packaged login response failing after valid credentials were
  accepted, which appeared in the app as `Load Failed`.
- Adds the Interlock application icon to the native password-reset,
  confirmation and error dialogs.
- Retains exact-username password recovery, cleared lockouts and revoked
  earlier sessions.

The macOS application remains Developer ID signed, notarized and distributed
through its signed Sparkle update feed.
