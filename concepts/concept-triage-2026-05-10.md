# Concept Triage — Ember Horizon Studios
**Date:** 2026-05-10
**Source:** `roguelite-horror-ideas.md` (17 concepts)
**Triage Gate:** Pre-P4 unlock pass. Goal: identify one concept to promote to the validated-game project and begin P4 planning.

---

## Scoring Rubric

Five axes, each 1–5:

| Axis | What it measures |
|------|-----------------|
| **Differentiation (D)** | How distinct is this from existing titles? Does it have a clear comp-gap? |
| **Market Signal (M)** | Evidence of audience demand: comp sales, streaming potential, wishlist angle |
| **Personal Resonance (R)** | Does this feel like *your* game? Will you sustain it for 6–12 months solo? |
| **Solo Feasibility (F)** | Can one developer ship a scope-floor version without collaborators? |
| **Pillar Fit (P)** | How well does it satisfy all four studio design pillars (see below) |

**Studio Pillars:**
1. The World Teaches Itself — no tutorials; rules absorbed through the loop
2. The Mechanic Is the Meaning — dread *is* the system, not narration on top
3. Convention Is a Foundation — uses roguelite literacy, then twists
4. Nothing Ships Unfinished — scope floor a solo dev can actually finish

**Total Score** = D + M + R + F + P (max 25)

**Solo Ship Score** = weighted for debut: (D × 1) + (M × 1) + (R × 1.5) + (F × 2) + (P × 1.5) (max 37.5 — used for ranking)

---

## Triage Results

| # | Concept | D | M | R | F | P | Total | Solo Ship | Flags |
|---|---------|---|---|---|---|---|-------|-----------|-------|
| 5 | **Static** | 5 | 5 | 4 | 4 | 5 | **23** | **34.5** | — |
| 10 | **Pawn** | 4 | 5 | 4 | 4 | 5 | **22** | **33.0** | Shop-state system is engineering challenge |
| 17 | **Standing Wave** | 4 | 4 | 4 | 5 | 5 | **22** | **33.0** | — |
| 15 | **Final Cut** | 5 | 4 | 4 | 4 | 5 | **22** | **32.5** | Per-reel content volume |
| 3 | **The Long Drive** | 4 | 5 | 4 | 4 | 4 | **21** | **31.5** | Audio is load-bearing |
| 13 | **The Reading** | 4 | 4 | 4 | 4 | 4 | **20** | **30.0** | Card art cost lever |
| 16 | **The Kiln** | 4 | 5 | 3 | 5 | 4 | **21** | **30.0** | Tonal sensitivity; low personal resonance |
| 4 | **Lighthouse Keeper** | 5 | 3 | 3 | 5 | 5 | **21** | **29.5** | Low market signal; streaming risk |
| 2 | **Pulse** | 5 | 4 | 3 | 4 | 4 | **20** | **29.0** | Voice acting cost |
| 7 | **Night Shift Audit** | 5 | 3 | 3 | 5 | 4 | **20** | **28.5** | Hard to clip/demo |
| 6 | **Lucky Strike** | 4 | 4 | 3 | 5 | 4 | **20** | **28.5** | Clover Pit comp risk |
| 1 | **Confessional** | 5 | 4 | 4 | 4 | 4 | **21** | **28.0** ⚠️ | Religious sensitivity; voice acting |
| 9 | **Subway Driver** | 4 | 5 | 3 | 4 | 4 | **20** | **28.0** | Low resonance; similar to Long Drive |
| 14 | **Cellar Door** | 3 | 3 | 2 | 5 | 4 | **17** | **24.5** | Overlaps Pawn; low resonance |
| 11 | **Vigil** | 5 | 3 | 5 | 3 | 4 | **20** | **28.0** ⚠️ | Needs collaborator; tonal risk |
| 8 | **Buzzer** | 5 | 3 | 3 | 3 | 3 | **17** | **22.5** ⚠️ | Needs voice work + performance assets |
| 12 | **Conductor** | 5 | 2 | 3 | 2 | 3 | **15** | **19.0** ⚠️ | Needs composer; rhythm tech demanding |

