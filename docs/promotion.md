# Promotion policy

Promotion converts evidence from an experiment into work governed by the
destination repository. It does not make the Lab artifact authoritative.

## Readiness checklist

Before recommending promotion, the experiment must provide:

- a concluded hypothesis and reproducible method;
- success, failure, and limitation evidence;
- synthetic fixtures and an explicit content classification;
- identified owners and affected consumers;
- security, privacy, and operational risks; and
- links to destination issues or RFCs.

## Promotion to Codex

Use this path when the durable result is an implementation-neutral contract,
schema, naming rule, taxonomy, prompt contract, manifest, context-package
specification, or asset convention.

1. Open a Codex RFC or contract-change issue.
2. Restate the result as normative behavior rather than prototype behavior.
3. Remove experimental implementation details and all private or story-specific
   content.
4. Add semantic versioning, compatibility analysis, schemas, and valid/invalid
   conformance fixtures.
5. Link the accepted RFC and released contract from the experiment record.
6. Record the exact Lab commit as historical promotion lineage. Consumers depend
   on the released Codex bundle, never on that Lab commit or branch.

## Promotion to Platform

Use this path when the durable result is production software or an operational
capability.

1. Open a Platform implementation issue and identify any Codex contracts.
2. Reimplement or harden the prototype with production architecture, tests,
   observability, failure handling, dependency ownership, and security review.
3. Replace experimental configuration and fixtures with approved runtime input
   mechanisms; never copy private production data through Lab.
4. Link the released implementation from the experiment record.
5. Record the exact Lab commit as historical lineage. The production artifact
   is owned, versioned, packaged, and released by Platform.

## Promotion to both

When a result needs both a shared contract and an implementation, Codex accepts
and versions the contract first. Platform then implements a pinned contract
version. Lab must not become an implicit dependency between them.

## Rejected shortcuts

- Consumers must not import or vendor Lab paths as stable dependencies.
- Copying files without destination review is not promotion.
- Merging an experiment does not guarantee it will be promoted.
- A successful result does not waive content, security, licensing, or production
  readiness review.
- A Lab tag, commit, archive, package, submodule, or copied path is never a
  stable production dependency. Promotion creates new destination-owned work.
