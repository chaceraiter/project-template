<!-- TEMPLATE FILE - Fill this out to explain your project's AI context system to humans. -->

# How to Use This AI Context System

This system keeps AI chats aligned over time by storing project context in files instead of relying only on chat memory.

## What This Solves

- Reduces context loss between chat sessions
- Preserves decisions and current status
- Helps new AI chats get oriented quickly

## Daily Workflow

1. Start each new AI chat by pasting `ai-context-management/for-humans/paste-this-into-new-ai-chats.txt`.
2. Let the AI orient using `ai-context-management/for-robots/` files before starting implementation.
3. During work, keep `ai-context-management/for-robots/current-work/` files updated as state changes.
4. When ending sessions, archive important chat context in `ai-context-management/for-robots/past-chat-record/`.

## Update Cadence (Important)

Update context files proactively, not only when something breaks.

- After meaningful code or architecture changes: update `ai-context-management/for-robots/current-work/current-context-for-new-chat.md`.
- When goals/phases/tasks shift: update `ai-context-management/for-robots/current-work/current-work-focus.md`.
- After major decisions, blockers, or long debugging sessions: create/update a dated note in `ai-context-management/for-robots/past-chat-record/`.
- Before switching chats or ending the day: do a quick context sync pass across `ai-context-management/for-robots/current-work/`.

## Minimum End-of-Session Checklist

1. `current-context-for-new-chat.md` reflects what changed, what works, what is blocked, and what is next.
2. `current-work-focus.md` still matches the real project goal, current phase, and immediate task.
3. Key decisions from the session are preserved in `past-chat-record/` when needed.

## Path Rule

Unless you intentionally customize the layout, keep all context-system files inside `ai-context-management/` and avoid creating duplicate root-level folders like `past-chat-record/` or `current-work/`.

## Rule of Thumb

If a future AI chat would be confused without this information, write it down now in the context system.
