# Experiment lifecycle

## 1. Propose

Allocate an `EXP-NNNN` identifier and define a falsifiable hypothesis, measures,
success and stop criteria, content classification, resource bounds, and likely
destination. A proposal must be safe to discuss in public.

## 2. Activate

Receive maintainer review, establish reproducible inputs and configuration, and
confirm that fixtures and expected outputs are synthetic or already public.
Pin dependencies, tools, and models as precisely as practical.

## 3. Run and record

Keep methods and results together. Record failures, negative findings, changes
to method, limitations, and unexpected risks. Raw runs and large artifacts stay
out of Git; commit content-safe summaries, checksums, and secure references when
needed.

## 4. Conclude

Compare results with the predeclared criteria. Choose one disposition:

- **continue** with a revised or follow-up experiment;
- **abandon** and record why the approach should not proceed;
- **promote to Codex** as a candidate stable contract;
- **promote to Platform** as a candidate production implementation; or
- **promote to both**, with the Codex contract accepted before Platform depends
  on it.

## 5. Archive or promote

Preserve the experiment record and link the destination work. Do not rewrite the
record to resemble a stable specification or supported implementation. The
destination repository decides whether promotion is accepted.
