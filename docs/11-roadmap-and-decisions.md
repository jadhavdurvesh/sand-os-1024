# 11 — Roadmap and decision register

## Roadmap
A. Charter and terminology.  
B. Freeze scalar/block semantics, instruction encoding, arithmetic, address model, reset, privilege, and traps.  
C. Build deterministic Deepframe emulator.  
D. Add assembler, disassembler, executable format, and linker.  
E. Boot a minimal Nexum Core kernel.  
F. Measure state-save cost, arithmetic cost, code density, and memory transfer behaviour.

## Open decisions
- Monolithic scalar versus block-visible register state.
- Register count, block widths, ordering, aliasing, and partial writes.
- Instruction encoding and immediate formats.
- Pointer, virtual-address, and physical-address widths.
- Endianness, alignment, and memory ordering.
- Privilege levels, interrupts, and ABI.

## Decision policy
Every accepted choice needs context, alternatives, rationale, consequences, affected specifications, and conformance tests. A feature moves from proposed to accepted, implemented, and verified only with evidence.
