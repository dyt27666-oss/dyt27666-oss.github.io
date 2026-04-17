# Portfolio Gallery Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Add a reusable gallery interaction to the portfolio so flagship and supporting project screenshots can be switched without expanding the page vertically.

**Architecture:** Keep the page as a static single-file site. Add reusable gallery CSS and a small vanilla JS initializer that activates slides, arrows, and dots for each gallery instance. Reuse the same component for the flagship gallery and the supporting-system screenshot blocks.

**Tech Stack:** HTML, CSS, vanilla JavaScript, static image assets

---

### Task 1: Prepare gallery assets and docs

**Files:**
- Create: `docs/plans/2026-04-18-portfolio-gallery-design.md`
- Create: `docs/plans/2026-04-18-portfolio-gallery-implementation.md`
- Create/Copy: `assets/cosoul-market/market-create-agent.png`
- Create/Copy: `assets/cosoul-feature/feature-profile.png`
- Create/Copy: `assets/cosoul-labs/soul-eval/detail-overview.png`
- Create/Copy: `assets/cosoul-labs/soul-eval/judge-workspace.png`
- Create/Copy: `assets/cosoul-labs/prompt-lab/multi-model.png`
- Create/Copy: `assets/cosoul-labs/prompt-lab/prompt-lab-report.png`
- Create/Copy: `assets/cosoul-labs/algorithm-test/funnel-overview.png`
- Create/Copy: `assets/cosoul-labs/algorithm-test/matching-report.png`
- Create/Copy: `assets/cosoul-labs/pipeview/pipeline-dashboard.png`

**Step 1: Copy the selected local screenshots into stable repo asset paths**

Use PowerShell `Copy-Item` from the local resume folders into the repo asset folders.

**Step 2: Verify the copied paths exist**

Run `Get-ChildItem assets -Recurse` and confirm the expected files are present.

**Step 3: Commit**

```bash
git add docs/plans assets
git commit -m "chore: prepare portfolio gallery assets"
```

### Task 2: Add reusable gallery styles and markup

**Files:**
- Modify: `index.html`

**Step 1: Replace flagship screenshot stack with a gallery structure**

Add a gallery container with:

```html
<div class="gallery flagship-gallery" data-gallery>
  <div class="gallery-stage">...</div>
  <div class="gallery-controls">...</div>
</div>
```

**Step 2: Replace each supporting-system screenshot block with gallery markup**

Each project keeps its card text, but its screenshot section becomes a reusable gallery instance.

**Step 3: Add CSS for slides, arrows, dots, and single-image fallback**

Styles should cover:

```css
.gallery
.gallery-stage
.gallery-slide
.gallery-button
.gallery-dots
.gallery-dot
.gallery.single-slide .gallery-controls
```

**Step 4: Commit**

```bash
git add index.html
git commit -m "feat: add reusable screenshot gallery layout"
```

### Task 3: Add vanilla JS gallery behavior and verify

**Files:**
- Modify: `index.html`

**Step 1: Add a gallery initializer script**

Implement a small initializer that:

1. Finds all `[data-gallery]`
2. Tracks current slide index
3. Wires previous/next buttons
4. Generates clickable dots
5. Hides controls for single-image galleries

**Step 2: Run lightweight verification**

Use:

```bash
git diff -- index.html
```

And confirm:

1. flagship gallery contains multiple slides
2. supporting galleries contain their intended image counts
3. no old stacked flagship layout remains

**Step 3: Commit**

```bash
git add index.html
git commit -m "feat: add screenshot gallery interactions"
```
