# Agentic Coding Training

This repository is the working area for a coding-agent evaluation task built around the Flask project.

## Selected codebase

- Project: Flask
- Upstream repository: https://github.com/pallets/flask
- License: BSD-3-Clause
- Inspected upstream commit: `49943b5a94413a530761350f04e896f76e8d620e`
- Python requirement at that commit: Python 3.11 or newer

The upstream project is kept separate from this task workspace. See [source/UPSTREAM.md](source/UPSTREAM.md) for provenance and license notes.

## Repository layout

- `source/` — upstream source details and checkout instructions.
- `task/` — the problem statement and instructions given to a coding agent.
- `verifiers/` — independent tests and the grading rubric.
- `docs/` — codebase notes, setup, and test instructions.
- `docker/` — notes for the separate Docker exercise.

## Current status

The source snapshot and the class-based views area have been inspected. The task itself is not finalized yet. No verifier suite has been run, and no agent result is being represented as complete.

The next project milestone is to choose a concrete behaviour to change, write a precise problem statement, and verify that the tests distinguish the original behaviour from a correct implementation.

## Working principles

- Keep the task small enough to understand and reproduce.
- Preserve upstream copyright and license notices when redistributing source.
- Test the original code before claiming that a verifier detects a missing behaviour.
- Keep actual test results and agent evaluation evidence separate from plans or examples.
- Record commands and outcomes accurately, including failures.

## Upstream references

- [Flask on GitHub](https://github.com/pallets/flask)
- [Pinned source commit](https://github.com/pallets/flask/tree/49943b5a94413a530761350f04e896f76e8d620e)
