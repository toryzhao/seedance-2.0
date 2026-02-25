---

## Module 00B: When to Direct vs. Delegate

**This is the most important strategic decision in Seedance 2.0 prompting.** The model has genuine director intelligence — world knowledge, narrative instinct, and cinematographic taste. Choosing the wrong level of specification wastes effort or suppresses the model's strengths.

### The Delegation Spectrum

#### Level 1 — Pure Intent (≤30 words)

**Use when:** The scene involves common knowledge domains (food, brands, sports, everyday activities), and you trust the model's editorial judgment.

**Pattern:** `[Subject/scenario], [one style/mood word], 注意分镜编排 (pay attention to shot arrangement).`

**Example:**  
```
生成一个精美高级的兰州拉面广告，注意分镜编排
(Generate an elegant premium Lanzhou ramen ad, pay attention to shot arrangement)
```

**Result:** The model independently chose slow-motion for noodle-pulling, arranged multiple shots, selected appropriate music, and made all cinematographic decisions. Total prompt: 18 Chinese characters.

**When this works:** The model knows how ramen is made, understands MUJI's brand philosophy, knows proper exercise form, understands film genre conventions. For these domains, **less is more**.

#### Level 2 — Guided Direction (30–100 words)

**Use when:** You have a specific vision but want the model to handle technical execution. **Most common mode for quality results.**

**Pattern:** Subject + action + environment + one camera note + one style anchor.

#### Level 3 — Time-Segmented Direction (100–300 words)

**Use when:** You need specific events at specific moments, multi-shot sequences, or narrative beats.

**Pattern:** Time-stamped segments (0–3s, 3–7s, 7–END) with camera and sound layers.

#### Level 4 — Full Choreography (300–1000+ words)

**Use when:** Fight scenes, precise product demos, frame-accurate lip-sync, or any scene requiring per-second control.

**Pattern:** Per-shot specifications with numbered cameras, impact physics, particle effects, and sound design per beat.

### Decision Framework

**Ask:** "Does the model already know how to shoot this?"  
- If yes → Level 1–2
- If you need something novel, unusual, or precisely timed → Level 3–4

**Ask:** "Am I better at this than the model?"  
- For common cinematography and editing → probably not, delegate
- For your specific creative vision → direct precisely

### Anti-Pattern

❌ Writing Level 4 prompts for Level 1 scenarios. Over-specification of common scenes often produces worse results than delegation because the model's trained instincts get overridden by your amateur shot-listing.

