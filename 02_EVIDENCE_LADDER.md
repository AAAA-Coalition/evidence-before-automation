# Evidence ladder

## States
- `VERIFIED` — directly tested against the claim.
- `SOURCE_BACKED` — source directly supports exactly the stated level.
- `MEMBER_CONFIRMED` — confirmed by the responsible member/owner.
- `DECLARED` — reported, not independently checked.
- `DERIVED` — computed or inferred from other evidence.
- `UNKNOWN` — insufficient evidence.
- `REJECTED` — tested and contradicted.

## Non-escalation
A state may rise only when a new instrument adds evidence.

```json
{
  "claim": "...",
  "state": "UNKNOWN",
  "source": null,
  "instrument": null,
  "timestamp_utc": null,
  "scope": null,
  "caveat": null
}
```
