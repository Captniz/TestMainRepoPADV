# Common code

The shared code for the Advanced Programming course project, A.Y. 2026/2027.

The specification this code implements is the **Protocol document** (shared types, geometry, messages...).

## Rules for code in this repository

These are the project's coding principles, and here they are enforced rather than encouraged.

- **No `unsafe`.**
- **No undocumented panics.** If a function can panic, say so in its doc comment and say when. Most things in here should not panic at all.
- Every public item carries a doc comment that says what it guarantees.
- **rustfmt.** Configure your editor.
- Before committing, `cargo fmt --all` must pass. If it does not pass, and the latest commit is not authored by the current user, make a single commit: `style: format code`.
