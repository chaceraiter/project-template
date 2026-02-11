# Current Context for New Chat

This meta folder mirrors the template structure and captures project-template-specific build notes and WIP plans.

## Current State

- The reusable template lives in `ai-context-management/` and should stay generic.
- This meta mirror lives in `project-template-build-out-meta-wip/.ai-context/` and is where we track build/process notes and future improvements.
- The targeted instruction/procedure backlog (items 1-6) was completed in the template on 2026-02-11.
- Main system-doc updates from the template were mirrored into this meta folder on 2026-02-11 (orientation/stale flows, human usage docs, export docs, and past-chat-record process docs).
- `current-work/` and `project-setup/` remain intentionally meta-specific instead of fully mirrored.

## Resolved Pain Points (Completed 2026-02-11)

- **Triple-option new chat onboarding was incomplete:** New-chat orientation now explicitly supports all three cases:
  - Brand-new repo + new AI context system
  - Existing repo + new AI context system
  - Existing repo + existing AI context system, but new chat (context-rot reset)
- **Relative path ambiguity caused wrong folder placement:** Instructions now use anchored `ai-context-management/...` paths and explicit root-folder guardrails.
- **Long-chat drift:** Proactive context-maintenance reminders were added so agents keep using the system during long sessions.

## Backlog Record (Completed)

1. **Stale chat procedure:** Completed in template.
2. **New chat entrypoint assumptions (A/B/C):** Completed in template.
3. **Update cadence emphasis + proactive reminders:** Completed in template.
4. **“Start fresh” automation with explicit git confirmations:** Completed in template.
5. **Chat export + past-chat-record procedures:** Completed in template.
6. **Path safety hardening:** Completed in template.

## Current Plan

- Keep implementation in the reusable template (`ai-context-management/`) and keep build/process tracking in this meta mirror.
- Keep meta status files current.
- Continue selective mirroring of shared system docs when template behavior changes, while preserving meta-specific tracking/project content.

## Possible Future Features

1. **Instruction self-test harness:** Add prompt-in/expected-behavior tests for core flows (A/B/C onboarding, stale-chat A/B gate, and root-folder guardrails).
2. **Template versioning:** Add `VERSION.md` and `CHANGELOG.md` under `ai-context-management/` so downstream projects can adopt updates safely.
3. **Context health-check script:** Add an automated check for missing required files, unresolved TODO placeholders, and ambiguous path references.
4. **Canonical scenario playbooks:** Add concrete end-to-end examples for the three onboarding scenarios to reduce agent interpretation drift.
5. **Agent drift recovery prompt:** Add a standard recovery/reset prompt when long chats stop using context files proactively.
6. **Update cadence SLA:** Define explicit minimum update cadence rules (for example, after major changes and periodically during long sessions).

## Progress Updates

- **2026-02-11:** Backlog item 1 completed in template. `ai-agent-stale-chat-procedures.md` now includes an explicit hard gate to ask A/B first and avoid any additional reading/actions until the user chooses.
- **2026-02-11:** Backlog item 2 completed in template. `ai-agent-orientation-start-here.md` and `paste-this-into-new-ai-chats.txt` now enforce explicit A/B/C onboarding triage, including the "existing repo + existing context system + fresh chat" case.
- **2026-02-11:** Backlog item 3 completed in template. Added proactive context-maintenance cadence rules to `ai-agent-orientation-start-here.md` and replaced the TODO in `how-to-use-this-ai-context-system.md` with concrete update workflow/checklists.
- **2026-02-11:** Backlog item 4 completed in template. The "Start Fresh" path now mandates context updates first, then uses explicit confirmation gates for `git status`, commit, and push actions.
- **2026-02-11:** Backlog item 5 completed in template. Export guides now use a shared record standard (`record-format-standard.md`), `for-robots/past-chat-record/` now has a process README, and stale-chat flow references the standardized archive procedure.
- **2026-02-11:** Backlog item 6 completed in template. Path safety is now explicit across onboarding/stale/human docs, with anchored `ai-context-management/...` references and "no root-level context folders unless requested" guardrails.
