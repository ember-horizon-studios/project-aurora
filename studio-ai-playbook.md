# Studio AI Playbook — Ember Horizon Studios

*One-page reference. Check this before starting any AI-assisted production task. Last updated: 2026-05-10.*

---

## The Stack

| Role | Tool | Access | Cost |
|---|---|---|---|
| Writing & reasoning | Claude (claude.ai) | Active | Subscription |
| Image generation | ComfyUI (local) | Active | Free (local GPU) |
| Music reference | Suno | Account created | Free tier (non-commercial) |
| Voice prototyping — fast | Piper TTS (local) | Installed | Free |
| Voice prototyping — quality | Kokoro TTS (local) | Installed | Free |
| Voice prototyping — expressive | ElevenLabs | Account created | Free tier |

**Principle:** local tools first, cloud tools when local quality isn't sufficient. Add nothing to the stack unless it earns its keep in the next 90 days.

---

## What Each Tool Does Here

**Claude** — game writing support across the production lifecycle: lore and found-text drafting, NPC dialogue scaffolding, mechanical flavor text (card names, status effects, death messages, item descriptions), tone checking against manifesto pillars. Brief it with the manifesto and strategy docs before any writing task. Never ship Claude output verbatim — use it to get past the blank page, then rewrite for voice.

**ComfyUI** — concept art reference and visual development. Validated workflows: text-to-image (prompt guide: `comfyui-prompt-guide.md`) and img2img iteration. Use for establishing visual language, environment mood, character silhouettes, and UI/card art direction. Not a final art pipeline — output is reference material for production decisions.

**Suno** — reference scoring only. Generate tracks to feel out a scene's emotional tone, communicate direction to a future composer, or prototype adaptive audio concepts. **Do not plan to ship Suno output** without reviewing current licensing terms first and confirming Steam disclosure compliance.

**Piper TTS** — bulk dialogue prototyping. Fast, CPU-based, zero VRAM cost. Use when you need to hear a lot of lines quickly to test whether dialogue reads right in context. Script: `/home/jake/Applications/piper/speak.sh "line" [ryan|lessac|alba]`.

**Kokoro TTS** — character-specific voice work. More natural than Piper, GPU-accelerated. Use when voice quality matters for a specific character or scene test. Close ComfyUI first (VRAM conflict). Script: `cd /home/jake/Applications/kokoro && .venv/bin/python speak.py "line" [voice]`. Voices: `am_fenrir` (deep male), `bf_emma` (composed British female), `am_michael`, `bf_lewis`, `af_heart`, `af_nova`.

**ElevenLabs** — expressive VO prototyping when Kokoro's emotional range isn't enough. Free tier: ~10,000 characters/month. Use sparingly — reserve for key character moments, not bulk dialogue passes.

---

## Use Cases by Production Phase

### Concepting & Prototyping
- ComfyUI → visual tone reference before any art commitment
- Suno → score reference to establish scene feel
- Claude → mechanic flavor text, world-building lore, design pillar checks

### Gray-box / Vertical Slice
- Piper → temp VO for all dialogue (fast, no VRAM cost)
- Claude → branching dialogue scaffolding, NPC voice drafts
- ComfyUI → UI element concepts, card art direction

### Pre-production (art-locked)
- Kokoro or ElevenLabs → character-specific temp VO for playtesting
- Claude → final polish pass on all player-facing text
- ComfyUI → final reference art passed to production pipeline

---

## Platform Disclosure Rules (Steam)

Steam requires disclosure for AI-generated content **consumed by players**. Using AI as a workflow tool (reference images, temp audio, internal drafts) does not require disclosure.

| Content                                               | Disclosure required?                        |
| ----------------------------------------------------- | ------------------------------------------- |
| AI concept art used as internal reference only        | No                                          |
| AI art shipped as in-game asset or marketing material | Yes                                         |
| Suno/Kokoro audio used as internal reference          | No                                          |
| Suno/Kokoro audio shipped in game or trailer          | Yes                                         |
| Claude-drafted text rewritten by human before ship    | No                                          |
| Claude-drafted text shipped verbatim                  | Yes (judgment call — err toward disclosure) |

**Rule of thumb:** if a player sees or hears it, disclose it. Log the decision in the game's production notes so it's not a last-minute surprise before Steam submission.

---

## Guardrails

- **No verbatim AI text ships.** Claude output is always a draft. All player-facing writing passes through a human edit.
- **No AI voice ships without decision.** Piper and Kokoro are prototype tools only until a deliberate call is made to use AI VO in the shipped game. That decision gets logged.
- **No Suno output ships without licensing review.** Confirm current commercial terms and Steam disclosure requirements before any generated track enters a trailer or build.
- **Stack audit at M4.** All subscriptions and tools reviewed for "earns its keep in the next 90 days" before the cost baseline locks.
