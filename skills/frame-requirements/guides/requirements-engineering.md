# Requirements-Engineering Guide

## Purpose and scope

Develop a requirements artifact that is useful for its agreed purpose, such as informing a solution, enabling review, supporting implementation, or providing a handoff. Requirements may be the final deliverable in their own right.

First determine the intended scope and level of detail. Ask focused questions when an unresolved issue would materially change the requirements. Otherwise, record a clearly labeled assumption or open question and proceed where useful.

Completeness is relative to the agreed scope and purpose. Elicit and organize requirements as thoroughly as warranted, but do not claim that every possible need has been found.

## Elicit and distinguish information

Identify relevant needs, behaviors, constraints, quality attributes, interfaces, and acceptance conditions as appropriate to the task. Do not impose categories that do not help the project.

Clearly distinguish:

- confirmed requirements;
- assumptions awaiting confirmation;
- open questions;
- constraints or dependencies; and
- proposals that have not been agreed.

Identify conflicts, ambiguity, duplication, and requirements that cannot yet be verified. Do not silently resolve substantive conflicts or invent stakeholder agreement.

## Write useful requirements

Write each requirement so it is clear and verifiable to the degree appropriate for its use. Avoid combining unrelated obligations in one requirement. Include measurable acceptance criteria when they can be agreed or derived; otherwise state what remains to be determined.

Assign concise, unique, stable IDs, such as `R-1`, `R-2`. Preserve IDs across revisions where the requirement remains materially the same. Explain changes, replacements, or splits when traceability matters.

When a problem frame exists, reference relevant frame IDs (for example, `P-1`) where this helps explain why a requirement exists. Do not force traceability links that add no value.

Priorities, rationale, source, and verification method may be useful fields, but include them only when they help the agreed purpose. Avoid creating a burdensome specification for a lightweight task.

## Output and quality review

Use a structure appropriate to the size and intended use of the artifact. Before delivery, check that:

- the stated scope is clear;
- requirements are understandable and sufficiently verifiable for their purpose;
- confirmed facts are not mixed with assumptions or proposals;
- material gaps, conflicts, and unresolved questions are visible;
- IDs and relevant traceability references are consistent; and
- the result does not imply unsupported completeness.

## Revisit during solution work

If design, implementation, or testing reveals a material missing requirement, contradiction, or invalid assumption:

1. Identify the evidence and affected requirement IDs, if available.
2. Explain how the issue may affect the current solution or its validity.
3. Propose revisiting the affected requirements and, if the underlying problem may be misunderstood, the relevant part of the problem frame.
4. Ask for a decision when the change affects user intent, scope, priorities, or a consequential tradeoff.

Do not silently treat an unapproved proposal as a confirmed requirement. Preserve valid work where possible, but reconsider decisions that depend on superseded requirements.
