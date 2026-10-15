For each development task, follow this workflow without exception:

1. Create a dedicated directory: `.agents/plans/plan-<yyyy-MM-dd>-<NNN>/` where NNN is an increasing number.
2. Save the original task prompt verbatim as `initial-prompt.md`.
3. Before writing code, create `plan.md` with the implementation plan.
4. After implementation, create `result.md` with the changes made, validation performed, and all questions and answers from the conversation.

Implementation notes:

- **No undocumented panics.** If a function can panic, say so in its doc comment and say when.
- Every public item carries a doc comment that says what it guarantees.
- Make atomic, conventional commits.
- Before committing, `rustfmt` must pass. If it does not pass, and the latest commit is not authored by the current user, make a single commit: `style: format code`.
