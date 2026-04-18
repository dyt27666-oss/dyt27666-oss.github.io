# Selected Work Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Add a selected-work section to the portfolio that restores the strongest non-Cosoul portfolio items without weakening the Cosoul-first narrative.

**Architecture:** Reuse the existing `project-card` and `gallery` patterns. Insert a new section after the career-target block, with three curated cards covering product delivery, data analysis, and research/modeling. Keep all Cosoul content unchanged.

**Tech Stack:** HTML, CSS, vanilla JavaScript, static image assets

---

### Task 1: Add planning docs

**Files:**
- Create: `docs/plans/2026-04-18-selected-work-design.md`
- Create: `docs/plans/2026-04-18-selected-work-implementation.md`

**Step 1: Write the design summary**

Describe why the old content should return only as curated supporting evidence.

**Step 2: Write the implementation plan**

Document the target section, files, and gallery reuse plan.

**Step 3: Commit**

```bash
git add docs/plans
git commit -m "docs: plan selected work section"
```

### Task 2: Add selected-work navigation and section

**Files:**
- Modify: `index.html`

**Step 1: Add a nav link for the new section**

Add a `Selected Work` anchor in the top nav.

**Step 2: Add a new section after the targets section**

Create a section with:

1. a short intro
2. one card for `FitTrack AI`
3. one card for `电商 GMV / RFM 分析`
4. one card for `Research Highlights`

**Step 3: Reuse gallery structure**

Each card should use the existing gallery component with 2-3 images.

**Step 4: Commit**

```bash
git add index.html
git commit -m "feat: add selected work section"
```
