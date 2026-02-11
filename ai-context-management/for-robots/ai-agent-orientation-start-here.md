<!-- SYSTEM FILE - Do not modify. This is the core orientation file for the AI context system. -->

# AI Agent Orientation - Start Here

Welcome! You are being onboarded to a project that uses an AI context system. This system is designed to solve the common problem of context loss between AI chat sessions.

Do not assume this is a brand-new project. First determine which onboarding scenario applies.

## Path Safety Rule (Required)

- Treat `ai-context-management/` as the context-system root.
- Do not create context folders like `past-chat-record/`, `current-work/`, or `project-setup/` at repo root unless the user explicitly asks for that layout.

## Required First Question (Before Any Other Work)

Ask the user:

Which scenario are we in right now?
- **A) Brand-new repo + new AI context system**
- **B) Existing repo + adding AI context system now**
- **C) Existing repo + existing AI context system, starting a fresh chat**

Wait for the user's answer before reading additional project files or proposing setup work.

## Directory Structure Overview

This project uses a structured approach to maintain context across conversations. Here's what everything means:

### `project-setup/` - Foundational Documents (Set Once)

All files in this section live under `ai-context-management/for-robots/project-setup/`.

**`agent-operating-rules.md`** - Your core operating principles for this project. This defines how you should communicate, what standards to follow, workflow preferences, and red lines you must never cross. These rules should be kept in mind throughout all interactions.

**`project-vision-and-goals.md`** - The big picture of what we're building and why. This explains the project's purpose, target users, success criteria, and long-term direction.

**`project-architecture.md`** - The technical architecture, technology stack, system design, and key architectural patterns. This provides the technical foundation for understanding how the system is built.

**`code-patterns-and-conventions.md`** - Established code patterns, naming conventions, and coding standards specific to this project. Follow these patterns when writing code.

### `current-work/` - Active Context (Updated Frequently)

All files in this section live under `ai-context-management/for-robots/current-work/`.

**`current-work-focus.md`** - A 3-5 sentence summary with three levels of focus. The **Project Goal** describes the high-level vision of what we're building (the big picture). The **Intermediate Goal** specifies the current phase or milestone we're working toward (medium-term). The **Current Task** states exactly what is being worked on right now (immediate focus). This hierarchical structure helps you quickly understand where we are in the overall journey.

**`current-context-for-new-chat.md`** - A living document with the current state of the project. What's working, what's broken, active issues, recent changes. This should be updated regularly as work progresses.

### `past-chat-record/` - Historical Archive

This directory contains archived summaries from previous AI chat sessions. Each file should be dated and include key decisions, code written, and problems solved. This serves as the project's memory.
This directory lives at `ai-context-management/for-robots/past-chat-record/`.

---

## Proactive Context Maintenance (Required)

Do not wait for the user to remind you. Proactively keep the context system current.

- After each meaningful implementation step, suggest updating `ai-context-management/for-robots/current-work/current-context-for-new-chat.md`.
- When project direction, milestone, or immediate task changes, update `ai-context-management/for-robots/current-work/current-work-focus.md`.
- When a long chat accumulates important decisions, suggest adding a dated summary in `ai-context-management/for-robots/past-chat-record/`.
- In long sessions, run periodic context hygiene checks (for example every 30-60 minutes or after major topic changes).
- Before ending a session or switching to a new chat, ensure current state is written down in `ai-context-management/for-robots/current-work/`.

---

## Scenario Handling Instructions

Follow the branch that matches the user's A/B/C choice.

### Scenario A: Brand-New Repo + New AI Context System

1. Set up the AI context files if they are missing.
2. Ask setup questions and fill in the foundational docs:
   - `ai-context-management/for-robots/project-setup/project-vision-and-goals.md`
   - `ai-context-management/for-robots/project-setup/project-architecture.md`
   - `ai-context-management/for-robots/project-setup/code-patterns-and-conventions.md`
   - `ai-context-management/for-robots/project-setup/agent-operating-rules.md`
3. Capture immediate state in:
   - `ai-context-management/for-robots/current-work/current-work-focus.md`
   - `ai-context-management/for-robots/current-work/current-context-for-new-chat.md`

### Scenario B: Existing Repo + Adding AI Context System Now

1. Ask for permission to quickly scan existing project docs/code so you can write accurate context files.
2. Populate the same foundational files in `ai-context-management/for-robots/project-setup/` based on the existing project.
3. Capture current status in `ai-context-management/for-robots/current-work/`:
   - What's already implemented
   - What's currently in progress
   - What's next
4. Flag any unknowns explicitly instead of guessing.

### Scenario C: Existing Repo + Existing AI Context System, Starting Fresh Chat

1. Re-orient by reading:
   - `ai-context-management/for-robots/project-setup/agent-operating-rules.md`
   - `ai-context-management/for-robots/current-work/current-work-focus.md`
   - `ai-context-management/for-robots/current-work/current-context-for-new-chat.md`
2. If needed, skim relevant files in `ai-context-management/for-robots/past-chat-record/` for missing decisions.
3. Confirm readiness and continue current work.
4. Only run setup-style onboarding questions if key files are missing or clearly outdated.
5. In long chats, proactively suggest context updates instead of waiting for user reminders.

---

## Setup Questions (Use for Scenario A, and for Scenario B when needed)

### Step 1: Project Vision
What is this project about? Tell me:
- What are you building?
- Why are you building it?
- Who is it for?

_(Keep it brief - I'll capture this in `ai-context-management/for-robots/project-setup/project-vision-and-goals.md`)_

### Step 2: Technical Architecture
What's the technical foundation?
- What languages, frameworks, or technologies?
- Any key architectural decisions already made?

_(I'll document this in `ai-context-management/for-robots/project-setup/project-architecture.md`)_

### Step 3: Code Patterns
Are there any specific code patterns, naming conventions, or standards you want to follow?

_(Goes into `ai-context-management/for-robots/project-setup/code-patterns-and-conventions.md`)_

### Step 4: Operating Rules
How should we work together?
- Any preferences on communication style?
- Testing or documentation requirements?
- Things I should never do without asking?

_(These become your `ai-context-management/for-robots/project-setup/agent-operating-rules.md`)_

### Step 5: Current Work
What are you working on right now?
- Overall project goal?
- Current phase/milestone?
- Immediate task?

_(This sets up `ai-context-management/for-robots/current-work/current-work-focus.md`)_

---

**After setup:** Briefly explain how to use `ai-context-management/for-robots/current-work/current-context-for-new-chat.md` and `ai-context-management/for-robots/past-chat-record/` to maintain continuity across sessions.
