# Project Archive Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Add a lightweight archive section that restores the remaining legacy portfolio projects without weakening the Cosoul-first structure.

**Architecture:** Reuse the page's existing card language but introduce a lighter archive-card style. Keep the archive below the selected-work section so the page reads from flagship work to supporting work to legacy archive.

**Tech Stack:** HTML, CSS, static image assets

---

### Task 1: Add planning docs

**Files:**
- Create: `docs/plans/2026-04-18-project-archive-design.md`
- Create: `docs/plans/2026-04-18-project-archive-implementation.md`

**Step 1: Write design summary**

Document the archive-vs-selected-work distinction.

**Step 2: Write implementation plan**

Document the lightweight archive card structure.

**Step 3: Commit**

```bash
git add docs/plans
git commit -m "docs: plan project archive section"
```

### Task 2: Add archive styles and section

**Files:**
- Modify: `index.html`

**Step 1: Add archive-grid and archive-card styles**

Create compact, lower-emphasis card styles that still fit the current dark cyberpunk page.

**Step 2: Add a Project Archive section after Selected Work**

Each archive card should include:

1. short project label
2. title
3. one-sentence description
4. one representative image

**Step 3: Commit**

```bash
git add index.html
git commit -m "feat: add archive section for legacy projects"
```
