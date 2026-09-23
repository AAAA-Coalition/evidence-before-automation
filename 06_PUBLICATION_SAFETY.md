# Public release safety and claim discipline

Before release:
- remove secrets, token values/fingerprints and credential artefacts;
- remove private host details/private operational paths unless deliberately public;
- remove personal names from public failure examples unless separately authorised;
- use synthetic examples where possible;
- qualify internal metrics as internal;
- date every metric and state aggregation semantics;
- never claim external adoption from internal message volume;
- never claim cryptographic trust until implemented and verified;
- preserve negative findings/open gaps.

Recommended public sentence:

> This project publishes both working mechanisms and the counterexamples that broke our assumptions. The aim is not to claim infallibility, but to make evidence levels and failure modes reproducible.
