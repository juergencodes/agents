# Example: Requirements

The example derives requirements from problem aspects `P-1` and `P-2` in a problem frame. The requirements are illustrative, not claims about validated stakeholder needs.

## Confirmed requirements

- **R-1 — Find current event details** (related to `P-1`): A coordinator must be able to identify the current time and location for an event from its designated source of truth.
  - **Acceptance criterion:** A coordinator can locate the current time and location for a selected event without consulting a separate chat history.
- **R-2 — Notify volunteers of changes** (related to `P-1`, `P-2`): When event details change, the coordinator must be able to communicate the updated details to affected volunteers.
  - **Acceptance criterion:** A volunteer receiving the update can identify what changed and which event it concerns.

## Assumptions

- **A-1:** Coordinators are authorized to update event details. This needs confirmation.

## Open questions

- **Q-1:** Which channels must be supported for notifications?
- **Q-2:** What response or attendance information do coordinators need to manage?

The IDs support discussion and tracking. The open questions prevent the illustrative requirements from being mistaken for a complete or approved specification.
