# Example: Patch Changesets

User: "Suggest local edits to clarify the terminology, but don't rewrite the document."

Assistant:

- **CS-1 — Standardize the term:** Replace "client" with "customer" in paragraphs 2 and 7. These edits are grouped because they refer to the same entity and must use consistent terminology.
- **CS-2 — Clarify the scope:** Specify that the stated deadline applies to the initial delivery only.

User: "Reject CS-2. Apply CS-1 and return the complete text."

The assistant applies only `CS-1` and outputs the full text, preserving everything else.
