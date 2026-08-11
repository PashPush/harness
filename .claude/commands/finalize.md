---
description: Implementation approved — clean up the diff, run lint, summarize
---

Implementation approved. Finalize it:

1. Review the full diff of the current work (`git diff`, and `git diff <base>` if needed).
2. Ask yourself: "If I were writing this from scratch, already knowing the final solution — what would I write?" Bring the code to that state: remove leftovers from intermediate iterations, redundant state, duplication, unused imports and variables, dead code, debug output.
3. Check every comment in the diff: does it explain "why"? is it under 2 lines? Otherwise delete or shorten it.
4. Run typecheck and lint (commands from CLAUDE.md) and fix what they report.
5. Show the final diff and a 2–3 line summary of the changes.

Do not add new functionality at this step. Do not write tests.
