# 07 — Emulator design

**Reference emulator:** Deepframe (provisional).

Deepframe should be a deterministic executable specification, not a speed-first simulator.

## Components
Image validator, fetch/decode, 1024-bit arithmetic helpers, architectural state, block-view logic, memory, executor, exception engine, trace writer, and conformance harness.

## Wide-value representation
A portable model may represent a 1024-bit value as sixteen 64-bit limbs. Specify limb order, carry/borrow propagation, signed interpretation, shifts, multiplication, division, and serialization explicitly. Never rely on host overflow.

## Required tests
Zero and maximum values; signed boundaries; carry across all sixteen limbs; shifts at 0, 1023, 1024, and larger; division corner cases; block aliasing; partial writes; memory faults; invalid encodings; deterministic replay.
