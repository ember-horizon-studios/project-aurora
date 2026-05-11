# Plan — P2: Studio Systems & Infrastructure

**Level:** 5 — Plan
**Parent Project:** P2 — `projects.md`
**Parent Goal:** Studio Goal — `project_aurora.md`
**Built:** 2026-05-05
**Status:** Active

---

## Milestones

### M1 — Core Development Toolchain
*State: Godot installed and a starter project committed to GitHub. VS Codium configured with GDScript support. ComfyUI running locally with a confirmed working inference.*

**Dependencies:** None — all installs are local and independent of other P2 milestones.

### M2 — AI Pipeline & Creative Tools
*State: ComfyUI workflows validated for concept art and reference generation. AI tools for writing support and audio reference identified and accessible. AI strategy inputs reviewed and distilled into a one-page studio AI playbook.*

**Dependencies:** M1 complete. ComfyUI must be running before workflows can be built.

### M3 — Domain & Studio Identity Infrastructure
*State: Studio domain registered and pointing to a holding page or minimal site. Studio email address active. Age Gate and Privacy Policy drafted (can be placeholder until a game ships).*

**Dependencies:** M1 complete (no hard dependency, but toolchain should be stable before committing to recurring hosting costs).

### M4 — Subscriptions Baseline
*State: All active subscriptions catalogued in a ledger (finance/subscriptions.md or finance ledger). Monthly recurring cost baseline documented. Unnecessary or redundant tools cancelled or deferred.*

**Dependencies:** M2 and M3 complete — all tools needed for the studio should be confirmed before locking the cost baseline.

---

## Sequencing

```
M1 → M2 ─┐
          ├→ M4
M1 → M3 ─┘
```

M1 is the prerequisite for all others. M2 and M3 can run in parallel once M1 closes. M4 closes only after M2 and M3 are both done.

---

## Dependencies

| Dependency                              | Type      | Required By    | Status                          |
| --------------------------------------- | --------- | -------------- | ------------------------------- |
| P1 fully closed (EIN, bank account)     | External  | M3, M4         | ✓ Met 2026-05-05                |
| Godot installed                         | M1 output | M2             | ✓ Met 2026-05-06                |
| ComfyUI running                         | M1 output | M2             | ✓ Met 2026-05-06                |
| Domain registered                       | M3 output | M4 cost review | Not available                   |

---

## Decision Rules

- **Godot version:** Default to current stable (4.x). Only choose LTS if a specific plugin or compatibility reason requires it. Record the decision in Task 1 of M1.

- **ComfyUI hardware constraint:** If local GPU is insufficient for meaningful inference, evaluate a lightweight cloud fallback (e.g., RunPod, Vast.ai) before committing to a local-only pipeline. Note the constraint in this file.

- **Domain registrar:** Prefer Namecheap or Cloudflare Registrar for simplicity and cost. Avoid bundled hosting upsells — use separate hosting or a static host (GitHub Pages, Cloudflare Pages) for the holding page.

- **Subscription audit scope:** Include all recurring charges touching the studio — software, cloud storage, AI tools, domain, hosting, and any personal tools primarily used for studio work. Apply a "does this earn its keep in the next 90 days?" test. Defer or cancel if not.

- **P3 domain overlap:** Domain registration may be a natural overlap between P2-M3 and P3-M1. Whichever project reaches it first owns the task. Log it in the other project's review notes to avoid duplication.

---

## Plan Execution Log

*Updated when milestones close or decision rules are triggered.*

| Date       | Milestone | Event                                       |
| ---------- | --------- | ------------------------------------------- |
| 2026-05-05 | —         | Plan built. P1 fully closed. M1 tasks generated in tasks.md. |
| 2026-05-06 | M1        | Closed. All 6 tasks completed. Godot 4.x stable installed, VS Codium configured, GitHub repo live with starter project, ComfyUI inference confirmed. M2 and M3 unlocked — both can run in parallel. |
| 2026-05-06 | M3        | Domain and email resolved via P3-M2 (P3 reached it first). emberhorizonstudios.com registered on Cloudflare, jacobodonnell@emberhorizonstudios.com active on Google Workspace. P2-M3 domain/email tasks closed without duplication. Holding page and public alias still needed — owned by P3-M2. |
| 2026-05-10 | M2        | Closed. ComfyUI workflows validated (txt2img + img2img). Prompt guide in `comfyui-prompt-guide.md`. Writing: Claude confirmed. Audio: Suno + ElevenLabs accounts created; Piper TTS and Kokoro TTS installed locally. AI playbook written to `studio-ai-playbook.md`. M4 unlocked — begin subscriptions baseline. |
| 2026-05-10 | M4        | Closed. Single recurring cost: Claude Pro $20/mo. All other tools free tier or local. Ledger in `finance/subscriptions.md`. **P2 fully closed.** |
