DCB and Context
===============

Spec Field (10 words / 40 bytes)::

   0x00 sz     parent   size in words
   0x04 id     system   domain id
   0x08 entry  parent   first-PC
   0x0C edel   parent   exception delegation 0|1
   0x10 exc    child    local exception entry
   0x14 irq    system   interrupt handle
   0x18 ipa    parent   address constraint table
   0x1C ptb    child    page-table base (0 = inherit)
   0x20 child  parent   current child DCB
   0x24 sec    system   security group handle

Impdef from 0x28 (e.g. ``isa``).

Context (GPR/PC/SP/flags) is **outside** DCB, ISA-defined.
No ``saved_*`` / ``irq_saved_*`` in Spec.
