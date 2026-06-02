# Personal OS Framework

[中文版](https://github.com/ottocat525/personal-os/tree/main)
> The framework is for everyone. Your PSYCHE.md can only be written by you.
> A personal knowledge and decision-making framework built on Markdown, centered on the person, and independent of any specific tool or AI model.
> No note-taking app lock-in. No AI vendor lock-in. Three core files. Ready to customize.

---

## Tool Compatibility

The foundation only depends on Markdown, so you can use any editor that supports Markdown.

Backlinks, block embeds, and the keyboard shortcuts listed below are optional enhancements. They require a compatible tool such as Obsidian. The core folder structure and three core files still work without them.

---

## Why Not Atomic Notes?

Atomic notes split knowledge into hundreds of small, interlinked entries. That approach has a structural flaw:

**It moves complexity instead of eliminating it.**

Split one long document into 100 atoms and the complexity moves from inside the document to the links between documents. As the number of notes grows, the cost of maintaining links rises sharply. Orphan nodes multiply, entropy increases, and the system eventually collapses.

The deeper problem is this: **atomic notes kill context.**

Six months later, an isolated note no longer tells you why you wrote it, what evidence shaped your judgment, or whether the conclusion was later overturned. Knowledge compounds when causal chains survive, not when individual facts survive.

Atomic notes are useful for knowledge that can be decoupled, such as programming documentation and technical specifications. Most personal knowledge is different:

```text
A judgment -> triggers a decision -> drives an action
```

Split that chain into three atoms and the context disappears. Every fragment becomes an orphan.

---

## Core Assumptions

```text
1. Knowledge has causal chains that should not be decoupled.
2. People change, so the system must grow with them.
3. Intuition and rational tools are equally valid inputs.
```

---

## Three Core Files: Way, Rules, Practice

The whole system has only three required files:

```text
PSYCHE.md   Way       Who you are and your underlying logic. Changes slowly.
CLAUDE.md   Rules     AI behavior rules that protect the Way.
NOW.md      Practice  Your current execution state. Updated whenever needed.
```

The Way shapes the Rules. The Rules govern Practice. Practice returns to the Way.

The AI first reads the Way (`PSYCHE.md`), then follows the Rules (`CLAUDE.md`), then checks the Practice (`NOW.md`) to understand where you are now.

### PSYCHE.md - Way

Your mirror. It records your thinking habits, decision-making principles, current stage, and communication preferences.

When an AI reads this file, it knows who it is talking to instead of giving generic advice to a stranger.

This file grows with you. When the AI notices a meaningful change in your preferences or behavior, it suggests an update and waits for your confirmation.

### CLAUDE.md - Rules

The AI's operating law. It defines what the AI may do, what it must never do, and how it should handle common situations.

The file is model-independent. Switch from DeepSeek to GPT or any other model and the rules still apply.

### NOW.md - Practice

Your current context: the three most important things this month, current blockers, key milestones, and temporary fragments.

**Review it weekly. Update it whenever needed. Do not archive or empty it.**

Daily tasks do not belong here. Use a phone note for today's three tasks, then clear it when the day is over. `NOW.md` is the strategic layer; your daily note is the execution layer.

---

## Folder Structure

```text
_private/              Vault for private information
00_foundation/         Time coordinates, decision principles, and methodology
01_current_era/        Active projects and execution
02_future_era/         Ideas that have not started yet
03_fragments/          Quotes, inspirations, and fragments recalled through search
04_external_resources/ Web pages, videos, PDFs, and other incoming references
05_self_growth/        Skills and subjects you are currently learning
```

### About `00_foundation`

This is the most important folder in the system. It stores the principles behind your decisions.

Everyone's foundation is different, but the structure stays the same:

```text
time_coordinates.md    The framework you use to give time meaning and priority
                       (quarterly OKRs, academic terms, industry cycles, or anything else)
decision_principles.md The principles you rely on when making decisions
glossary.md            Terms worth keeping because they appear repeatedly
```

The templates are intentionally empty. Fill them with what you actually believe. There is no standard answer.

---

## Long Scrolls, Not Atoms

**Core principle: split by narrative completeness, not by the size of a fact.**

One project equals one long scroll. Keep technical details, legal notes, execution logs, and decision records in one document so the causal chain remains intact.

Three techniques keep long documents navigable:

**1. Outline view**

Use `##` and `###` headings in long documents. Open the outline panel and collapse the sections you do not need. Even a document with tens of thousands of words becomes manageable.

**2. Split panes**

Pin your foundation on the left while switching between project scrolls on the right.

**3. Navigation anchors**

Add a table of contents at the top. Each section heading becomes an anchor, so you can jump directly to it even on mobile.

---

## Links: Stitch Only When Needed

Use backlinks (`[[ ]]`) only when two pieces of content need to support each other logically. Do not link merely for the sake of creating links.

**Three levels:**

**Basic: signpost**

```text
[[project_execution_scroll]]
```

Link directly to another document.

**Advanced: precise landing**

```text
[[industry_research_report#Key Findings]]
```

Add a `#` heading after the file name to jump directly to a specific section.

**Full embed: live projection**

```text
![[foundation^block-id]]
```

Add a `^` block ID at the end of a source paragraph and embed it elsewhere with `![[]]`. When the source changes, every embed updates automatically. This eliminates version conflicts.

---

## Growth Mechanism

This system grows with you:

**Proactive `PSYCHE.md` updates**

The AI notices a new habit or preference -> suggests an update -> you confirm -> the file changes.

The AI notices that an old entry conflicts with your current state -> asks whether to remove it -> you decide.

**Every update requires your confirmation. The AI must never silently modify any file.**

---

## Keyboard Shortcuts (Obsidian Examples)

```text
Ctrl/Cmd + P        Command palette
Ctrl/Cmd + O        Quick file switcher (type NOW and press Enter)
Ctrl/Cmd + Shift+F  Search the entire vault
Alt + click link    Open a backlink in a side pane
```

---

## Who This Framework Is For

- Your thinking jumps across domains and does not fit subject-based folders.
- You need a decision log, not a knowledge encyclopedia.
- You want a system that grows with you instead of a static database.
- You want AI as a collaborator, not merely an organizer.

---

## Who This Framework Is Not For

- Teams that need a collaborative knowledge base. This is a personal operating system.
- Pure technical documentation management. Atomic notes work well in that context.
- Anyone expecting a zero-customization setup. You must fill in `00_foundation` yourself.

---

## Getting Started

1. Clone this repository.
2. Create a local `_private/` directory for anything that must never sync to a public cloud.
3. Open the repository in any Markdown editor.
4. Fill in `PSYCHE.md` first. Describe who you are.
5. Then fill in `CLAUDE.md`. Tell the AI your rules.
6. Open `NOW.md`. Write down the three most important things this month.
7. Open `00_foundation`. Fill in your own time coordinates.

**Do not migrate all your old notes at once. Start with the skeleton. Move a project only when you need it.**

---

## Contributing

This is a living framework. Pull requests are welcome.

Templates for different groups are especially welcome: students, founders, freelancers, and others.

---

*Markdown foundation. Replaceable tools. Replaceable AI. The only irreplaceable part is what you put into the system yourself.*

---

## Requirements

**Basic Git knowledge is required.** This framework assumes that you use Git and GitHub for version control.

Benefits:

- `_private/` is excluded by `.gitignore`, so private information is not uploaded.
- Every change has history and can be rolled back.
- You can clone the repository on another device and continue working.

If you do not use Git, at minimum:

- Back up the entire folder locally on a regular basis.
- Or use a sync tool such as Obsidian Sync or OneDrive.
- **No matter what, never sync `_private/` to any public cloud.**
