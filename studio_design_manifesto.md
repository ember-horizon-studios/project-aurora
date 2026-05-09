# Studio Design Manifesto — Ember Horizon Studios

*This document defines what this studio makes and why. Reference it before starting any new game. If a design decision conflicts with this, the decision is probably wrong.*

---

## Core Vision

**Mission Statement**

Ember Horizon Studios makes games where the world itself is the text. Technical craft and conceptual depth are not traded against each other — both are required. The goal is to make players feel something that stays with them: not the thrill of winning, but the quiet awe of having genuinely understood something. That feeling is earned, never delivered.

**Design Pillars**

Four principles that must be present in every game. If a feature, mechanic, or design decision cannot be justified against at least one of these, it doesn't belong.

1. **The World Teaches Itself.** No tutorials. No waypoints. No hints. If it's in the world, a paying-attention player can find it. The game establishes its own language — through repetition, through contrast, through the way things are arranged — and trusts players to learn it.

2. **The Mechanic Is the Meaning.** Story and system are inseparable. What a player *does* carries emotional weight, not just what they're *told*. The design succeeds when you can't separate the narrative from the mechanic.

3. **Convention Is a Foundation, Not a Ceiling.** Genre tropes exist to establish player literacy — use them. Then build something on top that couldn't exist without them. The game should look familiar from the outside and be surprising from the inside.

4. **Nothing Ships Unfinished.** Polish is not a final layer — it's a standard applied throughout. Every player-facing element ships complete. No rough edges, no placeholder states, no "we'll fix it post-launch." If it isn't ready, it doesn't go in.

**Target Player Experience**

The player finishes the game — or finishes a five-minute run — and sits with it. Something stuck. Not the fading buzz of a clean win, but a quieter residue: the sense that the world (or the system, or the room they were just trapped in) revealed something true, and they're different for having seen it. The feeling after *Outer Wilds* ends. The unease that follows a *Buckshot Roulette* round you barely won. The slow chill after *Inscryption* makes you look at the table differently. This is the target state. Design backward from it.

**Genre Focus**

The studio's working lane is **roguelite horror and psychological horror**, with freedom to pair those genres with whatever mechanical chassis serves the concept (deckbuilders, sims, deduction games, rhythm games — whatever earns its place). Horror is the constant; the form is negotiable. The throughline is *lasting effect*: a game that the player can't stop thinking about an hour, a day, or a week later.

This is a focus, not a fence. A non-horror concept can still be made here if it satisfies the four pillars and produces the same lasting effect.

---

## Gameplay Philosophy

**The "Fun" Mandate**

Engagement at Ember Horizon comes from *a loop that doesn't let go*. The mechanic generates dread, recognition, or quiet awe — sometimes all three at once. Whether the player is making a slow-burn deduction or a thirty-second call under pressure, the texture is the same: *something is being communicated through play, and the player can feel it land.*

This is not the dopamine of a well-tuned Skinner box. It is also not the patient comprehension of a forty-hour exploration game. Both ends of that range are valid; what matters is that the loop carries weight. A single round of a five-minute game can stay with a player as long as a twenty-hour campaign — when the mechanic *is* the meaning.

**Approach to Difficulty**

Earned mastery. The game is not easy, but it does not punish arbitrarily. Difficulty is cognitive and perceptual — the challenge is in reading the situation correctly, recognizing the pattern, holding your nerve when the moment demands it. Players struggle because they haven't seen what's there yet. The moment of seeing is the reward.

In short-loop horror specifically, mastery is also somatic: managing your own response to dread is part of skill. A practiced player isn't fearless — they're composed. The game should reward composure, not punish hesitation.

Accessibility and mastery are not opposites: a player can engage at a surface level without being blocked, but depth is there for those who look.

**Replayability**

Procedural variety is a tool, not a crutch. It earns its place when each run is a fresh *reading* of the same system — when the rules stay constant but the situation forces new judgment, and the player keeps discovering something the system has always been saying. *Buckshot Roulette* and *Inscryption* use procedural and shifting elements to keep the mechanic's edge sharp; that is the right reason to use them.

If a run is interchangeable with the previous run, the proc-gen is wallpaper. Cut it. Replayability has to deepen the loop, not stretch it. A second playthrough — or a hundredth — must reveal something the first one couldn't.

**Innovation vs. Convention**

Establish the genre's foundation. Make the player fluent in the expected language — the roguelite run, the horror beat, the simulation rhythm, whatever chassis the game uses. Then build something on top that recontextualizes the form. The subversion should feel inevitable in retrospect, not arbitrary.

---

## Areas of Design

**Systems Design**

Systems exist to communicate. Every rule, every interaction, every constraint is a sentence in the world's language. Systems must be internally consistent — the player should be able to form hypotheses and test them. Surprise is acceptable; contradiction is not.

**Narrative Design**

Story lives in the world, not above it. What happened is written into the space — objects, arrangement, absence, change over time. No cutscenes that could have been mechanics. No exposition that could have been discovery. The player reconstructs meaning; the game does not deliver it.

**World and Space Design**

Space is a communicator. The layout of a room, the objects on a desk, the path a player is nudged toward — all of it is authorial. Every space should be readable. A player who pays attention should be able to understand something about the world by moving through it.

**UX / UI & Accessibility**

The interface should never break immersion or call attention to itself. UI exists to serve the world, not to annotate it. Every game ships with colorblind support, remappable controls, and readable type at any screen size. Accessibility is a design requirement, not a post-launch addition.

---

## Technical & Production Standards

**Prototype First, Always**

No art commitment before a gray-box prototype answers: *does the core mechanic create the intended experience?* The prototype does not need to be beautiful. It needs to prove the concept feels the way it should. If it doesn't feel right without art, it won't feel right with it.

**Scope Is a Design Decision**

Scope follows concept — there is no target game length. A 3-hour game with one idea executed completely is better than a 20-hour game that dilutes it. When in doubt, cut. When cutting feels wrong, that's a sign the feature belonged. Cut everything else.

Scoping rule: *if a feature cannot be justified against a design pillar, it is cut, not deferred.*

**Pipeline Integrity**

Tools and workflows are part of the product. A system that requires code changes to tweak a design value is broken. Iteration speed is a quality standard — the faster the studio can test ideas, the better the final game.

---

## Studio Operating Principles

*Solo-studio-specific commitments that govern how this work gets done.*

- **Failure is data.** A prototype that doesn't work told you something true. Log what it told you and move on.
- **Play it weekly.** If the prototype isn't being played, the project is drifting. Playing it is the feedback loop.
- **Reference this document.** If a design decision is hard to make, check it against the pillars. One of them will give an answer.
- **Ship complete things.** Nothing leaves this studio half-done. That includes prototypes shown externally, devlog clips, and store pages.

---

*Last updated: 2026-05-09 — added genre focus (roguelite/psychological horror) and rewrote Gameplay Philosophy around loop-based dread alongside slow comprehension.*
