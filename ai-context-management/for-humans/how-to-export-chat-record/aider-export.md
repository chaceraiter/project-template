<!-- SYSTEM FILE - Do not modify. Reference guide for exporting chats. -->

# Exporting Chats from Aider

First read `record-format-standard.md` in this folder.

## Method 1: Use `.aider.chat.history.md` (Primary)
1. Open `.aider.chat.history.md` in your project
2. Copy the relevant session or section
3. Save it to `ai-context-management/for-robots/past-chat-record/`
4. Use filename format from `record-format-standard.md`

## Method 2: Terminal History (Fallback)
1. Copy relevant conversation content from terminal scrollback
2. Save to `ai-context-management/for-robots/past-chat-record/` with standard naming

## Method 3: Structured Summary (Fallback)
Use this when you cannot produce a clean transcript:
1. Write a structured summary using required sections in `record-format-standard.md`
2. Save it to `ai-context-management/for-robots/past-chat-record/` with standard naming

## After Export

Follow the required post-export updates in `record-format-standard.md` so current context stays accurate.
