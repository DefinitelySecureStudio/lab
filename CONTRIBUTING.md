# Contributing

Lab contributions should make an uncertain idea easier to evaluate. They are not
a shortcut around Codex change control or Platform production review.

## Before starting

1. Confirm the work is experimental. Stable contracts belong in `codex` and
   production implementation work belongs in `platform`.
2. Search existing experiments and allocate the next `EXP-NNNN` identifier.
3. Copy `experiments/0000-template.md` and define the hypothesis, success and
   stop criteria, content classification, method, and intended disposition.
4. Use only synthetic or already-public inputs and outputs.

Never submit proprietary lore, unpublished canon, production context, secrets,
personal data, confidential communications, or restricted third-party content.
If material may be private, keep it out of Git and ask a maintainer privately.

## Reproducibility expectations

- Pin tools, models, dependencies, and external inputs as precisely as practical.
- Record relevant configuration without committing credentials.
- Separate reusable mechanisms from experiment-specific configuration.
- Store small, content-safe fixtures in `fixtures/`; summarize large or
  nondistributable artifacts with checksums and secure references.
- Record negative and inconclusive findings, not only successful outcomes.
- Define evaluation measures before interpreting results.

## Pull requests

Pull requests must identify the experiment, content classification, validation
performed, limitations, and whether the result should be continued, abandoned,
or considered for promotion. A promotion recommendation must link to destination
issues or RFCs; merging a Lab pull request does not itself promote the work.
