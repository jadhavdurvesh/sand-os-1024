# 05 — Memory and address model

Register width, block width, pointer width, virtual address width, physical address width, and memory transfer width are independent.

Specify load/store sizes, alignment, byte order, extension, effective-address formation, valid virtual ranges, translation tables, permissions, invalidation, fault reporting, atomicity, and memory ordering.

A theoretical 2^1024-byte address space is not a hardware memory target. Real capacity depends on implemented address bits, devices, buses, controllers, translation structures, and platform constraints.

Choose a practical address width independently of the 1024-bit scalar target.
