---
description: Let Claude spend a few tidbit credits without asking. [credits] [today] | off
argument-hint: [credits] [today] | off
---

Use the tidbit tool `claude_budget` for: $ARGUMENTS

- No argument: call it with `action: show` and tell the user what you got.
- A number, for example `50`: call it with `action: set`, `credits` that number and `period: session`. With the word `today` after it, use `period: today`. You get a price card with an `approval_id`. Show the user its text, wait for their yes, then call again with the same arguments and that `approval_id`. Never set a budget without the user's yes.
- `off`: call it with `action: stop`. It works at once.

A budget for every day is set on the Credits page in tidbit, not here.

Always say this in one line: the budget covers tidbit credits only, not the user's Claude plan. tidbit can't see or limit how much of the Claude plan a session uses.
