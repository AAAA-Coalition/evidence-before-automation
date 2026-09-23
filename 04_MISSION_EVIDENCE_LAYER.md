# Mission & Evidence Layer

Lot 2 asks whether a request can travel and return auditable protocol messages.

Lot 3 asks whether the mission can be trusted and reused.

```text
NEED -> MISSION -> TASK -> HANDOFF -> EVIDENCE -> DECISION
     -> DISSENT (optional) -> CLOSE -> REUSE
```

## Minimal mission
```yaml
mission_id: stable-id
requested_by: human-or-institution-id
mandate: explicit-scope
owner: session-or-team
status: OPEN
evidence_policy: evidence-ladder-v1
human_gate:
  required: true
  decision: null
```

## Minimal evidence receipt
```yaml
claim_id: stable-id
claim: human-readable statement
state: VERIFIED | SOURCE_BACKED | MEMBER_CONFIRMED | DECLARED | DERIVED | UNKNOWN | REJECTED
source_ref: optional
instrument: command/test/readback
timestamp_utc: optional
scope: explicit
caveat: explicit
```

## Close rule
A mission is not CLOSED because work stopped. Closure requires a result or explicit rejection, evidence state, owner, relevant human decision/gate, and a reusable reference or explicit non-reusability reason.
