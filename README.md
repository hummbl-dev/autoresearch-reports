# Autoresearch Reports

Shared depot for the Autoresearch → distillation → proposal pipeline.

## Pipeline

```
Windows Desktop (Autoresearch)  →  reports/
nodezero (qwen3.5:9b distill)  →  findings/
nodezero (synthesis + draft)    →  proposals/
MBP (human review + merge)      →  applied/
```

## Directory Structure

- `reports/` — Raw Autoresearch markdown output (pushed from Windows Desktop)
- `findings/` — Distilled structured JSON (generated on nodezero)
- `proposals/` — Draft improvement proposals (generated on nodezero)
- `applied/` — Archive of accepted changes (moved after merge)
- `research_queue.json` — Topic queue with recurrence schedules

## Naming Convention

- Reports: `reports/YYYY-MM-DD-domain-query-slug.md`
- Findings: `findings/YYYY-MM-DD-domain.json`
- Proposals: `proposals/YYYY-MM-DD-target-description.md`
