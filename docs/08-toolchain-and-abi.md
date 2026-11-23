# 08 — Toolchain and ABI

**Toolchain:** Axiom Forge (provisional).

Build sequence: freeze the base instruction subset; implement assembler/disassembler; define versioned object and executable formats; add linker/image builder; add compiler support after ABI decisions stabilise.

The ABI must define pointer width, argument and return locations, register preservation, stack alignment, aggregate layout, system-call entry, error representation, relocation types, and extension-state rules.

A 1024-bit value may be passed in one register, a register group, or memory. Define the convention and alignment explicitly. A 1024-bit scalar does not force 1024-bit pointers.

Require assembler/disassembler round trips, relocation tests, malformed-image rejection, and ABI conformance tests.
