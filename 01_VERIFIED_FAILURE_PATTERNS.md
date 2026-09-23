# Verified failure patterns

## 1 — Assumed incapability
**Failure:** a session was treated as unable to reach a host before the simplest direct test was run.  
**Counter-instrument:** run the command.  
**Rule:** `UNKNOWN` until tested; `NO` only after test.

## 2 — UNKNOWN silently became zero
**Failure:** frontend normalisation used literal zero as fallback; unknown counts displayed as `0`.  
**Counter-instrument:** fixtures containing both `null` and true `0`.  
**Rule:** unknown and zero need separate witnesses.

## 3 — Raw relationship count became a unique-network claim
**Failure:** a raw total was interpreted as unique partners/edges.  
**Counter-instrument:** explicit deduplication and separate counters.  
**Rule:** publish aggregation semantics beside the number.

## 4 — Direct collaboration mixed with shared-neighbour proximity
**Failure:** one list contained both `direct:true` and `direct:false`; its total could be read as direct collaborations.  
**Counter-instrument:** expose/count the discriminator.  
**Rule:** direct collaboration and shared third-party partner are distinct relations.

## 5 — Institutional evidence became a people-level story
**Failure:** a source-backed relation between legal entities could be retold as evidence that two people worked together.  
**Counter-instrument:** person/project fields remain null until separately sourced.  
**Rule:** institutional evidence never auto-promotes to personal evidence.

## 6 — Local page produced a false runtime diagnosis
**Failure:** a page opened under `file://` necessarily used fallback/demo data and could be mistaken for backend failure.  
**Counter-instrument:** QA through the served runtime URL.  
**Rule:** test the layer being claimed.

## 7 — `completed` was stronger than the evidence
**Failure:** a security task carried a historical completed label although direct closure evidence was incomplete.  
**Counter-instrument:** direct invalidation/revocation test where safely possible.  
**Rule:** critical historical status must be re-proved before reuse.
