# SparsePrimingRepresentations migration plan v26.11.16

Standing: UNVERIFIED

## Identity
- path: /Users/sac/SparsePrimingRepresentations
- remote: https://github.com/seanchatmangpt/SparsePrimingRepresentations.git
- branch@sha: main@4283aab (tracks origin/main)
- last commit: 2026-09-16; commits: 25; size: <1 MB
- languages/build: Python script (sprtool.py), no build system detected
- nested repos: none

## Observed state
- dirty: 0; untracked: 4 (`__pycache__/`, `docs/`, `tests/__pycache__/`)
- ahead/behind origin/main: 0/0; stash: 0
- unpushed local branch: `exp/spr-validator@2185f1d` (already merged into main)
- build/dep dirs: none; submodules: none
- NOTE: `docs/` is untracked — contains `docs/jira/v26.9.19/` (uncommitted catalogue docs)

## What it is
Fork of the Sparse Priming Representations research repo (prompt-compression technique for
LLMs) plus Sean's `sprtool.py` SPR parser/validator/renderer added in Sep 2026.

## Classification
WARM (census agrees: pushed, last touched 2026-09-16, small experiment).

## Migration risk
- untracked `docs/jira/v26.9.19/` would be lost if not committed
- `exp/spr-validator` is merged, so nothing unique there
Rate: LOW

## Recommended action
COMMIT-PUSH
1. `cd /Users/sac/SparsePrimingRepresentations && git add docs && git commit -m "docs: jira v26.9.19 + v26.11.16"`
2. `git push origin main`
3. `rm -rf __pycache__ tests/__pycache__`
4. DECISION: delete merged `exp/spr-validator` branch or `git push origin exp/spr-validator`.
5. On new machine: clone fresh (step 7); do not rsync this directory.

## First commands on the new machine
`git clone https://github.com/seanchatmangpt/SparsePrimingRepresentations.git && cd SparsePrimingRepresentations && python3 -m pytest tests`

## See Also
- ../v26.9.19/
- /Users/sac/docs/jira/v26.11.16/README.md
