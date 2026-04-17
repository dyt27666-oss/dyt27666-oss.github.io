# Cosoul Cyberpunk Portfolio Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Replace the current Apple-like portfolio homepage with a cyberpunk product-release style homepage focused on the Cosoul project family and the user's “AI engineer with product and full-stack delivery capability” identity.

**Architecture:** Continue using a single self-contained `index.html` for GitHub Pages simplicity, but rewrite the visual system, page copy, and section structure. Reuse the existing Cosoul screenshots in `assets/cosoul-ai/` as the main visual evidence.

**Tech Stack:** HTML5, CSS3, vanilla JavaScript, GitHub Pages

---

### Task 1: Rewrite the visual system

**Files:**
- Modify: `index.html`

**Step 1: Replace the current light palette**

- Introduce dark surfaces, cyan/magenta glow accents, and deeper contrast.

**Step 2: Add cyberpunk atmospheric layers**

- Use grid overlays, panel glows, and restrained scanline / glow details.

**Step 3: Preserve responsiveness**

- Ensure the redesign still works on desktop and mobile.

### Task 2: Rewrite the hiring narrative

**Files:**
- Modify: `index.html`

**Step 1: Replace the current hero message**

- Lead with “AI工程师，兼具产品与全栈落地能力”.

**Step 2: Rewrite support text**

- Explicitly frame the user as a hybrid contributor across PM, engineering, and experimentation.

**Step 3: Align the closing CTA**

- Make the page read as a job-facing AI portfolio.

### Task 3: Strengthen Cosoul-centric structure

**Files:**
- Modify: `index.html`
- Reuse: `assets/cosoul-ai/*`

**Step 1: Keep Cosoul.AI as the flagship**

- Make it visually dominant.

**Step 2: Reframe the four support repos**

- Present them as systems around the main product rather than separate demos.

**Step 3: Add capability matrix**

- Translate project experience into hiring-friendly capability framing.

### Task 4: Verify static delivery

**Files:**
- Verify: `index.html`
- Verify: `assets/cosoul-ai/*`

**Step 1: Run a local static server**

- Confirm the homepage returns `200`.

**Step 2: Verify screenshot assets**

- Confirm the referenced images return `200`.

**Step 3: Check headline / key sections**

- Confirm the page contains the new cyberpunk hiring narrative.
