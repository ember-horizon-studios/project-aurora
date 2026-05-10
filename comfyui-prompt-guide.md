# ComfyUI Prompt & Settings Guide — Ember Horizon Studios

*Reference for P2-M2 workflow validation. Use these during ComfyUI testing to calibrate the pipeline against the studio's aesthetic before committing to a checkpoint model.*

*Aesthetic target: psychological horror, quiet dread, slow unease. Not gore, not shock. Reference games: Buckshot Roulette, Inscryption, Faith, Mouthwashing, Crow Country.*

---

## Aesthetic Vocabulary

Before prompting, internalize the target feeling:
- **Texture over spectacle.** Grime, worn surfaces, analog artifacts, VHS noise, institutional decay.
- **Wrongness, not threat.** Something is off. The light is wrong. The proportions don't sit right. Nothing is attacking you — yet.
- **Emptiness with presence.** Spaces that feel inhabited but aren't. Objects arranged too deliberately. Absence that implies something.
- **Flat affect.** Characters who don't react the way they should. Eyes that look at you wrong.

---

## Sample Prompts

### 1. Environment — Abandoned Interior (Concept Reference)

**Use case:** Establishing visual language for indoor horror spaces. Test run for a new checkpoint.

**Positive:**
```
abandoned institutional interior, flickering fluorescent light, cracked linoleum floor, water stains on ceiling tiles, rusted metal lockers, long hallway, single bare bulb, deep shadows, muted color palette, photorealistic, cinematic, 4k, film grain, high detail, unsettling, liminal space, psychological horror
```

**Negative:**
```
bright colors, daylight, sunshine, people, cartoon, anime, illustration, low quality, blurry, deformed, watermark, text, oversaturated, gore, blood, jumpscares, modern clean design, neon
```

---

### 2. Character — Ambiguous Figure (Concept Reference)

**Use case:** NPC or antagonist silhouette exploration. Testing model's ability to produce uncanny human forms.

**Positive:**
```
lone figure standing at end of hallway, backlit, silhouette, face obscured, slightly wrong proportions, too tall, still, hospital gown or worn coat, muted desaturated tones, foggy atmosphere, cinematic lighting, photorealistic, film grain, unsettling, psychological horror, high contrast
```

**Negative:**
```
clear face, smiling, friendly, bright lighting, cartoon, anime, gore, blood, monster, weapons, low quality, deformed hands, multiple people, crowd, daylight, oversaturated
```

---

### 3. Object / Item — Diegetic Horror Prop (Concept Reference)

**Use case:** Inventory items, key objects, story props. Testing detail fidelity and texture quality.

**Positive:**
```
close-up product shot, worn playing cards on wooden table, candlelight, dramatic side lighting, aged paper texture, handwritten ink annotations, occult symbols, shadows, macro photography, photorealistic, film grain, isolated object, dark background, high detail
```

**Negative:**
```
plastic, modern, clean, bright, cartoon, anime, low quality, multiple objects cluttered, blurry, watermark, oversaturated, neon, digital art style
```

---

### 4. Environment — Exterior at Night (Atmosphere / Mood Reference)

**Use case:** Key art mood exploration, cover art research, establishing environmental tone.

**Positive:**
```
rural road at night, single streetlight, dense treeline, thick fog, overcast sky, no stars, gravel, old telephone poles, distant light in treeline, desaturated, muted green and amber tones, photorealistic, cinematic wide shot, film grain, eerie, quiet dread, psychological horror
```

**Negative:**
```
city, urban, daylight, sunshine, people, cartoon, anime, neon lights, colorful, fantasy, monsters visible, low quality, blurry, watermark
```

---

### 5. UI / Card / Diegetic Interface (Concept Reference)

**Use case:** Deckbuilder or tabletop-adjacent UI explorations. Testing fine detail and graphic element fidelity.

**Positive:**
```
tarot card design, aged parchment, woodcut illustration style, black ink, intricate linework, skull and candle motif, gothic typography, worn edges, yellowed paper, flat lay photography, high detail, dramatic lighting from above, dark atmosphere, occult
```

**Negative:**
```
digital, modern, glossy, bright colors, cartoon, anime, low quality, blurry, watermark, photorealistic face, neon, fantasy color palette
```

---

## Img2Img Prompts

For img2img, your text prompt guides the *direction* of the transformation — the source image provides structure. Keep prompts leaner; let the image carry the composition.

