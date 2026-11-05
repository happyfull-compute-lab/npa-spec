NPA — Nested Privilege Architecture
===================================

**NPA** (formerly RPA) decouples privilege management from fixed ISA levels
into a memory-resident domain tree with two symmetric primitives:
``descend`` and ``ascend``.

This site is the **official specification** (draft v0.3). Implementation
algorithms (crypto, root-trust storage, protocols) are out of scope.

.. toctree::
   :maxdepth: 2
   :caption: Contents

   overview
   naming
   primitives
   lifecycle
   dcb
   events
   memory
   security
   invariants

Status
------

* Theory frozen for implementation probes (see ``npa`` research repo).
* Corrections discovered in pysim/QEMU/gem5 follow: discuss → revise → record.

HTML drafts
-----------

* ``_static/NPA_SPEC_DRAFT.html`` — full draft with diagrams
* ``_static/NPA_SPEC_BRIEF.html`` — one-page summary
