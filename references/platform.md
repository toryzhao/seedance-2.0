## Platform Overview

**Seedance 2.0** is developed by **ByteDance** and accessed primarily through:

- **Dreamina (即梦):** [jimeng.jianying.com](https://jimeng.jianying.com) — full web interface, two entry modes
- **CapCut / Jianying app:** Mobile integration
- **Xiaoyunque (小云雀) app:** Mobile-first access
- **Volcengine API:** Programmatic access (model string: `Doubao-Seedance-2.0`)
- **Doubao app:** Mobile with simplified interface

The platform uses a **Dual-Branch Diffusion Transformer** architecture for simultaneous video and audio generation.

---

## Platform Constraints

**VERIFIED Q1 2026**

| Parameter | Limit | Notes |
|-----------|-------|-------|
| **Generation duration** | 4–15 seconds (web), 5–10s (some mobile) | Adjustable slider |
| **Resolution** | 720p default, up to 1080p (2K for premium) | No native 4K |
| **Image inputs** | Up to 9 | JPG/PNG/WEBP, <30MB each |
| **Video inputs** | Up to 3 | <50MB each, <15s each |
| **Audio inputs** | Up to 3 (MP3) | Total ≤15s combined |
| **Total file inputs** | 12 maximum | The "Rule of 12" |
| **Audio output** | Dual-channel stereo | Synced to video length |
| **Aspect ratios** | 16:9 / 9:16 / 1:1 / 4:3 | 9:16 changes composition rules |

### Text Prompt Length

The exact character limit for text prompts is not officially documented with a hard number. In practice, Chinese-language creators routinely use prompts of **1000–3000+ Chinese characters** with success on the Dreamina web interface. The API may have different constraints. English prompts tend to require more characters for equivalent semantic density.

**Practical guidance:** Keep prompts as concise as possible — not because of a hard cutoff, but because shorter, structured prompts consistently outperform verbose ones. Research across 150+ prompt variations shows that **30–100 word English prompts** (or roughly 50–200 Chinese characters for simple scenes, up to 500–1000 for complex choreography) produce the best motion quality. Beyond that range, the model's attention dilutes and motion degrades.

**Budget discipline:** Even without a confirmed hard limit, treat prompt length as a scarce resource. Every word should be verifiable in-frame or in-audio. If you cannot point to what a phrase controls, delete it.

### Real-Face Restriction

Real human face references require identity verification or authorization on the platform. Workarounds include using AI-modified portraits (run through an image model first) or illustrated/3D character references.

---
