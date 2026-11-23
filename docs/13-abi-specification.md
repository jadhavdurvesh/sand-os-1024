# 13 — ABI specification

**Status:** Not yet specified.

The ABI must define pointer width, argument and return locations, register preservation, stack layout and alignment, aggregate layout, system-call entry, error representation, relocation types, symbol conventions, and extension-state handling.

A 1024-bit value may be passed in one register, multiple registers, or memory. Define the convention, alignment, and costs explicitly. A 1024-bit scalar does not imply 1024-bit pointers.

ABI compatibility requires stable documented rules and conformance tests.
