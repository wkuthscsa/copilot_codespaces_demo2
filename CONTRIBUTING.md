## Required tools

The recommended development environment is the checked-in dev container / GitHub Codespaces configuration.

At a minimum, contributors should have:

- R and RStudio or RStudio Server - the CRAN packages required by this code

## Local workflow

1. Read the TODO.md checklist and pick the item that seems to be most important unless directed by your human to a specific item, or add tasks as they are requested or warranted by circumstances

2. Make the smallest change that satisfies the issue.

3. Update documentation and issue state if behavior changed.

## Coding expectations

- Keep repo-wide workflow guidance that applies to both humans and coding agents in this file

- Use AGENTS.md for guidance specifically for Copilot, Codex, and other coding agents.

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

- Use repo-level documents such as this file for shared workflow rules, and keep code-local implementation notes near the code they govern.

## Automated checks

Develop tests to the extent that they are needed, perhaps using testthat

## Task tracking

The canonical backlog should live in TODO.md

## Documentation sync

When you change code, update the relevant documentation in the same branch when any of the following change:

- outputs written by the script

- dependency expectations

- contributor workflow