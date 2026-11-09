# Preparing and Using a Side-Investigation Prompt

## Keep the scope focused

The prompt should be self-contained but not reproduce the main conversation. Include only the context necessary to answer the chosen question. Prefer one well-defined question over a broad request to solve the entire parent task.

State the purpose of the investigation, relevant constraints, and any terms that might otherwise be ambiguous. If an independent perspective is desired, do not include the main conversation's preferred answer or framing unless it is necessary evidence; doing so may bias the investigation.

Ask for the form of output that will help the parent task, such as a short assessment, alternatives with tradeoffs, a validation, or explicit reasons the question cannot be resolved. Do not imply that a conclusive answer is required.

## Decide how to run it

- For a user-run separate chat, provide the complete prompt in a copyable block and let the user decide whether to start it.
- For an available autonomous agent, delegate only when the environment permits it and the result can be used directly without interactive user involvement in that side conversation.
- If separate execution is not available, do not simulate it by pretending the context is independent. Offer the prompt or explain the limitation.

## Integrate cautiously

When a result is returned to the main conversation:

- identify its conclusion and the relevant support;
- preserve caveats, assumptions, disagreements, and unresolved questions;
- distinguish investigation output from confirmed project decisions;
- use only the parts relevant to the parent task; and
- allow a no-result outcome to remain no result rather than forcing a conclusion.

The user controls what is copied back from a manually run side conversation. Do not require the full transcript; a concise summary or selected findings may be enough.
