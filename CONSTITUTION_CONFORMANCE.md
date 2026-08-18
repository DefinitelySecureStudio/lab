# Constitution conformance record

## Constitutional alignment

- Constitution: [Definitely Secure Studio Constitution v1.0.0](https://github.com/DefinitelySecureStudio/studio/tree/constitution/v1.0.0)
- Constitution tag: `constitution/v1.0.0`
- Constitution commit: [`a9cc8a503aa30e17820edc62ac95f7cbe10e0564`](https://github.com/DefinitelySecureStudio/studio/commit/a9cc8a503aa30e17820edc62ac95f7cbe10e0564)
- Status: `Conforming` (effective only after accountable-owner approval and merge of the adopting pull request)
- Assessed scope: all scaffold files at the assessed revision, including experiment lifecycle, agent/prompt/validator/pipeline guidance, fixtures, promotion boundaries, and repository controls
- Excluded scope: future experiments and executions; no active experiment, agent implementation, external provider, generated artifact, or promotion exists at this revision
- Accountable owner: [`@andrewperis`](https://github.com/andrewperis), Lab maintainer
- Assessment revision and date: `3c8261d0479862a3b70063a59bdcbb2a2ce76731`; 2026-08-17
- Checklist revision: `a9cc8a503aa30e17820edc62ac95f7cbe10e0564`
- Applicable profiles: universal; repository and production-system; agent and automated-workflow
- Evidence: this record; repository files at the assessed revision; GitHub settings verified 2026-08-17; adoption issue [#3](https://github.com/DefinitelySecureStudio/lab/issues/3); adopting pull request
- Active constitutional exceptions: None
- Residual risk: the repository contains policy and templates but no executed experiment; every future consequential run needs its own evidence and human approval
- Next review: 2026-11-17, or before the first consequential experiment/promotion and on Constitution, agent capability, provider, data class, tool, destination, authority, owner, visibility, or security-boundary change

Before merge this proposal remains `Transition required`. Owner review and
merge provide A4 governance approval and record the adopting commit. Sensitive
run evidence, if later needed, stays restricted; only a non-derivable,
reader-safe attestation belongs here.

## Findings

| ID | Severity | Disposition | Evidence |
| --- | --- | --- | --- |
| LB-1 | Major | Resolved in adopting change | The experiment and agent guidance now require explicit delegation, external policy enforcement, audit evidence, and failure/recovery tests. |
| LB-2 | Major | Resolved 2026-08-17 | Secret scanning, push protection, vulnerability alerts, and Dependabot security updates were enabled. |
| LB-3 | Minor | Resolved 2026-08-17 | Undocumented Projects was disabled. |
| LB-4 | Advisory | Deferred by scope | No active experiment exists; run-specific safety, reproducibility, and provider evidence must be assessed before execution. |

## Checklist evidence

`P` means Pass and `N/A` has the stated rationale. IDs follow the pinned
checklist order.

### Assessment identity

| ID | Result | Evidence or rationale |
| --- | --- | --- |
| I1 | P | Identity, base revision, public experimental environment, audience, scope, and exclusions are exact. |
| I2 | P | Version, immutable tag, full commit, and checklist revision are pinned. |
| I3 | P | `@andrewperis` is accountable owner/CODEOWNER; automation proposes and the human reviews and merges. |
| I4 | P | Profiles, evidence, date, freshness, status, findings, and triggers are recorded. |
| I5 | P | Public evidence is reader-safe; sensitive evidence must use a restricted attestation. |

### Universal profile

| ID | Result | Evidence or rationale |
| --- | --- | --- |
| U1 | P | README, experiment records, CODEOWNERS, and promotion policy identify authorities, inputs, and owners. |
| U2 | P | Lab owns experiments only and cannot redefine Studio, Codex, Platform, Canon, or Lore authority. |
| U3 | P | Updated templates require explicit data, tool, time, cost, capability, and escalation bounds. |
| U4 | P | Activation/promotion requires maintainer review; agents cannot self-approve or cross A4 gates. |
| U5 | P | Stop criteria, uncertainty, limitations, unexpected risk, and escalation are required. |
| U6 | P | Proposed, Active, Concluded, Promoted, Abandoned, and Archived are explicit and are not Canon states. |
| U7 | P | README assigns public Canon to Universe and private Lore to Lore. |
| U8 | N/A | Lab cannot perform Canon promotion, correction, deprecation, or retcon. |
| U9 | P | Only synthetic/already-public data is permitted; private Lore/context is prohibited. |
| U10 | N/A | No creative generation run exists at the assessed revision. |
| U11 | P | Experiment template requires inputs, tools, models, versions, parameters, transformations, results, humans, and approvals. |
| U12 | P | Results separate measurements, negative/inconclusive findings, limitations, and interpretation. |
| U13 | P | Reproducibility expectations require precise pins and honest limitations. |
| U14 | N/A | No selected generated output or released bytes exist. |
| U15 | P | Git history plus experiment records and updated audit fields preserve attributable, ordered evidence. |
| U16 | P | Safety sections require classification, trust boundaries, failure modes, resource bounds, and owners before activation. |
| U17 | P | Public synthetic inputs, bounded tools/destinations, and least-privilege delegation minimize processing. |
| U18 | P | README, CONTRIBUTING, SECURITY, fixtures, and templates prohibit secrets everywhere. |
| U19 | P | Classification applies to inputs, outputs, logs, fixtures, screenshots, caches, and traces. |
| U20 | P | A future provider must be pinned and reviewed within the experiment's delegation and data bounds. |
| U21 | P | CONTRIBUTING requires exact third-party provenance, permission, compatible terms, and notices. |
| U22 | P | Questionable provenance, leakage, rights, or security stops the public experiment and uses private escalation. |
| U23 | P | Hypothesis, measures, success/failure, and stop criteria precede results. |
| U24 | P | Automated validators are experimental bounded predicates; humans decide interpretation and promotion. |
| U25 | P | Durable experiment records have stable IDs, Git history, content-safe artifacts, checksums, and destination-owned promotion. |
| U26 | P | Lab provider assumptions are experimental and cannot become durable dependencies without Codex/Platform review. |
| U27 | P | Promotion is destination-owned, preserves lineage, and forbids copy-based migration or implicit dependency. |

### Repository and production-system profile

| ID | Result | Evidence or rationale |
| --- | --- | --- |
| R1 | P | README, architecture, CODEOWNERS, LICENSE, and NOTICE define public experimental responsibility and prohibited content. |
| R2 | P | Protected `main`, CODEOWNER review, private reporting, and enabled security protections match the standard; no dependencies/releases exist. |
| R3 | P | Consumers cannot depend on Lab; promotion records lineage and creates destination-owned immutable artifacts. |
| R4 | P | Every fixture, example, prompt, result, and log must be synthetic or already public. |
| R5 | P | This file is the required declaration. |

### Agent and automated-workflow profile

| ID | Result | Evidence or rationale |
| --- | --- | --- |
| G1 | P | Updated experiment template names identity, owner, authority, actions, data, tools, destinations, budgets, duration, monitoring, and revocation. |
| G2 | P | Updated agent policy treats retrieval/tool results as untrusted and requires enforcement outside model output. |
| G3 | P | Agent guidance forbids self-expansion, self-approval, concealed uncertainty, Canon claims, and A4 crossings. |
| G4 | P | Updated failure/evidence section covers calls, retries, failures, context, transformations, outputs, and approvals without leakage. |
| G5 | P | Updated template requires timeout, provider loss, partial/duplicate action, recovery, rollback, containment, and takeover tests. |

### Assessment outcome

| ID | Result | Evidence or rationale |
| --- | --- | --- |
| O1 | P | LB-1 through LB-4 are classified; no unresolved Blocker or Major remains in scope. |
| O2 | P | Effective status is exactly `Conforming`; pre-merge status remains `Transition required`. |
| O3 | P | Approval covers the base revision and exact adoption diff only. |
| O4 | P | Date and material triggers are explicit. |

## Approval

The owner approves this assessment by reviewing and merging the adopting pull
request. Future experiments cannot inherit run-level conformance from this
repository-scoped record.
