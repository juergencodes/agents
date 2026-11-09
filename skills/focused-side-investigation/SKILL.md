---
name: focused-side-investigation
description: Identifies when a subquestion would benefit from a focused, relatively independent investigation and prepares a standalone prompt or delegates it to an available agent when the result can be used directly.
---

# Focused Side Investigation

Use this skill when a question or subtask within a larger conversation may benefit from being investigated in a
separate, tightly scoped context.

## When to suggest an investigation

Consider a side investigation when the subtask:

- is sufficiently self-contained to be handled with little context from the main conversation;
- may benefit from a narrower, less contextually biased, deeper, or independent perspective;
- could meaningfully advance, illuminate, or validate the larger task; and
- is open-ended: a useful outcome may be an answer, a useful perspective, a limitation, or no conclusive result.

Do not suggest one merely because a task can be split. If the subtask is straightforward in the current conversation,
depends heavily on its history, or would not benefit from focused separation, handle it in the main conversation.

## Default: offer a prompt for the user's decision

When an investigation seems worthwhile, normally propose it in the main conversation and include a ready-to-use
standalone prompt. Showing the prompt should let the user judge the scope and decide whether to start the investigation.

Do not start a separate interactive chat on the user's behalf. The user will usually run the prompt manually,
participate in any follow-up discussion, and decide what to bring back to the main conversation.

## When autonomous delegation is appropriate

If the environment explicitly permits launching a separate agent, the task is well-scoped, and its result is expected to
be directly useful in the current work without requiring user participation in the side conversation, the agent may
launch that investigation autonomously.

Use the available delegation mechanism and follow its constraints. Do not claim to have started a separate chat or agent
unless that action actually occurred. If delegation is unavailable or not appropriate, provide the prompt for the user
instead.

## Prompt requirements

Read [guides/prompt-and-handoff.md](guides/prompt-and-handoff.md) when preparing an investigation prompt or integrating
its result. Consult [examples/side-investigation.md](examples/side-investigation.md) when a concrete example would help.

The prompt should:

- state one focused question or task and its intended purpose;
- include the minimum context and definitions needed to work independently;
- distinguish known facts from assumptions and avoid importing irrelevant conversation history;
- request a concise, useful result, including reasoning or sources when relevant;
- explicitly allow the investigator to report uncertainty, limitations, or that no reliable/conclusive result was found;
  and
- say what form of result would be useful to return to the main task.

## Use and return of results

Treat an investigation as exploratory, not as guaranteed to produce a usable answer. Evaluate its result for relevance
and limitations before relying on it. If the user runs the side conversation, let them choose whether and what to bring
back. When summarizing a result into the main conversation, preserve material uncertainty, assumptions, and
disagreements; do not silently present exploratory findings as established facts.
