# CLAUDE.md

## Code style

- Write the minimum code that solves the task. Do not add abstractions "for the future".
- No new dependencies without explicit approval.
- Comments explain only "why", never "what". Maximum 2 lines. If code needs a "what it does" comment — rewrite the code so it is self-evident.
- Leave no commented-out code, no console.log, no debugging artifacts, no TODO without a ticket.
- CSS Modules use the `styleName` attribute, not `className`; the css file sits next to its component.
- User-facing text goes through i18next only; the key set is identical across every language in `config/locales/`.

## Workflow

- Before editing, name the files you are going to change and give a 2–4 point plan.
- Keep edits surgical: change only what the task requires. Do not reformat or "improve" neighbouring code unless asked.
- DO NOT WRITE TESTS until the user has explicitly approved the implementation (the /tests command, or the words "implementation approved"). This rule outranks any habit of "cover it with tests right away".
- After the implementation is approved: /finalize first, then /tests.
