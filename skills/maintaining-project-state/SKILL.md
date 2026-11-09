---
name: maintaining-project-state
description: Creates, updates, or consolidates a concise shared project-state document such as state.md so a human and an AI can continue work from a reliable current reference.
---

# Maintaining Project State

Use this skill when creating, updating, reviewing, or handing off a persistent project-state document intended to be
readable by both a human and an AI.

## Core principles

- Keep the shared state concise, clear, scannable, and useful for continuing the work.
- Record the current relevant knowledge, not a chronological transcript or a complete history of activity.
- Consolidate regularly: remove obsolete, duplicated, completed, or superseded information.
- Distinguish confirmed decisions and facts from assumptions, unresolved questions, and proposals.
- Do not claim that information has been saved or that the state is current unless the relevant file or storage has
  actually been checked or updated.
- A task may also use a separate AI workspace for working notes or intermediate material. The shared state and that
  workspace can coexist; keep their purposes clear and do not copy all workspace contents into the shared state.

## Choose the relevant operation

- For creating or structuring a state document, read [guides/structure.md](guides/structure.md).
- For deciding what to add, retain, revise, or remove, read [guides/curation.md](guides/curation.md).
- For examples, consult only the relevant file:
    - [examples/project-state.md](examples/project-state.md)
    - [examples/state-and-workspace.md](examples/state-and-workspace.md)

## Update behavior

When a durable project decision or other confirmed change affects the shared project state, update the state file if it
is available and the task context permits writing. Briefly tell the user what changed.

Do not treat every new message, completed task, or tentative idea as a state change. If it is unclear whether
information is confirmed, durable, or appropriate for the shared state, ask before recording it.

If the state file is unavailable, inaccessible, or cannot be written, say so plainly. You may provide a proposed update,
but do not imply that it was persisted.
