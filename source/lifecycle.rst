Domain lifecycle
================

::

   FREE --descend(first)--> LIVE --ascend(EXIT)--> TERM
      ^                                              |
      +------------- parent reap / reinit -----------+

======  ==================  ==========================
State   descend             transition
======  ==================  ==========================
FREE    first (entry)       create / reap
LIVE    resume (Context)    first descend
TERM    **reject**          ascend(EXIT)
======  ==================  ==========================

DCB placement vs ``task_info`` is an OS choice. Lifecycle is hardware-owned,
not a task-state mirror. Hot path: select DCB object + ``descend(dcb)`` only.
