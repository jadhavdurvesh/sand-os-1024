# 15 — Architecture decision register

**Codename:** Orryxen

Statuses: Open, Proposed, Accepted, Superseded, Rejected.

### O1024-001 — Project independence
**Status:** Accepted. SAND-1024 is an independent architecture in the SAND family. Shared principles do not imply shared ISA or ABI.

### O1024-002 — Scalar width
**Status:** Proposed. General-purpose scalar target is 1024 bits.

### O1024-003 — Scalar versus block model
**Status:** Open. Compare monolithic scalar registers, block-visible registers, and a hybrid model. Define aliasing, partial writes, and context-save behaviour.

### O1024-004 — Register inventory
**Status:** Open. Select register count, block widths, special state, and reset behaviour.

### O1024-005 — Address widths
**Status:** Open. Choose pointer, virtual, and physical address widths independently.

### O1024-006 — Instruction encoding
**Status:** Open. Compare fixed, variable, and structured hybrid formats.

### O1024-007 — Endianness and memory transfer
**Status:** Open. Specify byte order, access sizes, alignment, and transfer strategy.

### O1024-008 — Privilege and events
**Status:** Open. Define privilege domains, reset, traps, interrupts, and return semantics.

### O1024-009 — ABI
**Status:** Open. Define calling convention, pointer representation, system-call ABI, and executable format.

Every accepted decision must include context, alternatives, rationale, consequences, affected specifications, and conformance tests.
