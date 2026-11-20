# Qualification workflow

This document separates the parts of the qualification so that each result can be checked honestly.

## Part 1: Prepare the source project

- Choose an open-source codebase under MIT, Apache-2.0, or BSD-3-Clause.
- Record its repository URL, exact full commit ID, and license.
- Keep a clean copy of the original source for comparison.
- Confirm that the environment and existing tests can be run.

Current candidate: Flask, BSD-3-Clause, commit `49943b5a94413a530761350f04e896f76e8d620e`.

## Part 2: Define and check the coding problem

- Write the task in `problem.txt` using clear, observable requirements.
- Avoid prescribing a particular implementation.
- Check the task against the untouched source.
- Use the Carrot agent to generate or check the verifier tests.
- Review the generated tests for alignment with the stated requirements.

The task and verifier suite are not finalized yet.

## Part 3: Evaluate the coding agent

The qualification workflow distinguishes Carrot (used to prepare/check tests) from Celery (the coding agent being evaluated).

- Start from a fresh copy of the original source when instructed.
- Run the exact task prompt with Celery.
- Preserve the actual transcript and output.
- Run the reviewed verifier tests against the resulting code.
- Record failures accurately. A meaningful failure must be a real missed requirement or reasoning error, not a timeout, service outage, or proxy problem.
- Do not edit or fabricate transcripts, ratings, screenshots, or test results.

## Part 4: Complete the Docker exercise

The Docker Todo exercise is separate from the Flask source project. Use the actual provided Todo starter project, create and test its Dockerfile, and package the files requested by the qualification.

## Submission evidence

Keep the requested files and evidence together. The qualification instructions mention items such as:

- `problem.txt`
- `problem_checker_results.md`
- `da_training_project_tests/`
- the OpenCode configuration and `.opencode/` directory
- the actual Celery run transcript/log
- screenshots of the test results
- the Dockerfile submission ZIP

Check the live qualification instructions before final packaging in case the expected filenames or ZIP layout differ.

## Integrity

Only report actions that were actually performed. Mark planned commands as planned, and record real output after execution. Keep API keys and proxy credentials out of Git.
