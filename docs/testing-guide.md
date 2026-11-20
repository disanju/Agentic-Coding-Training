# Testing guide

## Existing upstream tests

Flask uses pytest. The project configuration sets `tests/` as the test directory and treats warnings as errors.

For the class-based views area, the focused test file is:

```text
tests/test_views.py
```

Once the environment is installed, the focused command is:

```bash
uv run pytest tests/test_views.py
```

The full upstream suite can be run with:

```bash
uv run pytest
```

## Training-task verifiers

The task-specific verifier suite will live in `verifiers/`. It should test only requirements stated in `task/problem.md`.

Before calling the verifier suite complete, check all of the following:

1. It fails against the unmodified baseline for the intended missing behaviour.
2. It passes against a known-correct implementation.
3. It does not rely on a particular implementation detail unless the task explicitly requires it.
4. It covers normal and relevant edge cases.
5. It can be run using documented commands from a clean checkout.

No task-specific verifier has been implemented or executed yet.
