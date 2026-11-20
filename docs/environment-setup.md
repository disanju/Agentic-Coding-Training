# Environment setup

## Requirements

The inspected Flask snapshot requires Python 3.11 or newer. It uses a `pyproject.toml` project configuration and includes a `uv.lock` lockfile.

## Suggested setup

The following commands use `uv` to install the project and its test dependency group from the checked-in lockfile:

```bash
git clone https://github.com/pallets/flask.git
cd flask
git checkout 49943b5a94413a530761350f04e896f76e8d620e
uv sync --group tests
```

Run the existing test suite with:

```bash
uv run pytest
```

Run only the class-based view tests with:

```bash
uv run pytest tests/test_views.py
```

## Validation status

These commands are based on the upstream project configuration. They have not yet been run in a clean environment as part of this task, so they are documented as proposed commands, not verified results.

Record the Python version, uv version, command, exit status, and any relevant output after running them.
