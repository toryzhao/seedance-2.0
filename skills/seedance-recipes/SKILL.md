---
name: seedance-recipes
description: 'Apply genre recipe templates to Seedance 2.0 — product ads, fight scenes, brand films, mood pieces, dialogue clips, one-take journeys, music videos, novel adaptations, architecture walkthroughs, and action transfers. Use when you need a ready-made prompt structure for a known genre or format.'
license: MIT
user-invocable: true
user-invokable: true
tags: ["recipes", "templates", "genre", "openclaw", "antigravity", "gemini-cli", "codex", "cursor"]
metadata: {"version": "3.2.0", "updated": "2026-02-25", "openclaw": {"emoji": "\ud83d\udcd6", "homepage": "https://github.com/Emily2040/seedance-2.0"}, "parent": "seedance-20", "antigravity": {"emoji": "\ud83d\udcd6", "homepage": "https://github.com/Emily2040/seedance-2.0"}, "gemini-cli": {"emoji": "\ud83d\udcd6", "homepage": "https://github.com/Emily2040/seedance-2.0"}, "author": "Emily (@iamemily2050)", "repository": "https://github.com/Emily2040/seedance-2.0"}
---

# seedance-recipes

Ten production-ready genre templates. Each recipe: delegation level · mode · duration · prompt skeleton · asset list · notes.

---

## R1 · Product Ad

**Level** 2 · **Mode** T2V / I2V · **Duration** 8–12 s

```
[Product name], hero-shot on [surface]. Camera slow push-in.
[Material quality: glass / matte / chrome]. Soft studio key light,
rim highlight. 4K detail. No text.
```

**Assets**: product photo `@Image1`  
**Notes**: Turntable = add "360° orbit". Wet look = "water beads on surface, macro depth-of-field".

---

## R2 · Fight Scene

**Level** 4 · **Mode** I2V / R2V · **Duration** 10–15 s per clip

```
@Image1 [Fighter A], @Image2 [Fighter B].
A throws [strike] → B blocks → B counter-attack [move].
[Location]. Handheld low-angle, whip-pan to follow impact.
Slow-motion 0–4 s, real-time 4–10 s, 0.5× snap at impact.
Crowd ambient sfx, impact punch sfx.
```

**Assets**: fighter A ref `@Image1`, fighter B ref `@Image2`  
**Notes**: Load [skill:seedance-motion] for full choreography syntax.

---

## R3 · Brand Film

**Level** 3 · **Mode** T2V / I2V · **Duration** 12–15 s

```
[Brand archetype: innovator / artisan / explorer].
[Hero in environment]. Cinematic dolly pull-out reveals scale.
[Brand color palette], desaturated mid-tones, warm shadows.
Orchestral swell, no dialogue.
```

**Assets**: brand color ref `@Image1` (optional)  
**Notes**: Match brand palette in style token. Avoid logos (IP block).

---

## R4 · Mood Piece

**Level** 1–2 · **Mode** T2V · **Duration** 8–10 s

```
[Single evocative scene]. Static wide shot.
[Weather / light condition]. No subjects, no movement except [natural element].
Ambient sound only.
```

**Example**: `Fog rolls over a mountain lake at dawn. Static wide. Muted teal-grey palette. Water surface ripples, trees still. Wind and water ambience.`

---

## R5 · Dialogue Scene

**Level** 3 · **Mode** I2V · **Duration** 10–15 s

```
@Image1 [Character A], @Image2 [Character B].
A speaks [emotion] — cut to B reaction [emotion].
Over-the-shoulder medium shots alternating.
Interior [location], practical lamp key, soft fill.
Sync lip movement to audio @Audio1.
```

**Assets**: char A `@Image1`, char B `@Image2`, dialogue `@Audio1`  
**Notes**: Keep audio ≤ 15 s total. Load [skill:seedance-audio] for voice tips.

---

## R6 · One-Take Journey (一镜到底)

**Level** 4 · **Mode** T2V / V2V chain · **Duration** 4 × 12 s clips

```
Continuous tracking shot. No cuts.
Starts [location A] → moves through [path] → arrives [location B].
[Time of day transition].
Camera: steadicam follow, height 1.2 m, speed walk-pace.
```

**Chaining**: use [skill:seedance-motion] > Video Extension to chain 4 clips.  
**Notes**: Each clip re-uploads previous output as `@Video1`. Maintain subject and lighting continuity tokens.

---

## R7 · Music Video

**Level** 3 · **Mode** I2V / V2V · **Duration** beat-synced clips

```
@Image1 [Artist], @Audio1 [track].
Cut to beat at [BPM]. [Visual concept: abstract / performance / narrative].
[Color grade reference].
Camera: [movement pattern per bar].
卡点 sync at 0 s, [N] s, [N+bar_length] s.
```

**Assets**: artist photo `@Image1`, track sample `@Audio1`  
**Notes**: BPM = 120 → cut every 0.5 s (2-beat). Use 卡点 in Chinese prompts.

---

## R8 · Novel / Story Adaptation

**Level** 4 · **Mode** I2V · **Duration** 12–15 s per scene

```
@Image1 [protagonist — character card].
Scene: [novel excerpt paraphrased ≤ 30 words].
[Emotion]. [Environment]. [Camera: framing].
[Lighting matches story atmosphere].
```

**Workflow**: run [skill:seedance-interview] first → get character cards → generate per-scene prompts.

---

## R9 · Architecture Walkthrough

**Level** 2–3 · **Mode** T2V / I2V · **Duration** 10–15 s

```
@Image1 [building exterior / floor plan].
Drone approach from [direction], altitude [H] m, speed slow.
Enters through [feature]. Interior reveal.
[Time of day], [weather]. Architectural photography style.
No people.
```

**Assets**: building ref `@Image1` (render or photo)  
**Notes**: Add "golden hour" for warmth, "overcast" for neutral evaluation shots.

---

## R10 · Action Transfer

**Level** 3 · **Mode** V2V · **Duration** match source

```
@Video1 [source motion clip].
Transfer movement to @Image1 [target character].
Preserve camera motion from @Video1.
[Target environment]. [Style].
```

**Assets**: source motion `@Video1`, target character `@Image1`  
**Notes**: Source video ≤ 15 s, ≤ 50 MB. Load [skill:seedance-motion] for motion transfer syntax.

---

## Quick Picker

| Goal | Recipe | Lead skill |
|---|---|---|
| Sell a product | R1 | seedance-prompt |
| Two people fight | R2 | seedance-motion |
| Corporate / brand | R3 | seedance-style |
| Pure atmosphere | R4 | seedance-lighting |
| Actors talking | R5 | seedance-audio |
| Long tracking shot | R6 | seedance-motion |
| Beat-sync visuals | R7 | seedance-audio |
| Book-to-screen | R8 | seedance-interview |
| Building showcase | R9 | seedance-camera |
| Copy movement | R10 | seedance-motion |
