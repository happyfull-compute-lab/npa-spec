Invariants
==========

I1–I2  upward only ``ascend``; parent resume = after ``descend``
I3/I18 entry is not return point; single ``descend(dcb)`` form
I4     Spec free of saved_*/ABI fields
I11–I12  ptb=0 tightens only; pure INHERIT not wider than parent
I13–I14  edel=0 always ascends; overreach always fails
I15    naming vocabulary (id / parent-child / δ)
I16–I17  bind checks absolute id; TERM rejects resume
I19–I20  no task_info in Spec; no bulk DCB rewrites on hot path
I21–I24  lazy memory; bind chain; key ownership; keys out of Spec
I25–I26  csec hidden from root; secure lib is small sec/csec
I27–I28  preempt allowed, snoop denied; masked context for csec
