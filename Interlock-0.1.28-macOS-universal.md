Interlock 0.1.28
================

This macOS release makes the desk and mobile companion react to trading-state
changes immediately, without waiting for their next polling refresh.

Changes
-------

- Added a shared authenticated event stream for account, position, broker,
  signal, activity and system-state updates.
- The desktop desk and mobile companion now refresh the affected data as soon
  as Interlock publishes an event, keeping both surfaces in step.
- Added reconnect handling with bounded backoff and visibility-aware recovery
  for temporarily interrupted event streams.
- A dropped stream is only reported as stale after it has connected at least
  once, avoiding a false warning during initial sign-in and application start.
- Fixed a startup cache edge case that could briefly suppress broker, signal
  and activity events immediately after launching Interlock.
- The mobile development server now targets the installed desk profile by
  default, matching the data shown in the native desktop application.

Verification
------------

- Python event-bus, event-stream and desk-event tests pass.
- Frontend and mobile type-checks pass.
- Frontend and mobile production builds pass.
