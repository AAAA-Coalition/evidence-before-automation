# Canaries and counterexamples

A test suite that has never been seen fail can create false confidence.

For every important rule:
1. positive witness — should pass;
2. negative witness — should fail;
3. counterexample — old/incorrect logic must fail;
4. regression test — corrected implementation stays green.

## UNKNOWN vs zero
- `count=null` -> `?`
- `count=0` -> `0`
- old fallback logic must fail the null fixture

## Capability attestation
- untested -> UNKNOWN
- tested success -> OUI
- tested denial/block -> NON for that session/instrument, not global impossibility

## Direct vs indirect network edge
- `direct=true` -> enters direct-collaboration count
- `direct=false` -> excluded from direct count; may enter shared-network proximity

## Actor requirements
- university-only consortium -> negative witness where a call requires other actor categories
- synthetic consortium meeting every minimum -> positive witness
- unreadable requirement -> UNKNOWN, never PASS
