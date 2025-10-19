# Project Vision and Goals

## What We're Building

An AI context system (starter pack) for vibe coding and AI-assisted development. This is a tool-agnostic folder structure with documentation files that any AI agent can read to quickly understand a project's context, goals, patterns, and current state.

## Why We're Building It

**Pain points this solves:**
1. Context loss between AI chat sessions
2. Having to manually paste summaries at the start of new chats
3. AI agents losing awareness of project goals and patterns mid-conversation
4. No structured way to maintain project memory across different AI tools

## Project Goals

- **Universal compatibility:** Works with any AI tool (Cursor, ChatGPT, Claude, Copilot, Aider, etc.)
- **Easy adoption:** Simple paste-this-into-chat workflow to get started
- **Minimal maintenance:** Low overhead to keep context files updated
- **Scalable:** Works for solo devs and teams, small scripts and large projects

## Target Users

- Developers doing AI-assisted coding ("vibe coding")
- Solo developers who want project continuity across sessions
- Teams who want AI agents to understand their project conventions
- Anyone frustrated with re-explaining their project to AI repeatedly

## Repository Structure

The repository maintains two contexts:

**`ai-context-management/`** - The clean template product
- This is what users copy into their projects
- Contains only SYSTEM and TEMPLATE files
- No example content or implementation details

**`project-template-build-out-meta-wip/`** - Development workspace
- Contains working examples with actual content
- Includes meta documentation and planning
- Used for developing and testing the template itself
- **Not included in releases** (handled via `.gitattributes` export-ignore)

This structure allows us to work with real examples while distributing a clean template to users.

