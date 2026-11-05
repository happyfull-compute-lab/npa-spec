Events
======

* Software: ``ascend``
* Sync exception: ``edel=1 && exc≠0`` → local ``exc``; else ``ascend(EXCEPTION)``
* IRQ: interrupt-instance vector (async)

``edel`` is parent-owned at create. Fault is a software class of exception,
not a third hardware entry. Delegation ≠ privilege; unauthorized access fails.
