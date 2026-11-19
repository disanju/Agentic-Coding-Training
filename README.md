# Agentic Coding Training

A workspace for preparing an agentic-coding training task. It will contain the selected open-source codebase, a clearly scoped coding problem, setup instructions, automated verifiers, and reproducible execution instructions.

## Project status

**In progress — repository scaffold only.** The starter files do not yet represent a completed or validated training task.

## Planned structure

```text
.
├── README.md
├── source/
│   └── README.md
├── task/
│   ├── problem.md
│   └── instructions.md
├── verifiers/
│   ├── README.md
│   └── grading-rubric.md
├── docs/
│   ├── codebase-analysis.md
│   ├── environment-setup.md
│   └── testing-guide.md
└── docker/
    └── README.md
```

## Selected source codebase

The current candidate is **Flask**, maintained by Pallets:

- Repository: https://github.com/pallets/flask
- License: BSD-3-Clause (verify the exact upstream license file and retain required notices before redistributing source)
- Why it is a candidate: Python project with an established test suite and a codebase that can be explored by a beginner.

This is a candidate, not yet a final task selection. Before writing the challenge, inspect the upstream repository, its current structure, tests, dependencies, and license.

## Workflow

1. Inspect and document the upstream codebase.
2. Choose one small, precise, useful problem grounded in the code.
3. Write instructions that describe expected behaviour without giving away the implementation.
4. Build independent automated tests (verifiers) for the requirements.
5. Run the tests against the original code and a correct solution.
6. Document exact setup and test commands; add Docker only after the environment is understood.
7. Record evidence of reproducibility and known limitations.

## Important

Do not claim that a verifier passes until it has actually been run. Do not copy an upstream project into this repository without preserving its license and notices. Keep the upstream project and this training-task workspace clearly distinguished.
