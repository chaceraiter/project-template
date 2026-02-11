<!-- SYSTEM FILE - Do not modify. Shared standard for saving chat records. -->

# Past Chat Record Standard

Use this standard for every exported or summarized chat record.

## Destination Folder

Save records to:

`ai-context-management/for-robots/past-chat-record/`

## Filename Standard

Use:

`YYYY-MM-DD-<tool>-<short-topic>.md`

Examples:
- `2026-02-11-cursor-context-backlog.md`
- `2026-02-11-chatgpt-architecture-decisions.md`

If multiple records share the same topic/date, add a numeric suffix:
- `2026-02-11-cursor-context-backlog-02.md`

## Minimum Required Content

Each record should include:

1. Session metadata (date, tool, participants if useful)
2. What was attempted or discussed
3. Key decisions made
4. Changes made (include file paths when applicable)
5. Open issues or risks
6. Next recommended step

## Full Export vs Structured Summary

- Prefer full export when the platform provides clean chat output.
- Use a structured summary when full export is unavailable, noisy, or excessively long.
- For very long chats, include a concise summary plus a pointer to the raw transcript source if available.

## Required Follow-Up After Saving a Record

After the chat record is written:

1. Update `ai-context-management/for-robots/current-work/current-context-for-new-chat.md`
2. Update `ai-context-management/for-robots/current-work/current-work-focus.md` if goals/phase/task changed
3. Ensure the next chat can continue without re-discovering decisions
