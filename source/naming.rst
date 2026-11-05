Naming
======

=======  ======  ==========  =========================================
Concept  Notation  Chinese   English
=======  ======  ==========  =========================================
Absolute identity  ``id``   域 ID      domain id
Current            ``self``  当前域     self
Tree links         ``parent`` / ``child``   父域 / 子域
Relative depth     ``δ``     相对层差   relative depth
Root               ``root``  根域       root domain
=======  ======  ==========  =========================================

**Forbidden:** Domain 0/1/−1; ordering by id; using δ for security identity.

Identity is ``id``; relations are parent/child; recursion is ``δ``.
