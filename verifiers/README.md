# Verifiers

Verifiers are independent checks that decide whether a submitted change meets the task requirements.

They should:
- test externally observable behaviour rather than a particular implementation;
- include normal cases, boundary cases, and relevant regressions;
- fail on the unmodified baseline when the task describes missing behaviour;
- pass on a known-correct implementation;
- run deterministically with documented commands.

No verifier has been implemented or run yet.
