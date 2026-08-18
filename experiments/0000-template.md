# EXP-0000: Experiment title

- Status: Proposed
- Owners: GitHub handles
- Created: YYYY-MM-DD
- Primary area: Agents, prompts, validators, pipelines, or cross-cutting
- Content classification: Synthetic or already public
- Intended destination: None, Codex, Platform, both, or unknown
- Related issues and RFCs: None
- Constitution version: 1.0.0
- Constitution tag: `constitution/v1.0.0`
- Constitution commit: `a9cc8a503aa30e17820edc62ac95f7cbe10e0564`
- Applicable checklist profiles: Universal; agent and automated workflow
- Conformance evidence: Issue, pull request, or restricted attestation

## Hypothesis

State the falsifiable claim or decision this experiment will inform.

## Success and stop criteria

Define measurements, success, failure, resource limits, and when to stop.

## Method

Describe inputs, tools, models, versions, parameters, steps, controls, and the
reproduction procedure without including secrets or private context.

## Delegation and operating bounds

Name the responsible human owner, authority level, permitted and prohibited
actions, data classes, tools, destinations, cost/resource budget, duration,
monitoring, revocation, and escalation path. Authorization and policy checks
must be enforced outside model output.

## Safety and content boundary

Identify data classification, trust boundaries, expected failure modes, and how
outputs will be checked for leakage or unsafe behavior.

## Failure and recovery

Define timeout, provider loss, partial execution, duplicate-action,
containment, rollback, and human-takeover tests. Record tool calls, retries,
failures, transformations, outputs, and approvals without leaking protected
content.

## Results

Record measurements and observations, including negative and inconclusive
results. Link only content-safe artifacts.

## Limitations

Explain what the experiment does not establish and which assumptions may not
hold in production.

## Decision

Choose continue, abandon, or recommend promotion. A promotion recommendation
must name destination issues or RFCs and the work needed to meet their standards.
