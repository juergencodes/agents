# Example: Shared State and AI Workspace

A project may use both a concise shared state and a more detailed working area. They serve different readers and purposes.

**Shared `state.md`:**

```markdown
## Current status
The migration plan is approved. Implementation has not started.

## Confirmed decisions
- Migrate one service at a time.
- Keep the existing API stable during the migration.

## Open questions
- Confirm the maintenance window for the first service.

## Next steps
- Draft the first service's migration checklist.
```

**Possible AI workspace contents:**

- Comparison notes for migration strategies.
- Intermediate analysis of service dependencies.
- Draft checklist variants.
- Detailed findings and links collected during research.
- Temporary calculations or task-specific working notes.

Only durable decisions, relevant current status, actionable open questions, and necessary next steps belong in the shared state. The workspace may be more detailed and task-specific. If workspace material leads to a confirmed project decision, summarize that decision in `state.md`; do not copy the entire analysis.
