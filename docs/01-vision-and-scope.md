# 01 — Vision and scope

**Codename:** Orryxen · **Scalar target:** 1024 bits · **Status:** Research proposal

SAND-1024 investigates extreme-width scalar computation and block-oriented machine design. Its central question is whether a 1024-bit value should be treated as one monolithic architectural scalar, as a structured block, or through a hybrid model.

## Goals
- Define an original machine contract and ISA.
- Specify 1024-bit arithmetic and data representation precisely.
- Compare monolithic and block-visible register models.
- Account for architectural state movement and context preservation.
- Keep pointer, virtual-address, physical-address, and instruction widths independent.
- Build a deterministic emulator before considering hardware.

## Non-goals
No commercial processor, compatibility promise, performance claim, or assumption that 1024-bit registers require 1024-bit addressing.

| Property | Initial direction |
|---|---|
| General scalar register | 1024 bits, proposed |
| Native integer arithmetic | At least 1024 bits, proposed |
| Pointer width | Open |
| Virtual / physical address widths | Open |
| Instruction encoding | Open |

Success means a precise, testable specification and emulator, not a theoretical memory number.
