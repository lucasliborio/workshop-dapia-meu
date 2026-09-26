# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project status

`dapia` is a freshly scaffolded Python project (the output of `uv init`): a single `main.py` entry point with a stub `main()`, no dependencies, no tests, and no commits yet. The README and the `pyproject.toml` description are still empty placeholders. Update this file as real structure, tooling, and architecture are added.

## Environment

- Python **3.14** (pinned in `.python-version`; `pyproject.toml` requires `>=3.14`).
- Managed with **uv**. The virtualenv lives in `.venv/` (gitignored).

## Commands

```bash
uv run main.py          # run the entry point
uv add <package>        # add a runtime dependency (updates pyproject.toml + uv.lock)
uv add --dev <package>  # add a dev dependency (e.g. pytest, ruff)
uv sync                 # create/refresh .venv from the lockfile
```

No linter, formatter, or test framework is configured yet. If you add one, document its commands here, including how to run a single test.
