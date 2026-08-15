# Definitely Secure Studio Lab

Experimental creative-production agents, prompts, validators, and pipelines.

> [!WARNING]
> Everything in this repository is experimental unless explicitly promoted to
> an authoritative repository. Do not use Lab interfaces as production
> contracts or depend on `main` for production behavior.

## Responsibility

`lab` is the public research and development space for creative-production
ideas. It is the authoritative home for experiments, but it is not the
authoritative home for any stable contract or production implementation.

Its scope includes:

- experimental agents and coordination patterns;
- exploratory prompt designs and evaluations;
- prototype validators and policy checks;
- pipeline and orchestration experiments;
- reproducible research fixtures and examples; and
- findings that support a promotion or abandonment decision.

Stable, implementation-neutral contracts belong in
[`codex`](https://github.com/DefinitelySecureStudio/codex). Hardened production
software belongs in
[`platform`](https://github.com/DefinitelySecureStudio/platform). Public
creative canon belongs in `universe`; private or unrevealed world-building
belongs in the private `lore` repository.

The organization-wide ownership model is defined in the
[`studio` repository architecture](https://github.com/DefinitelySecureStudio/studio/blob/main/ARCHITECTURE.md).

## Repository layout

| Path | Purpose |
| --- | --- |
| [`agents/`](agents/) | Experimental agent roles, instructions, and coordination patterns |
| [`prompts/`](prompts/) | Exploratory prompts and prompt evaluations |
| [`validators/`](validators/) | Prototype validation and policy-checking tools |
| [`pipelines/`](pipelines/) | Experimental multi-step production workflows |
| [`experiments/`](experiments/) | Registered hypotheses, methods, results, and decisions |
| [`fixtures/`](fixtures/) | Synthetic, content-safe inputs and expected outputs |
| [`examples/`](examples/) | Minimal public demonstrations of experimental work |
| [`docs/`](docs/) | Experiment lifecycle and promotion policy |

## Content boundary

This repository is public. Do not commit:

- proprietary lore, unrevealed story details, or unpublished canon;
- production prompt instances or context packages containing private material;
- credentials, personal data, confidential communications, or production logs;
- copyrighted third-party inputs without redistribution permission; or
- generated output that reveals private source material through summaries,
  embeddings, caches, snapshots, or evaluation traces.

Experiments, fixtures, examples, screenshots, logs, and recorded outputs must use
synthetic or already-public content. A safe experimental mechanism does not make
its production inputs safe to publish.

## Experiment lifecycle

Every substantial experiment records a hypothesis, success and stop criteria,
method, content classification, reproducible inputs, measurements, findings,
and disposition. Start with the
[`experiment template`](experiments/0000-template.md) and follow the
[`experiment lifecycle`](docs/experiment-lifecycle.md).

## Promotion

Lab work becomes durable only through review in its destination repository:

- promote a stable, implementation-neutral contract to `codex` through its RFC,
  specification, schema, and conformance-fixture process;
- promote a proven implementation to `platform` by hardening or reimplementing
  it with production tests, operations, security, and dependency ownership; or
- promote both by accepting the contract in `codex` before the production
  implementation depends on it.

Promotion is not a Git copy operation, and consumers must not treat Lab paths as
stable dependencies. See [the promotion policy](docs/promotion.md).

## Contributing and security

Read [CONTRIBUTING.md](CONTRIBUTING.md) before proposing work. Report security
vulnerabilities or sensitive disclosures through the private process in
[SECURITY.md](SECURITY.md), not a public issue.

## License

Except where otherwise noted, original work in this repository is licensed
under the [Apache License 2.0](LICENSE). See [NOTICE](NOTICE) for attribution and
important boundaries.

The license does not grant rights to Definitely Secure Studio names, the Prompt
Mark, wordmarks, logos, other brand assets, or proprietary creative material.
Third-party material remains subject to its own terms. Examples and fixtures
must be synthetic, properly licensed, or already public.
