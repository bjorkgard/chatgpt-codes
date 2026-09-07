# Travel Posters Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Add a collection-based prompt library with a new "Travel Posters" collection and generated examples for all 14 travel poster prompts.

**Architecture:** Keep the static Markdown catalog simple: a top-level prompt collection index, one folder per collection, one Markdown file per prompt, and matching example image folders. Existing prompt content remains intact, while Travel Posters adds a reusable master template plus city-specific prompts.

**Tech Stack:** Markdown documentation, local filesystem organization, generated PNG assets through ImageGen, shell verification commands.

---

### Task 1: Reorganize Prompt Collections

**Files:**
- Modify: `/Users/nathanael/Code/chatgpt-codes/docs/prompts/README.md`
- Create: `/Users/nathanael/Code/chatgpt-codes/docs/prompts/visual-illusions/README.md`
- Move: `/Users/nathanael/Code/chatgpt-codes/docs/prompts/01-anamorphic-staircase.md` through `/Users/nathanael/Code/chatgpt-codes/docs/prompts/09-miniature-city-diorama-portrait.md`
- Move: `/Users/nathanael/Code/chatgpt-codes/examples/prompts/*.png`

- [ ] Create `docs/prompts/visual-illusions/` and `examples/prompts/visual-illusions/`.
- [ ] Move the existing 9 prompt Markdown files into `docs/prompts/visual-illusions/`.
- [ ] Move their 9 existing PNG examples into `examples/prompts/visual-illusions/`.
- [ ] Update image links inside the moved Markdown files from `../../examples/prompts/...` to `../../../examples/prompts/visual-illusions/...`.
- [ ] Replace `docs/prompts/README.md` with a collection index linking to Visual Illusions and Travel Posters.

### Task 2: Add Travel Posters Prompt Files

**Files:**
- Create: `/Users/nathanael/Code/chatgpt-codes/docs/prompts/travel-posters/README.md`
- Create: `/Users/nathanael/Code/chatgpt-codes/docs/prompts/travel-posters/00-master-template.md`
- Create: `/Users/nathanael/Code/chatgpt-codes/docs/prompts/travel-posters/01-paris.md` through `/Users/nathanael/Code/chatgpt-codes/docs/prompts/travel-posters/14-rome.md`

- [ ] Create the Travel Posters collection README with usage guidance, prompt design rules, and city index.
- [ ] Create the master template with the three fill-in slots: landmarks, supporting elements, and palette.
- [ ] Create 14 city prompt files: Paris, Istanbul, Sydney, Dubai, Tokyo, London, Barcelona, Venice, Amsterdam, Hong Kong, Seoul, San Francisco, New York, and Rome.
- [ ] Ensure each city file includes a complete standalone prompt and concise usage notes.

### Task 3: Generate Example Images

**Files:**
- Create: `/Users/nathanael/Code/chatgpt-codes/examples/prompts/travel-posters/01-paris.png` through `/Users/nathanael/Code/chatgpt-codes/examples/prompts/travel-posters/14-rome.png`

- [ ] Generate one vertical example image for each city prompt.
- [ ] Save each generated example to the expected city filename.
- [ ] Confirm every image is a readable PNG.

### Task 4: Verify Documentation Links

**Files:**
- Check all changed Markdown and generated images.

- [ ] Run a file existence check for all city Markdown files and PNG examples.
- [ ] Search for stale `../../examples/prompts/` links in moved prompt files.
- [ ] Review `git diff --stat` and `git diff -- docs/prompts README.md`.
- [ ] Report any ungenerated or missing assets clearly.
