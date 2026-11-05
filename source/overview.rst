Overview
========

NPA (Nested Privilege Architecture) models privilege as a **domain tree**:

* Relative perspective uses **δ** (self = 0, child = +1, parent = −1).
* Absolute identity uses **domain id** (security anchor, not privilege rank).
* Control transfer is **call/return**: ``descend(dcb)`` / ``ascend(reason, x)``.

Principles
----------

======  ==========================  ============================================
P1      Minimal concept set         no cockpit unless distinction helps software
P2      One name, one meaning       no dual names
P3      Separation                  DCB ≠ Context ≠ ABI ≠ task_info
P4      Recursive view              no absolute privilege levels in the ISA story
P5      ISA independent             no register/EL/Ring names in Spec
P6      Executable first            probes may falsify theory
======  ==========================  ============================================

Meta-principle: guidance yields to implementation; discuss and revise on clash.
