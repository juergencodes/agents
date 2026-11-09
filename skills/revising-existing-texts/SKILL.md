---
name: revising-existing-texts
description: Revises existing substantial texts either selectively or as a whole. Use when proposing or making changes to an existing text, regardless of whether it was written by the user or an AI.
---

# Revising Existing Texts

Use this skill when changes are requested to an existing, substantial text. The text may have been written by the user or by an AI.

## Choose a revision mode

- **Patch mode:** Make only agreed, localized changes; preserve unaffected content and structure. See [modes/patch.md](modes/patch.md).
- **Revision mode:** Rework the agreed text scope as a whole; structure and wording may change substantially, and existing content may be replaced. See [modes/revision.md](modes/revision.md).

An explicit user instruction determines the mode and scope. Otherwise, use context and text size only as heuristics: a long text may need local edits, while a short text may need a full rewrite. If it is unclear whether the user wants localized changes or a fundamental revision, if the scope is unclear, or if the choice would materially change the result, ask before editing. Do not assume permission for a full revision.

Read only the detail file for the selected mode. Consult an example file only when useful for the requested output:

- Patch examples: [examples/patch-changesets.md](examples/patch-changesets.md)
- Full-revision example: [examples/full-revision.md](examples/full-revision.md)
- Unified-diff example: [examples/unified-diff.md](examples/unified-diff.md)

## Choose an output format

Treat revision mode and output format as separate decisions. Follow any explicit user preference.

- **Changesets:** Identified change proposals without reproducing the entire text.
- **Complete revised text:** The full text after the requested changes.
- **Unified diff:** Changes shown against an exact source version.

If no format is specified, present changesets first in patch mode. In revision mode, provide the complete revised text when a full revision was clearly requested; otherwise ask if the intended scope is unclear. Choose another format only when the request clearly implies it.

Produce a unified diff only when the exact source version is available and the edits can be reliably applied to it. Otherwise, use changesets or the complete revised text, and briefly explain if the requested diff cannot be produced reliably.

## Final check

Before responding, verify that the result follows the chosen mode and agreed scope, that patch-mode changesets and dependencies were applied as selected, and that the output format matches the user's request. Do not make unrequested editorial changes outside the agreed scope.
