# Interlock 0.1.10 Private Alpha

This release expands Interlock's chart analysis with independently selectable EMA 9, 21, 50 and 200 overlays in a compact multi-select control.

Optional annotations identify 9/21 momentum crosses, golden crosses and death crosses. Candle patterns at historically confirmed support or resistance now show outcome scoring when at least five decided examples are available; smaller samples remain hidden.

Chart controls have been tightened further, Clear now sits beside the timeframe controls, and opt-in chart alerts can notify you about newly completed qualifying candle-pattern and EMA-cross signals. Alerts never place, modify or close trades.

Telegram signal listeners now share the same Application Support state as the app. A connection heartbeat recovers half-closed Telegram sockets automatically, while messages delayed by more than five minutes are ignored so reconnecting cannot execute stale signals.

The chart history has increased to 600 candles for better EMA warm-up and scoring. This release also removes hard-coded username defaults and adds repository tooling for running released and testing interfaces side by side.
