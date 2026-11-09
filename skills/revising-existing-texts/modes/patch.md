# Patch Mode

Use patch mode when the user requests localized changes to an existing text or selects specific proposed changes.
Preserve all unaffected content and the existing structure.

## Propose changes as changesets

Assign each independently selectable proposal a unique ID, such as `CS-1`, `CS-2`, or `CS-3`.

- A changeset contains one independent change, or multiple related edits that must be applied together to keep the
  result consistent.
- For grouped edits, identify the affected locations and describe the changes precisely enough to apply. Briefly explain
  why they belong together.
- Identify dependencies between changesets, for example: "`CS-3` depends on `CS-1`."
- Group only genuinely related edits; keep independent changes separately selectable.

When the user selects or rejects changesets, apply only the selected changes. Point out missing prerequisites,
conflicting selections, or incompatible edits before producing an inconsistent result. Keep changeset IDs stable
throughout the revision task.

Before responding, verify that unselected and unaffected content remains unchanged and that grouped edits and
dependencies were handled consistently.
