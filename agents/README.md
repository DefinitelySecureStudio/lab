# Agents

Experimental agent roles, instructions, tools, handoff patterns, and evaluation
methods belong here.

Each agent experiment must identify its `EXP-NNNN` record, model and tool
assumptions, allowed inputs, expected outputs, failure modes, and evaluation
method. Agent definitions are not production prompt contracts; stable interfaces
are promoted to `codex`, while hardened execution belongs in `platform`.

The experiment record must also state the responsible human, delegated
authority, prohibited actions, data classes, tool destinations, budget,
duration, monitoring, revocation, escalation, audit evidence, and tested
failure/recovery behavior. Retrieval and tool results are untrusted data.
Agents cannot expand their own scope, approve their own work, create Canon, or
cross an A4 gate without explicit human action.

Use only synthetic or already-public context. Never embed private lore,
unpublished canon, credentials, personal data, or real production context.
