# 04 — Instruction-set architecture

Decoded operations are provisionally **Axiom**; encoded sequences are **Axiom Path**.

Candidate families: data movement, block composition/decomposition, 1024-bit arithmetic, sub-block operations, comparisons, loads/stores, control transfer, system entry, privileged control, and optional atomic operations.

Encoding remains open: compare fixed, variable, and structured hybrid formats. Evaluate code density, decode complexity, immediate range, extension space, alignment, and compiler cost.

Every accepted instruction must specify encoding, operands, exact result, architectural state effects, block aliasing, partial writes, exceptions, privilege, examples, and boundary tests. No opcode values are stable yet.
