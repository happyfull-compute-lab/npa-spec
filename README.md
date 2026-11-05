# NPA Spec (Sphinx)

Official **Nested Privilege Architecture** specification (draft v0.3).

## Build

```bash
cd npa-spec
python -m venv .venv && . .venv/bin/activate
pip install sphinx
sphinx-build -b html source _build/html
```

Open `_build/html/index.html`.

Static HTML drafts (same content, ASCII diagrams) are in `source/_static/`.

## Scope

Architecture **requirements** only. Crypto, root-trust storage, and protocols
are implementation choices.

## History

Supersedes `happyfull-compute-lab/rpa-spec` (legacy, keep for research trail).
Name: RPA → NPA (Nested Privilege Architecture).
