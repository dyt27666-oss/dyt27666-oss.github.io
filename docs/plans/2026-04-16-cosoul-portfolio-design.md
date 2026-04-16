# Cosoul Portfolio Homepage Design

**Goal:** Rebuild the homepage as an Apple-inspired portfolio landing page centered on the Cosoul.AI project family, while preserving the user's positioning for AI agent and data-intelligence roles.

**Audience:** Recruiters, interviewers, collaborators, and hiring managers who need to understand the user's project depth quickly.

**Design Direction:** Calm, high-precision, Apple-like presentation with soft gradients, restrained glass layers, large typography, and low-noise information hierarchy. The page should feel premium rather than flashy.

---

## Content Strategy

### Positioning

- Primary identity: AI agent and data-intelligence project developer
- Secondary identity: early-career candidate with practical project delivery, not just coursework
- Message: can contribute to both collaborative AI product development and independent tooling / evaluation / algorithm experimentation

### Project Narrative

The page should present a clear ladder:

1. **Cosoul.AI** as the flagship collaborative product
2. **Soul Eval** as the evaluation and prompt optimization platform
3. **Humanlike Task Agent Prompt** as the prompt lab for improving agent interaction quality
4. **PipeView** as the monitoring and observability dashboard
5. **Cosoul.AI-Algorithm-Test** as the matching algorithm experiment and benchmark platform

This sequence makes the project family feel like a system instead of unrelated demos.

### Copy Tone

- Concise, product-minded, technically grounded
- Avoid exaggerated metrics that are not verified
- Use claims that can survive interview follow-up
- Emphasize ownership, architecture, and engineering decisions

---

## Page Structure

### 1. Hero

- Large headline establishing the portfolio theme
- Supporting paragraph describing the user's work on AI agent systems, evaluation, workflow, and algorithm experimentation
- Two CTAs:
  - jump to projects
  - open GitHub profile

### 2. Featured Project Spotlight

- Dedicated panel for **Cosoul.AI**
- Explain product concept, multi-agent social matching, cross-platform architecture, and role in the team project
- Include high-signal tags:
  - Next.js
  - Expo / React Native
  - TypeScript
  - PostgreSQL / pgvector
  - Multi-Agent

### 3. Project Grid

- Four polished cards for the independent supporting projects
- Each card should include:
  - what problem it solves
  - what was built
  - technical keywords
  - role ownership

### 4. Capability Bands

- Three grouped capability lenses:
  - Agent Product Engineering
  - Evaluation and Prompt Systems
  - Retrieval, Matching, and Monitoring

This helps recruiters understand the user's repeated strengths across projects.

### 5. Selected Highlights

- Small numeric / factual section using conservative counts:
  - 5 linked projects
  - cross-platform app architecture
  - evaluation / monitoring / algorithm stack
  - independent build ownership on 4 supporting repos

### 6. Contact Footer

- GitHub link
- email placeholder or existing contact if available
- short closing statement oriented to internship / junior opportunities

---

## Visual System

### Palette

- Warm white base
- Light silver gradients
- Blue-gray accent
- Dark graphite text
- Soft glass borders, not strong neon glow

### Typography

- Strong display headline with system-friendly Apple-adjacent feel
- Chinese-first readability
- English labels remain clean and understated

### Motion

- Subtle fade / slide entrances
- Gentle hover lift on cards
- No aggressive parallax or over-animated backgrounds

### Layout

- Wide desktop spacing
- Compressed but readable mobile stacking
- Strong section rhythm with alternating density

---

## Implementation Notes

- Since the repo currently serves a built static page, replace `index.html` with a self-contained static implementation that does not depend on missing source files.
- Keep existing `assets/` untouched for now unless specific Cosoul screenshots are later added.
- Use a handcrafted HTML + CSS + small JS reveal script so deployment remains simple on GitHub Pages.

---

## Risks

- The current project evidence is stronger on architecture and tooling than on quantified outcomes, so the copy must avoid fake business impact.
- Too much “Apple style” would make the page feel generic or empty; the design should still prioritize recruiter comprehension.
- If the user later wants bilingual content, the page structure should remain easy to extend.
