Security
========

Ordinary secure domain
    Isolated from all but root trust; root may read content.

Confidential domain (csec)
    Even root cannot read unless **explicitly exposed** (``ascend(x)`` / share window).

Control vs visibility
    Parent **may** preempt/interrupt; content stays hidden (I27).
    On preempt, parent receives **masked context** (token); security
    subsystem restores true Context on resume (I28).

Keys
    Held by security subsystem; never in DCB Spec; parent has no key.

Interfaces (requirements only): preset, bind, attest, key_set_region,
expose, check_access. Algorithms and root-trust storage are implementation.

secure lib = small/reused address space sec/csec, verify, run, EXIT.
