# Current Context for New Chat

This meta folder mirrors the template structure and captures project-template-specific build notes and WIP plans.

## Current State

- The reusable template lives in `ai-context-management/` and should stay generic.
- This meta mirror lives in `project-template-build-out-meta-wip/.ai-context/` and is where we track build/process notes and future improvements.
- The system is mostly finished; remaining work is a short set of targeted improvements to agent instructions and procedures.

## Known Pain Points to Address

- **Triple-option new chat onboarding is incomplete:** New-chat orientation must explicitly support all three cases:
  - Brand-new repo + new AI context system
  - Existing repo + new AI context system
  - Existing repo + existing AI context system, but new chat (context-rot reset)
- **Relative path ambiguity causes wrong folder placement:** Some agents interpret names like `past-chat-record/` as repo-root folders instead of `ai-context-management/for-robots/past-chat-record/`.
- **Long-chat drift:** In long sessions, agents stop proactively using or referencing the context management system unless the user reminds them.

## Backlog: Planned Improvements (Do Next, 1-by-1)

1. **Stale chat procedure:** Adjust stale AI flow so it explicitly asks which of the two options to take before doing any additional project reading or actions. Target: `ai-context-management/for-robots/ai-agent-stale-chat-procedures.md`.
2. **New chat entrypoint assumptions:** Update the “new AI chat” flow so it explicitly supports three cases: (a) brand-new repo + new AI context system, (b) existing repo + new AI context system, and (c) existing repo + existing AI context system with a new chat for context reset. Targets: `ai-context-management/for-robots/ai-agent-orientation-start-here.md` and `ai-context-management/for-humans/paste-this-into-new-ai-chats.txt` (or equivalent entrypoint).
3. **Update cadence emphasis + proactive reminders:** Improve the docs to emphasize regularly updating `current-work/` and other context folders, with clearer guidance on when/what to update and where those reminders live; include explicit proactive reminder behavior for long chats. Targets: orientation + human instructions + operating rules if needed.
4. **“Start fresh” automation:** Rework the stale-chat “Start Fresh” path to guide automatic context updates first, then ask whether to run `git status`, commit, and push (only after explicit user confirmation). Targets: stale-chat procedures + possibly operating rules.
5. **Chat export + past-chat-record procedures:** Update export instructions and the `past-chat-record/` process (format, naming, what to include, export vs summary, and how/when to update current-work docs afterward). Targets: `ai-context-management/for-humans/how-to-export-chat-record/*.md` and related robot procedures.
6. **Path safety hardening:** Standardize instructions to use unambiguous anchored paths under `ai-context-management/` (or explicit relative-from-current-file references) and explicitly say not to create context folders at repo root unless intentionally configured.

## Plan

- Keep all implementation changes in the reusable template (`ai-context-management/`) but track planning and decisions here.
- Execute the backlog top-to-bottom (1 → 6), validating each change against the intended “template vs meta” separation.

## Progress Updates

- **2026-02-11:** Backlog item 1 completed in template. `ai-agent-stale-chat-procedures.md` now includes an explicit hard gate to ask A/B first and avoid any additional reading/actions until the user chooses.
- **2026-02-11:** Backlog item 2 completed in template. `ai-agent-orientation-start-here.md` and `paste-this-into-new-ai-chats.txt` now enforce explicit A/B/C onboarding triage, including the "existing repo + existing context system + fresh chat" case.
- **2026-02-11:** Backlog item 3 completed in template. Added proactive context-maintenance cadence rules to `ai-agent-orientation-start-here.md` and replaced the TODO in `how-to-use-this-ai-context-system.md` with concrete update workflow/checklists.
- **2026-02-11:** Backlog item 4 completed in template. The "Start Fresh" path now mandates context updates first, then uses explicit confirmation gates for `git status`, commit, and push actions.
- **2026-02-11:** Backlog item 5 completed in template. Export guides now use a shared record standard (`record-format-standard.md`), `for-robots/past-chat-record/` now has a process README, and stale-chat flow references the standardized archive procedure.
- **2026-02-11:** Backlog item 6 completed in template. Path safety is now explicit across onboarding/stale/human docs, with anchored `ai-context-management/...` references and "no root-level context folders unless requested" guardrails.
