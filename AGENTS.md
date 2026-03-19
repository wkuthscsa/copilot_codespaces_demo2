---
description: "Instructions for coding agents working on this R project"
---

## Coding expectations

- Prefer small, reviewable commits.

- If code behavior changes, update any affected documentation and issue acceptance criteria in the same change.

- Do not commit from a knowingly broken branch unless a human explicitly asks for that override.

- Prefer fixing existing bugs in the touched area before expanding scope with new features.

- Before analyzing, the data should be split into training and testing as per standard practice.

- All libraries and global variables should be at the top of the script

- The script should have a YAML header suitable for automatically compiling to Markdown in RStudio

## R style conventions

- Terminate expressions with semicolons in project R files.

- Prefer descriptive variable names instead of single-character names. For temporary index variables where single letters like 'x', 'y', 'i', 'j', etc. are traditionally used, instead double them, e.g. 'xx', 'yy', 'ii', 'jj'.

- Add a short purpose / input / output comment immediately above each function.

- In larger functions or free-standing code, separate major steps with blank lines and a brief step comment.

- Prefer dplyr pipelines where they improve readability.

- Use repo-level documents such as CONTRIBUTING.md for shared workflow rules, and keep code-local implementation notes near the code they govern.