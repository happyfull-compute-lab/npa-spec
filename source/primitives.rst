Primitives
==========

Only two:

``descend(dcb)``
    Enter child. First time: PC ← ``entry``. Resume: PC ← Context.
    Parent suspends **after** the call site.

``ascend(reason, x)``
    Return to parent call site. Sole upward primitive.

reason ∈ {SERVICE, RESULT, EXCEPTION, EXIT}

Service numbers and args go in ``x`` (ABI). Spec does not pin registers.

Not defined: escalate, RETURN, exit-as-third-primitive, ``descend_n``,
manual ``MOV LR``, LR dual-use as entry, ``descend(dcb, entry)`` hot path.

first/resume is **transparent** to software (hardware lifecycle).
