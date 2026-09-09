# Interlock 0.1.33

- Separate Cloud execution and Local execution into clearly labelled broker sections and matching groups in the New Order selector.
- Show Live/Demo, current balance, availability and the default-account star in the selector.
- Put “Set as default” directly on eligible broker cards and keep that choice when a local account executes through Cloud.
- Reconcile unavailable local profiles with their working Cloud route by saved broker identity, avoiding duplicate or contradictory accounts.
- Rename the Brokers menu actions to describe what they actually do: add a local MT5 account or show broker accounts.
- Avoid displaying `undefined%` when a broker assessment does not supply a risk percentage.
