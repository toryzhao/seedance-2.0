# 🎬 seedance-20

> **Seedance 2.0 — Quad-Modal AI Filmmaking Skill Library**  
> Text-to-Video · Image-to-Video · Video-to-Video · Reference-to-Video

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-3.6.0-blue.svg)](CHANGELOG.md)
[![Agent Skills](https://img.shields.io/badge/Agent_Skills-Open_Standard-green.svg)](https://agentskills.io/)
[![Antigravity](https://img.shields.io/badge/Antigravity-compatible-orange.svg)](https://antigravity.google/docs/skills)
[![Gemini CLI](https://img.shields.io/badge/Gemini_CLI-compatible-blue.svg)](https://geminicli.com/docs/cli/skills/)
[![Claude Code](https://img.shields.io/badge/Claude_Code-compatible-purple.svg)](https://docs.anthropic.com/en/docs/claude-code/skills)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-compatible-red.svg)](https://clawhub.ai/)
[![GitHub Copilot](https://img.shields.io/badge/GitHub_Copilot-compatible-black.svg)](https://docs.github.com/en/copilot)

**Author:** [Emily (@iamemily2050)](https://github.com/Emily2040)  
**Platform:** [ByteDance Seedance 2.0](https://seed.bytedance.com) · Dreamina · Jimeng  
**Updated:** 2026-02-25 · Q1 2026 release intelligence

---

## What is this?

A production-ready Agent Skill library for **Seedance 2.0** — ByteDance's quad-modal AI video generation system. This skill package teaches any compatible AI coding agent (Claude Code, Antigravity, Gemini CLI, GitHub Copilot, OpenClaw, Cursor, Codex, Windsurf, OpenCode, Firebase Studio) how to:

- Write and validate Seedance 2.0 prompts across all four modes (T2V · I2V · V2V · R2V)
- Direct camera movement, lighting, motion, character consistency, and VFX
- Design native audio, dialogue, and lip-sync for multi-character scenes
- Build post-processing pipelines with ComfyUI and Firebase Studio
- Navigate the Feb 2026 copyright enforcement landscape (Disney, Paramount, MPA, SAG-AFTRA)
- Prompt in 6 languages with native cinematic vocabulary

> ⚠️ **Feb 2026 Status**: Seedance 2.0 API global release was delayed due to copyright enforcement actions. Real-person face uploads paused Feb 15. Content filters tightened for named franchise characters, anime IPs, and streaming originals. Run `seedance-copyright` before every generation.

---

## 📦 Installation

### Universal (all platforms that support the Agent Skills open standard)

```bash
# Antigravity
antigravity skills install https://github.com/Emily2040/seedance-2.0

# Gemini CLI
gemini skills install https://github.com/Emily2040/seedance-2.0

# Claude Code
claude skills install https://github.com/Emily2040/seedance-2.0

# OpenClaw / ClawHub
claude skills install https://github.com/Emily2040/seedance-2.0

# Codex
codex skills install https://github.com/Emily2040/seedance-2.0

# Cursor
cursor skills install https://github.com/Emily2040/seedance-2.0

# Windsurf
windsurf skills install https://github.com/Emily2040/seedance-2.0

# OpenCode
opencode skills install https://github.com/Emily2040/seedance-2.0
```

### Manual installation

Clone or copy the skill folders into your agent's skill directory:

| Platform | Workspace path | Global path |
|---|---|---|
| **Antigravity** | `.agent/skills/seedance-20/` | `~/.gemini/antigravity/skills/seedance-20/` |
| **Gemini CLI** | `.gemini/skills/seedance-20/` | `~/.gemini/skills/seedance-20/` |
| **Firebase Studio** | `.idx/skills/seedance-20/` | — |
| **Claude Code** | `.claude/skills/seedance-20/` | `~/.claude/skills/seedance-20/` |
| **OpenClaw** | `.claude/skills/seedance-20/` | `~/.claude/skills/seedance-20/` |
| **GitHub Copilot** | `.github/skills/seedance-20/` | `~/.copilot/skills/seedance-20/` |
| **Codex** | `.agents/skills/seedance-20/` | `~/.agents/skills/seedance-20/` |
| **Cursor** | `.cursor/skills/seedance-20/` | `~/.cursor/skills/seedance-20/` |
| **Windsurf** | `.windsurf/skills/seedance-20/` | `~/.codeium/windsurf/skills/seedance-20/` |
| **OpenCode** | `.opencode/skills/seedance-20/` | `~/.config/opencode/skills/seedance-20/` |

---

## 🗂 Skill Directory

### Core Pipeline (auto-activated)

| Skill | Emoji | What it does |
|---|---|---|
| `seedance-prompt` | ✍️ | Build and validate prompts — 5-layer stack, @Tag system, quad-modal rules |
| `seedance-camera` | 🎥 | Camera movement, shot framing, multi-shot sequences, anti-drift locks |
| `seedance-motion` | 🏃 | Motion timing, action choreography, fight physics, video extension chains |
| `seedance-lighting` | 💡 | Lighting, atmosphere, light transitions, mood and time-of-day specs |
| `seedance-characters` | 🎭 | Character identity locking, @Tag assignment, multi-character scene management |
| `seedance-style` | 🎨 | Visual style, render-engine tokens, period aesthetics, style-transfer reference |
| `seedance-vfx` | ✨ | VFX physics contracts, particle systems, destruction, energy effects |
| `seedance-audio` | 🔊 | Native audio design, dialogue lip-sync, @Audio1 reference, desync fixes |
| `seedance-pipeline` | 🔗 | ComfyUI nodes, API integration, Firebase Studio, post-processing chains |
| `seedance-recipes` | 📖 | Genre template recipes: product ads, fight scenes, music videos, and more |
| `seedance-troubleshoot` | 🔧 | QA checklist, generation failure diagnostics, emergency fix procedures |

### Content Quality

| Skill | Emoji | What it does |
|---|---|---|
| `seedance-copyright` | ⚖️ | IP rules, safe substitutions, Feb 2026 enforcement data |
| `seedance-antislop` | 🚫 | Detects and removes AI filler language and hollow superlatives from prompts |

### Multilingual Vocabulary

| Skill | Emoji | Languages |
|---|---|---|
| `seedance-vocab-zh` | 🇨🇳 | 320+ Chinese cinematic terms (15 categories) |
| `seedance-vocab-ja` | 🇯🇵 | 280+ Japanese cinematic terms (14 categories) |
| `seedance-vocab-ko` | 🇰🇷 | 270+ Korean cinematic terms (13 categories) |
| `seedance-vocab-es` | 🇪🇸 | 270+ Spanish cinematic terms (Castilian + Latin American, 13 categories) |
| `seedance-vocab-ru` | 🇷🇺 | 270+ Russian cinematic terms (Eisenstein/Tarkovsky tradition, 13 categories) |

### Production Workflow

| Skill | Emoji | What it does |
|---|---|---|
| `seedance-interview` | 📋 | Guided pre-production interview → structured Seedance prompt |

---

## 🗄 Repository Structure

```
seedance-2.0/
├── SKILL.md                    ← Root skill (entry point)
├── LICENSE                     ← MIT
├── README.md                   ← This file
├── CHANGELOG.md                ← Version history
├── .github/
│   └── CODEOWNERS              ← @iamemily2050 owns all files
├── skills/
│   ├── seedance-audio/SKILL.md
│   ├── seedance-camera/SKILL.md
│   ├── seedance-characters/SKILL.md
│   ├── seedance-antislop/SKILL.md
│   ├── seedance-copyright/SKILL.md
│   ├── seedance-interview/SKILL.md
│   ├── seedance-lighting/SKILL.md
│   ├── seedance-motion/SKILL.md
│   ├── seedance-pipeline/SKILL.md
│   ├── seedance-prompt/SKILL.md
│   ├── seedance-recipes/SKILL.md
│   ├── seedance-style/SKILL.md
│   ├── seedance-troubleshoot/SKILL.md
│   ├── seedance-vfx/SKILL.md
│   ├── seedance-vocab-es/SKILL.md
│   ├── seedance-vocab-ja/SKILL.md
│   ├── seedance-vocab-ko/SKILL.md
│   ├── seedance-vocab-ru/SKILL.md
│   └── seedance-vocab-zh/SKILL.md
└── references/
    ├── json-schema.md
    ├── platform-constraints.md
    ├── prompt-examples.md
    └── quick-ref.md
```

---

## ✅ Platform Compatibility

All 20 skills pass the [AgentSkills open standard](https://agentskills.io/) validation:

- ✅ `name` — lowercase, hyphen-separated, no dots or spaces
- ✅ `description` — single-quoted, verb-first, includes WHEN trigger phrases
- ✅ `license: MIT`
- ✅ `user-invocable: true` and `user-invokable: true` on all 20 skills
- ✅ `tags:` array on all 20 skills
- ✅ `metadata` with `version`, `updated`, `author`, platform blocks
- ✅ `metadata.parent: seedance-20` on all 19 sub-skills
- ✅ No illegal top-level custom fields

---

## 📄 License

MIT © 2026 [Emily (@iamemily2050)](https://github.com/Emily2040)

---

## 🤝 Contributing

Pull requests welcome. Please run the front-matter validator before submitting:

```bash
# validate all SKILL.md files
python3 scripts/validate_frontmatter.py
```

---

*Built with ❤️ by Emily (@iamemily2050) — AI artist, filmmaker, and agent skill architect.*  
*Source intelligence: ByteDance Seedance 2.0 official blog, Douyin creator community, CSDN practitioner tutorials, Q1 2026.*
