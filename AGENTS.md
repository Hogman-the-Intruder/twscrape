# AGENTS

This repository contains the **twscrape** library and its tests.
These instructions describe how automated agents should work with the
project.

## Environment
- Python ≥3.10
- Install development dependencies before running checks:
  ```bash
  pip install -e .[dev]
  ```

## Workflow
1. **Lint & Format**
   - Run `make lint` to apply import sorting, format with `ruff`,
     perform linting, and run `pyright` type checks.
2. **Tests**
   - Run `make test` to execute the full test suite with coverage
     using `pytest`.
3. You may also run both steps at once with `make check`.

## Code Style
- Formatting and linting is handled by `ruff` with a line length of 99
  characters and `E501` ignored.
- Type checking uses `pyright`.

## Additional Notes
- Source code lives in the `twscrape/` directory and tests in `tests/`.
- When modifying code, prefer adding or updating tests to cover the change.

