
## Module 01: Prompt Architecture

### The Five-Layer Stack (Motion-First Order)

The model prioritizes motion coherence. Structure prompts to establish subject → define action → control camera → set style → add constraints.

1. **SUBJECT** — who/what is central (the anchor point for all motion)
2. **ACTION** — what changes (primary motion verb + physics/timing details)
3. **CAMERA** — framing + movement + speed + angle
4. **STYLE & LIGHT** — one strong visual anchor + named light source
5. **CONSTRAINTS** — what must stay consistent, what to avoid

**Optional Layer 6: SOUND** — ambient bed + key SFX + music + silence design.

### One Primary Motion Verb Per Shot

Multiple competing actions ("walks while turning and gesturing and looking around") create chaos. For complex choreography, break actions into sequential beats with timestamps or use a reference video.

### Syntax Conventions (Reliable)

- **Commas** sequence events within a beat: `"door opens, light spills in, dust rises."`
- **Periods** separate layers: new layer = new sentence.
- **Parentheses** for technical asides: `"(rack focus foreground→background)."`
- **Explicit temporal markers** for multi-scene: `"Scene 1: ... Scene 2: ... Scene 3: ..."`
- **Timestamps** for precise control: `"0–3s: ... 3–7s: ... 7–END: ..."`
- Avoid semicolons and long em-dash chains.
- Prefer positive specification over long negative lists.

### Prompt Hygiene and Anti-Slop

**Avoid empty filler:** "cinematic," "epic," "masterpiece," "ultra-real," "award-winning," "viral."

**Replace with controls:**
- ❌ "cinematic lighting" → ✅ "single hard key 45° camera-left, warm amber, deep shadow fill."
- ❌ "epic" → ✅ "wide shot, slow push-in, rising wind, sustained low drone, crescendo at 6s."
- ❌ "high quality" → ✅ "stable exposure, no flicker, consistent character design, clean edges."
- ❌ "8K" → (delete unless combined with a render-engine style token; see Module 07).

**Conflict check:** Never combine mutually exclusive instructions. Common conflicts:
- locked-off + handheld
- bright flat + low-key shadows
- rapid cuts + long-take
- slow graceful + energetic pacing

**Deletion rule:** If a word cannot be verified in-frame or in-audio, delete it or convert it into something observable.

### ⚠️ COPYRIGHT, IP, LIKENESS & SAFEGUARDS

Seedance 2.0 has strict content filters, tightened under pressure from the Motion Picture Association and Disney. The platform scans both text and uploaded images before generation.

**Hard blocks (will trigger rejection):**
- Celebrity faces/voices, politicians, influencers, private individuals without authorization
- Named franchise characters, IP keywords ("Iron Man," "Mickey Mouse," "Harry Potter")
- Scene recreations of copyrighted content
- Brand logos when the goal is replication
- Visual uploads of recognizable copyrighted characters (even without naming them)

**Do this instead:**
- Use original characters, original worlds, original props
- Use archetypes and film grammar (lens, light, pacing), not IP names
- Describe characters generically: "red armored robot suit" not "Iron Man"
- Use AI-generated or illustrated character references

**If blocked:** Remove named IP/real people. Redesign toward originality. Do not iterate toward "almost forbidden."

⚠️ This skill is not legal advice. Commercial use should receive professional legal review.

---

## Module 01A: Universal Reference System

### Paradigm Shift: Reference-Driven Workflow

Seedance 2.0's core breakthrough is **全能参考 (Universal Reference)**. The old workflow was "write detailed text → hope for the best." The new workflow is **"provide the right reference assets → write minimal orchestration text."**

Reference assets replace manual art direction. You don't need to manufacture keyframes if you have good reference materials. The model's aesthetic becomes **"your selection is the only standard."**

### Platform Entry Modes

Dreamina offers two entry points — choose the right one:

1. **First/Last Frame mode (首尾帧):** For single image + text. Use when you have one reference image and want to animate it.
2. **Universal Reference mode (全能参考):** For multi-modal combinations. Use whenever you have more than one image, or any video/audio references. **This is the mode that unlocks Seedance 2.0's full power.**

**Rule of thumb:** If your inputs are just one image + text → First/Last Frame. Everything else → Universal Reference.

### Input Limits

