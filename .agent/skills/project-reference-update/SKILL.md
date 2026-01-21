---
name: project-reference-update
description: Keep PROJECT.md updated with significant project progress
---

# Project Reference Update Skill

## When to Update PROJECT.md

Update `/Users/qamarularifinbinabdmanan/Development Work/medication-snapshot/PROJECT.md` whenever:

1. **Phase completion** - A major phase (Planning, Setup, Implementation) is finished
2. **Key decisions made** - New stakeholder decisions are confirmed
3. **Sprint completion** - At the end of each sprint
4. **Architecture changes** - Significant technical decisions change
5. **Scope changes** - Features added/removed from v1
6. **Status changes** - Current phase or next step changes

## What to Update

| Section | When to Update |
|---------|----------------|
| Key Decisions | New decisions confirmed with stakeholder |
| Critical Requirements | Scope changes |
| Out of Scope | Features deferred or added |
| Current Status | Every significant milestone |
| Update Log | Every update session |

## Update Process

1. Edit the relevant section(s) in PROJECT.md
2. Update the "Current Status" section with phase/next step
3. Add entry to "Update Log" with date and summary
4. Commit and push to GitHub

## Reminder

Always commit PROJECT.md changes with a descriptive message like:
```
git commit -m "Update PROJECT.md: [brief description of changes]"
```
