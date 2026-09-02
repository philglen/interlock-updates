# Interlock 0.1.25

This update restores manual live-order permission in the packaged macOS app
and adds persistent display-currency conversion.

- Fixes valid manual orders being rejected with `ALLOW_LIVE_TRADING is false -
  calculator only` while signal bots could still trade.
- Adds a persistent display-currency selector for GBP, USD, EUR, CNY, JPY,
  AUD, NZD, CHF and CAD.
- Converts monetary values using live broker FX mid quotes without changing
  native broker balances or stored history.
- Uses standard currency precision and removes silent GBP fallbacks.

The macOS application remains Developer ID signed, notarized and distributed
through its signed Sparkle update feed.
