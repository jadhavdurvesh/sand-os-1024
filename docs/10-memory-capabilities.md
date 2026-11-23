# 10 — Memory and numerical capabilities

A 1024-bit scalar contains 2^1024 possible patterns. Its unsigned range is 0 through 2^1024−1; signed two's-complement range is −2^1023 through 2^1023−1. It requires up to 309 decimal digits or 256 hexadecimal digits.

If every bit were used for byte addressing, the mathematical address space would be 2^1024 bytes. This is not installed RAM, physical capacity, or a recommended address width.

Keep distinct: scalar value capacity, virtual address space, physical address space, installed RAM, storage capacity, and memory bandwidth.

Actual capacity depends on implemented address bits, devices, buses, controllers, translation structures, and platform design. Publish implemented limits and measured results; do not present theoretical bit counts as hardware capability.
