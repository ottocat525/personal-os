# CLAUDE: Foundational Rules for AI Collaboration

> **[How to use this file]**
> These are absolute instructions for AI assistants. Any model connected to this knowledge base must follow them.
> Before each conversation, read `PSYCHE.md`.

---

## Folder Structure

```text
_private/              Vault. Never read it.
00_foundation/         Decision-making foundation. Permanent layer.
01_current_era/        Active projects and execution.
02_future_era/         Ideas that have not started yet.
03_fragments/          Fragments recalled through search.
04_external_resources/ Incoming external references.
05_self_growth/        Subjects and skills currently being learned.
```

---

## Absolute Prohibitions

- Never split documents into atomic notes.
- Never read or modify anything inside `_private/`.
- Never silently modify any file without user confirmation.
- Never create standalone wiki-style glossary pages.
- Never delete content merely because it appears repetitive.

---

## Operating Rules

**When receiving new material:**

Decide which folder it belongs to, tell the user, and let the user choose the final location.

**When finding a version conflict:**

Output a conflict list and let the user decide. Never merge conflicts without permission.

**During ordinary conversation:**

Answer directly. Do not proactively read any file.

---

## Rules for Updating PSYCHE.md

Trigger: the user explicitly asks for an update, or the AI notices a clear change in the user's thinking or preferences.

Process:

1. List the entries that should be added or removed.
2. Wait for user confirmation.
3. Update the file only after confirmation. Never modify it silently.

---

## Rules for NOW.md

`NOW.md` describes the user's current context. It is not the AI's workspace.

- The AI may read it to understand the user's current state.
- Write to it only when the user explicitly says: "Help me update NOW."

---

## Rules for Updating CLAUDE.md

Trigger: the user explicitly says: "Update the rules."

Process: list the proposed changes and wait for user confirmation before writing them.
