# lifeos-contracts

Event contracts between services. One folder per topic:

- `schemas/envelope.schema.json`: the envelope every event uses
- `schemas/strategy/`: events on `lifeos.strategy.events.v1`
- `schemas/coach/`: events on `lifeos.coach.events.v1`
- `schemas/trigger/`: events on `lifeos.trigger.events.v1`

Versioning: semver. A breaking change means a new version of the event (`eventVersion` is incremented);
the old version keeps being published for a transition period.
