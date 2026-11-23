# 09 — Kernel and boot architecture

**Kernel environment:** Nexum Core (provisional).

The first target is a virtual platform in the reference emulator. Specify reset state, memory map, reserved regions, image format, entry privilege, loader responsibilities, handoff data, and device discovery before implementing boot.

Initial kernel responsibilities:
- Boot handoff and processor initialisation.
- Exception and interrupt handling.
- Memory inventory and allocation.
- Virtual-memory setup.
- Basic task isolation.
- Minimal system-call interface.
- Emulator console output.

A 1024-bit register bank may create substantial context-save cost. The kernel must know which state is mandatory to preserve and how extension state is handled. Begin with a minimal protected kernel; GUI, networking, SMP, and broad device support are later.
