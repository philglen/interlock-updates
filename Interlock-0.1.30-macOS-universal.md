Interlock 0.1.30
================

This update cleans up duplicated broker accounts after Cloud sign-in.

Changes
-------

- Historical Cloud connection attempts are collapsed by MT5 login and broker
  server, with the current connected record taking priority.
- A local broker and its matching connected Cloud account now appear as one
  broker card while retaining the direct Cloud execution route.
- Failed or stale Cloud records no longer replace a healthy local broker.
- Cloud-only accounts remain visible once per distinct MT5 identity.

Verification
------------

- 324 Python tests pass.
- 21 desktop frontend tests and 9 mobile tests pass.
- Desktop and mobile production builds and native Capacitor sync pass.
