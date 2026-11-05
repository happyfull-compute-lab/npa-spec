Address views (lazy)
====================

======  ======  =============================  ================
ptb     ipa     translation                    ipa check
======  ======  =============================  ================
0       0       inherit parent                 none
0       ≠0      inherit + permission overlay   VA
≠0      *       stack chain to PA              parent-view addr
======  ======  =============================  ================

Every access: translate → ipa → confidentiality/keys → allow.
Cache/TLB may accelerate page-table hits but **must not** change semantics.