### General img2img positive (apply on top of any of the above):
```
[keep core subject description], enhanced detail, cinematic lighting, film grain, photorealistic, horror atmosphere, muted palette
```

### General img2img negative (applies to all):
```
cartoon, anime, low quality, blurry, deformed, watermark, oversaturated, bright colors, gore, text
```

**Denoise strength guidance:**
| Goal | Denoise |
|---|---|
| Refine while keeping composition | 0.35 – 0.50 |
| Significant style shift, keep loose structure | 0.55 – 0.70 |
| Near-full regeneration (loose reference only) | 0.75 – 0.90 |

Start at 0.45 for most iteration work. Go higher only when the source is a rough sketch or blocking reference.

---

## KSampler Settings Reference

### Text-to-Image (Concept Exploration)

| Setting | Value | Notes |
|---|---|---|
| Steps | 25–35 | 25 for fast iteration; 35 for final review |
| CFG Scale | 7–8 | 7 for flexibility; 8 for tighter prompt adherence |
| Sampler | DPM++ 2M Karras | Fast, high quality, good for photorealistic |
| Scheduler | Karras | Pairs with DPM++ 2M for smooth output |
| Denoise | 1.0 | Always 1.0 for pure txt2img |

### Text-to-Image (Final / High Detail Pass)

| Setting | Value | Notes |
|---|---|---|
| Steps | 40–50 | Diminishing returns above 50 on most models |
| CFG Scale | 7.5 | Split the difference — stays controllable |
| Sampler | DPM++ 2M Karras or DDIM | DDIM slightly crisper on fine detail |
| Scheduler | Karras | |
| Denoise | 1.0 | |

### Img2Img (Iteration / Refinement)

| Setting | Value | Notes |
|---|---|---|
| Steps | 20–30 | Fewer steps needed — source image front-loads structure |
| CFG Scale | 6–7.5 | Lower CFG gives the source image more authority |
| Sampler | DPM++ 2M Karras | |
| Scheduler | Karras | |
| Denoise | 0.35 – 0.70 | See denoise guidance above |

### Upscale Pass (via HiRes Fix or Ultimate SD Upscale)

| Setting | Value | Notes |
|---|---|---|
| Steps | 15–20 | Upscale passes need fewer steps |
| CFG Scale | 6 | Keeps the upscale faithful to the base |
| Denoise | 0.30 – 0.45 | Low — you're adding detail, not redrawing |
| Upscale by | 1.5–2x | 2x for final art; 1.5x to stay manageable on local GPU |

---

## Sampler Quick Reference

| Sampler | Best For |
|---|---|
| DPM++ 2M Karras | General use, photorealistic, fast — use this as default |
| DPM++ SDE Karras | More variation per seed; good for exploring style range |
| Euler a | Fast and loose; good for rough concept passes |
| DDIM | Consistent and crisp on fine details; good for final passes |
| LCM | Extreme speed (4–8 steps); quality tradeoff — use for rapid sketch-level ideation only |

---

## CFG Scale Effect

| CFG | Behavior |
|---|---|
| 4–5 | Loose — model interprets freely. More dreamlike, less literal. |
| 6–7 | Balanced — good starting range for most work |
| 7.5–8 | Prompt-adherent — closer to literal interpretation |
| 9+ | Over-cooked — tends toward artifacts, oversaturation, and stiffness. Avoid. |

---

## Workflow Testing Protocol (P2-M2 Task 2 & 3)

For task 2 (txt2img workflow validation):
1. Run prompts 1 and 4 (environment) on your chosen checkpoint at default settings (25 steps, CFG 7, DPM++ 2M Karras).
2. Check: Is the horror tone present without explicit gore? Is the color palette reading as muted/desaturated? Is the level of detail acceptable for reference use?
3. If yes — record the checkpoint and settings in `plan-studio-systems.md` and call workflow validated.
4. If no — adjust CFG up/down first before changing sampler. If still off, the checkpoint model is wrong.

For task 3 (img2img workflow validation):
1. Take one output from task 2 and run it through img2img at denoise 0.45.
2. Modify the prompt slightly (e.g., add "winter, snow, frost" or "summer, overgrown, vines") to test how well the loop responds to direction.
3. Check: Does the output maintain the composition while incorporating the change? If yes — the feedback loop works.

---

*Last updated: 2026-05-10*
