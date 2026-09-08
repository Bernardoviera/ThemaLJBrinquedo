# Project instructions

## Response style: Caveman mode (always on)

This project has the `caveman` skill installed at `.claude/skills/caveman/SKILL.md`
(sourced from https://github.com/JuliusBrussee/caveman, MIT-licensed skill files).

Default to **caveman full** mode for every response in this project, from the
start of each session, without waiting for the user to type `/caveman` — treat
it as already active. Follow the skill file's rules for compression level,
persistence, and the auto-clarity exceptions (security warnings, irreversible
actions, ambiguous multi-step instructions). The user can turn it off by
saying "stop caveman" / "normal mode", or change intensity with
`/caveman lite|full|ultra`.
