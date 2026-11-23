# SAND-1024 — Orryxen

**Experimental 1024-bit computing architecture research.**

SAND-1024 is an independent clean-sheet architecture experiment within the SAND Architecture Research Family. It shares family-wide design principles, but defines its own register organisation, instruction set, execution model, memory contract, toolchain, and ABI.

> **Status:** Research documentation only. No processor, emulator, kernel, full-width address space, or performance advantage is claimed.

## Research direction

Investigate extreme-width computation as explicit computational blocks. Compare monolithic scalar operations with block decomposition, determine whether sub-block operations are visible to software, and account for the cost of moving and preserving very wide architectural state.

## Provisional vocabulary

| Concept | Term |
|---|---|
| Architecture | Orryxen |
| 1024-bit scalar register | Mon |
| Register organisation | Monolith Array |
| Decoded instruction | Axiom |
| Instruction sequence | Axiom Path |
| Kernel environment | Nexum Core |
| Reference emulator | Deepframe |
| Toolchain | Axiom Forge |

Names are provisional and not claims of trademark uniqueness.

## Width discipline

A 1024-bit scalar does not imply 1024-bit pointers, virtual addresses, physical addresses, or installed RAM. These are separate design parameters.

## SAND Universal Architecture Foundation

All architectures in the SAND family follow the shared [SAND Universal Architecture Foundation (SUAF)](docs/00-sand-universal-architecture-foundation.md). It establishes common engineering principles and terminology while preserving independent instruction sets, register models, memory contracts, execution semantics, and ABIs.


## Numerical Systems Research

The shared [SAND Numerical Systems Research (SNSR)](docs/22-sand-numerical-systems-research.md) programme investigates alternative radices and numeric representations, including **sexagesimal (base-60)**, balanced ternary, decimal/BCD, fixed- and floating-point, and residue number systems. These are research topics, not claims that every format is implemented in the ISA.

## Documentation

See [docs](docs/) for the architecture charter, register and numeric model, instruction set, memory and address model, execution, protection, emulator, toolchain, ABI, kernel, capabilities, verification, roadmap, and decisions.

## Planned structure

```text
specifications/  Machine-readable ISA definitions
emulator/        Deepframe reference emulator
assembler/       Assembler and disassembler
toolchain/       Linker, image builder, compiler experiments
boot/            Virtual platform boot contract
kernel/          Nexum Core experimental kernel
tests/           Architecture conformance tests
```

Directories will be created when meaningful implementation begins.

## Current status

| Area | Status |
|---|---|
| Charter / terminology | Drafted / proposed |
| Register / numeric model | Proposed |
| ISA / encoding | Open |
| Address / memory model | Open |
| Emulator / toolchain / kernel | Not implemented |
| Hardware | Not implemented |

## License

No license has been selected. All rights are reserved unless and until a license is added.
