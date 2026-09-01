# Interlock 0.1.11 Private Alpha

Broker accounts now have a single **Manage broker account** dialog for changing the display name, selecting the default account, verifying the MT5 connection, and safely archiving an unused account.

Archiving is blocked while positions or pending orders remain, disables assigned copy trading only with confirmation, and preserves trade and audit history. Archived accounts appear in a separate list and can be restored later without silently re-enabling copy trading.

Interlock continues to keep broker credentials outside the application. If an MT5 password changes, sign the saved terminal back in and use **Verify MT5 connection**.

Opening the full-screen chart workspace now carries across the mini-chart timeframe, OHLC preference, enabled overlays, EMA selections, support/resistance settings, session levels, and chart-alert state.
