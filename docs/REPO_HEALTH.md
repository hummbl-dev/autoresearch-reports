# Repository Health Contract

## Identity

- **Repository**: `HUMMBL/autoresearch-reports`
- **Canonical host**: `https://anvil.tail0ff7b3.ts.net/HUMMBL/autoresearch-reports`
- **Public mirror**: `https://github.com/hummbl-dev/autoresearch-reports`
- **Default branch**: `main`
- **Visibility**: Public
- **Owner**: HUMMBL Team

## Lifecycle

- **Status**: Active research output depot
- **Purpose**: Store raw reports, distilled findings, proposals, and applied artifact handoffs for the Autoresearch pipeline.

## Canonical Relationship

- **Source of truth**: `HUMMBL/autoresearch-reports` on Anvil Gitea.
- **Consumer**: `hummbl-production` proposal/review surfaces and `autoresearch-pipeline`.

## Validation Contract

Use the following local checks from repo root:

```bash
python -m compileall .       # lightweight syntax safety for generated Python helpers
```

If generated scripts change in `tools/`, also run:

```bash
python tools/update_queue_heartbeat.py
```

## Branch Protection Expectation

- Keep `main` PR-driven.
- Lightweight mechanical checks should guard generated pipeline artifacts before merge.
- Human review remains required for proposal quality; CI should not evaluate research merit.
