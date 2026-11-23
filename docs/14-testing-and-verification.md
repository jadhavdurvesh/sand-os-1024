# 14 — Testing and verification

## Verification levels
Arithmetic helpers; register/block-view state; decoder; instruction semantics; memory translation and permissions; traps and privilege; assembler/disassembler round trips; ABI programs; kernel boot; deterministic replay.

## Extreme-width cases
Test carry and borrow across all sixteen 64-bit limbs, signed boundaries, maximum values, shifts around 1024 bits, division corner cases, block aliasing, partial writes, serialization, and context-save/restore integrity.

## Status labels
Proposed, accepted, implemented, verified, deferred. A feature is verified only when tests demonstrate its specified behaviour.
