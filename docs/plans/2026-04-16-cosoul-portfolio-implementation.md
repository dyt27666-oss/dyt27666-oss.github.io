# Cosoul Portfolio Homepage Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Replace the current built homepage with a static Apple-inspired portfolio landing page focused on the Cosoul.AI project family.

**Architecture:** Implement a self-contained `index.html` with embedded CSS and minimal JS. Keep the deployment model simple for GitHub Pages by avoiding any bundler dependency. Structure the page into hero, featured project, supporting projects, capability bands, highlights, and footer.

**Tech Stack:** HTML5, CSS3, vanilla JavaScript, GitHub Pages

---

### Task 1: Replace the current shell page with a full static homepage

**Files:**
- Modify: `index.html`

**Step 1: Remove the bundled-app bootstrap**

- Delete the current `<script type="module">` and stylesheet asset references.
- Replace the empty `#root` shell with full static markup.

**Step 2: Build the semantic page structure**

- Add sections for hero, featured project, project grid, capability bands, highlights, and footer.
- Keep anchors for in-page navigation.

**Step 3: Add project content**

- Use conservative descriptions for:
  - Cosoul.AI
  - soul-eval
  - humanlike-tastk_agent_prompt
  - PipeView
  - Cosoul.AI-Algorithm-Test

**Step 4: Add Apple-inspired visual styling**

- Implement layered gradients, light glass cards, restrained shadows, large typography, and responsive spacing entirely inside a `<style>` block.

**Step 5: Add light interaction**

- Add a small script for reveal-on-scroll and nav state polish.

### Task 2: Verify local rendering

**Files:**
- Verify: `index.html`

**Step 1: Open the page locally in a browser-compatible way**

- Use a simple local server or file-open flow to ensure the page renders without build tooling.

**Step 2: Inspect structure**

- Confirm the new page no longer depends on old build assets for critical rendering.

**Step 3: Check mobile behavior**

- Ensure cards stack cleanly and typography remains readable.

### Task 3: Preserve maintainability

**Files:**
- Create: `docs/plans/2026-04-16-cosoul-portfolio-design.md`
- Create: `docs/plans/2026-04-16-cosoul-portfolio-implementation.md`

**Step 1: Save the design summary**

- Document the design direction and content strategy.

**Step 2: Save the execution plan**

- Document the concrete implementation steps for later iteration.
