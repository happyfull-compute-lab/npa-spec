# NPA Spec (Sphinx)

Official specification for **Nested Privilege Architecture (NPA)**
(draft v0.3). Formerly named RPA (Recursive Privilege Architecture).

## Build

```bash
cd npa-spec
python -m venv .venv && . .venv/bin/activate
pip install sphinx
sphinx-build -b html source _build/html
```

Open `_build/html/index.html`.

Static HTML drafts with ASCII diagrams live in `source/_static/`.

## Scope

This repository defines architecture **requirements** only:
primitives, DCB, events, address views, security model and interfaces.
Cryptographic algorithms, root-trust storage, and wire protocols are
implementation choices.

## Author

Paper and documentation signature: **Arthur Dev**.

## History

Supersedes `happyfull-compute-lab/rpa-spec` (legacy, archived for the
research trail). Keep old RPA names only in historical notes.

---

This work was completed with AI assistance.
