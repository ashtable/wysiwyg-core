# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project state

This is a freshly-scaffolded Python 3.13 project managed with [uv](https://docs.astral.sh/uv/). At present it contains only `main.py` (a hello-world entrypoint), an empty `pyproject.toml` (no dependencies, no build backend, no script entrypoints), and `uv.lock`. There is no `src/` package, no tests, no linter config, and no CI. The README is a single line.

The repo was originally a Rust library (`41d707f Created new Rust lib project`) and was switched to a Python scaffold in `0b661b3`. Any architecture decisions still need to be made — there is no "big picture" to preserve yet.

## Commands

- Run the app: `uv run main.py`
- Add a dependency: `uv add <pkg>` (then commit `pyproject.toml` and `uv.lock` together)
- Sync the environment to the lockfile: `uv sync`

There are no test, lint, or build commands configured yet. If the user asks you to run tests/lint, ask which tool to wire up (e.g., `pytest`, `ruff`) rather than guessing.
