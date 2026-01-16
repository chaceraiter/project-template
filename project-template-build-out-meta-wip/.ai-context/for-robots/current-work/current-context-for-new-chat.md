# Current Context for New Chat

This meta folder mirrors the template structure and captures project-template-specific build notes and WIP plans.

## Current State

- The reusable template lives in `ai-context-management/` and should stay generic.
- This meta mirror lives in `project-template-build-out-meta-wip/.ai-context/` and is where we track build/process notes and future improvements.
- The system is mostly finished; remaining work is a short set of targeted improvements to agent instructions and procedures.

## Backlog: Planned Improvements (Do Next, 1-by-1)

1. **Stale chat procedure:** Adjust stale AI flow so it explicitly asks which of the two options to take before doing any additional project reading or actions. Target: `ai-context-management/for-robots/ai-agent-stale-chat-procedures.md`.
2. **New chat entrypoint assumptions:** Update the “new AI chat” flow so it does not assume either (a) existing project adding a new AI context system or (b) brand-new project adding a new AI context system; support (c) existing project + existing AI context system, but starting a fresh chat to reduce context rot. Targets: `ai-context-management/for-robots/ai-agent-orientation-start-here.md` and `ai-context-management/for-humans/paste-this-into-new-ai-chats.txt` (or equivalent entrypoint).
3. **Update cadence emphasis:** Improve the docs to emphasize regularly updating `current-work/` and other context folders, with clearer guidance on when/what to update and where those reminders live. Targets: orientation + human instructions.
4. **“Start fresh” automation:** Rework the stale-chat “Start Fresh” path to guide automatic context updates first, then ask whether to run `git status`, commit, and push (only after explicit user confirmation). Targets: stale-chat procedures + possibly operating rules.
5. **Chat export + past-chat-record procedures:** Update export instructions and the `past-chat-record/` process (format, naming, what to include, export vs summary, and how/when to update current-work docs afterward). Targets: `ai-context-management/for-humans/how-to-export-chat-record/*.md` and related robot procedures.

## Plan

- Keep all implementation changes in the reusable template (`ai-context-management/`) but track planning and decisions here.
- Execute the backlog top-to-bottom (1 → 5), validating each change against the intended “template vs meta” separation.