⚠️ = needs collaborator or has a structural risk that blocks solo debut consideration

---

## Top Tier Analysis

### 🥇 Static — Score 23 / Solo Ship 34.5 — **RECOMMENDED**

*Inscryption at a CRT-repair workbench — every TV that comes in plays a problem, and some of the problems aren't electrical.*

**Why it wins:**
- Perfect pillar fit: the repair loop teaches itself, the mechanic (diagnosing the impossible) *is* the horror, it leverages the "workbench sim" roguelite frame audiences already read, and the scope floor (one workbench, 20 TV scenarios, 5 tools) is genuinely solo-shippable.
- Analog horror is enormous on YouTube (Local 58, The Mandela Catalogue) but has almost no commercial-game representation — a real white space.
- CRT shader + pixel art delivers the aesthetic at low production cost. The strongest 5-second clip hook in the batch: a vintage TV showing something that shouldn't exist.
- Highest combined score AND highest solo ship score in the batch.

**Risk to manage:** Per-TV "broadcast" content is the cost driver. Mitigation: procedurally distort footage or use static art sequences rather than full video. Cap broadcast content at 20 scenarios for scope floor; 10 is MVP.

**Verdict: Promote to P4.**

---

### 🥈 Pawn — Score 22 / Solo Ship 33.0

*Strange Horticulture meets Buckshot Roulette — a pawnshop counter at night where the wrong appraisal lets the wrong thing into your shop.*

Strong across all axes. The item-taxonomy mechanic has commercial proof (Strange Horticulture, 300k+ reviews). The shop-state-changing system is the one engineering challenge that needs a design spike before committing. Strong backup if Static encounters an unforeseen blocker.

---

### 🥉 Standing Wave — Score 22 / Solo Ship 33.0

*Iron Lung as a shortwave radio operator — the stations cycle, and one has started responding to you specifically.*

Tied with Pawn on solo ship score. Pure audio-and-UI game — lowest art ceiling in the top tier. Numbers-station aesthetic is niche but deeply committed audience. The "one room, one rig" constraint makes this the easiest debut scope in the batch. If you want to ship something in under 6 months, this is the path. Keep as P4 alternate.

---

## Collaborator-Dependent Concepts — Hold for Later

These scored well on differentiation and resonance but require voice actors, composers, or performance assets that push them past solo-debut feasibility:

- **Vigil** (5 resonance — revisit when you have a collaborator pipeline)
- **Confessional** (religious sensitivity + voice work — revisit post-debut)
- **Conductor** (needs a composer — long-term project)
- **Buzzer** (performance assets are the whole game)

---

## Archived / Deprioritized

- **The Cellar Door** — overlaps Pawn mechanically; lower resonance; archive.
- **Lucky Strike** — comp risk with Clover Pit without stronger differentiation; hold in backlog.
- **The Subway Driver** — low resonance; similar structure to The Long Drive; archive.

---

## Decision

**Concept promoted to P4: Static**

Next step: build `plan-debut-title.md` using Static as the subject. First milestone should be a core-loop prototype — the repair interaction and one working TV scenario end-to-end in Godot.

---

## Gate A — Backlog Items Processed

Per the open Weekly Review checklist item:

| Backlog Item | Gate A Decision |
|---|---|
| Evaluate business consultant (Gemini gem reference) | ❌ Defer — no clear need at current studio scale. Re-audit when P4 reaches prototype phase. |
| Age Gate + Privacy Policy on website | ✅ Promote to P3 successor task — schedule before any game has a Steam page. Low urgency until P4-M1. |
| Studio design manifesto | ✅ Promote — write before P4 planning begins. Needed to keep design decisions anchored. 1–2 page doc, M energy, ~45 min. |
| Game conventions document | ❌ Hold — belongs to P4 plan; generate after P4 plan is built and a concept is in prototype. |
