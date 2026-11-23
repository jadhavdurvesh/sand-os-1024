# 02 — Architecture overview

**Architecture:** Orryxen · **Status:** Proposed

Layers: value and block model; register inventory; instruction encoding and semantics; execution and retirement; memory and translation; protection and events; platform reset/boot; executable format and ABI.

## Extreme-width investigation
Compare:
- A monolithic 1024-bit scalar register.
- A block composed of smaller architectural elements.
- A hybrid design with full-width operations and explicitly exposed sub-block operations.

For each model, evaluate encoding cost, data movement, partial writes, aliasing, compiler visibility, context-save size, and emulator complexity.

Start with deterministic single-core sequential execution. Speculation, out-of-order execution, multicore, and cache coherence are deferred.

A 1024-bit register does not imply 1024-bit pointers or addresses. Address formation and translation are independent.
