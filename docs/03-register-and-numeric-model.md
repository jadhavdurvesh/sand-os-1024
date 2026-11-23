# 03 — Register and numeric model

**Register:** Mon · **Register organisation:** Monolith Array (provisional).

A 1024-bit scalar contains 128 octets and has 2^1024 possible bit patterns.
- Unsigned range: 0 through 2^1024−1.
- Signed two's-complement range: −2^1023 through 2^1023−1.
- Up to 309 decimal digits or 256 hexadecimal digits.

## Register model
The key open choice is monolithic versus block-visible state. Specify register count, block widths, ordering, overlap, aliasing, partial writes, atomicity, reset, privilege visibility, and context-save rules.

## Arithmetic contract
Define wrap/trap/saturate behaviour, carry and borrow propagation, signed and unsigned comparisons, division-by-zero, signed division corner cases, shifts, and source/destination aliasing.

## State cost
A 1024-bit register bank can make context switching and interrupt preservation expensive. Do not claim practical efficiency without measuring the actual register count and state-save workload.

Binary is the underlying representation; decimal, octal, and hexadecimal are not separate machine architectures.
