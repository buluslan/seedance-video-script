[简体中文](README.md) | English

<div align="center">

<!-- <img src="assets/banner.png" alt="Seedance Video Script" width="100%"> -->

# 🎬 Seedance Video Script

**Turn business intent + assets into ready-to-use Seedance 2.5 video storyboard prompts**

**Want the latest AI industry trends, AI × e-commerce/advertising practices, and thoughts on human-AI collaboration? Follow the WeChat Official Account: 【新西楼.AI】**

![qrcode_for_gh_e3b954bd3859_258](https://github.com/user-attachments/assets/d8f068d9-c4f8-46c7-914c-fbcab5d52f2a)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-SKILL-blueviolet.svg)](https://docs.anthropic.com/en/docs/claude-code)
[![Version](https://img.shields.io/badge/version-0.2.0-black.svg)]()

**Timestamped storyboards · @reference syntax · White-model refs · Green-screen/region/camera editing · Native audio · SPACE framework · Zero dependencies**

**Created By Buluu@新西楼.AI**

</div>

## Overview

An **agent-native** Skill: feed it business intent + assets, and it outputs a complete Seedance 2.5 storyboard prompt — ready to paste into **Dreamina / Volcengine Ark** — plus the asset upload order.

- **Agent-native**: works with any agent (Codex / Claude Code / Cursor, etc.) — install it and generate prompts via the 5-step flow
- **Platform-compatible**: outputs fit both Dreamina (C-end) and Volcengine Ark (B-end API)
- **Zero dependencies**: no API calls, doesn't render the video itself — a pure knowledge base + prompt generator

## ✨ What it does

Turns "I want a video about X" into a prompt Seedance 2.5 can execute precisely:

| Capability | Description |
|---|---|
| Timestamped storyboards | `0-5s: ...; 6-10s: ...` — the core 2.5 syntax |
| @reference assignment | Tag each asset's role (character / scene / camera / voice / product) |
| White-model refs | `@白模N` locks spatial structure / camera / trajectory |
| Editing | Green-screen / region / camera / timestamp editing |
| Native audio | Dialogue `{}`, SFX `<>`, music `()`, subtitles `【】` + audio-driven pacing + multilingual |
| SPACE framework | A compact storyboard formula |
| Pitfall self-check | ID drift / rogue subtitles / style drift — with fixes |

**5-step flow**: clarify intent → assign @references → timestamped storyboard → audio + constraints → pitfall self-check

## 🚫 What it doesn't do

- ❌ No Seedance API calls (pure prompt output — you upload to Dreamina/Ark yourself)
- ❌ Doesn't generate the video itself (output is a text prompt, not a video file)
- ❌ Doesn't handle asset files (you upload assets to the platform; the skill only gives @IDs + order)

## 🚀 Quick Start

**Install** (drop into your agent's skills path):
```bash
# User-level (available across all projects)
git clone https://github.com/buluslan/seedance-video-script.git ~/.claude/skills/seedance-video-script
```

**Minimal input example**:
```
Make a 30s TikTok shoppable video for an automatic litter box. I have product photos and a cat photo.
```
The agent will ask follow-ups (scene / platform / ratio / assets) — or fill the "Input Contract" in SKILL.md once to skip the back-and-forth.

## 🧠 Knowledge Base

Covers all Seedance 2.5 capabilities (see `references/`): 30s duration / 50 references / timestamped segments / white-model refs / green-screen·region·camera editing / native audio & audio-driven / SPACE framework.

## 📁 Structure

```
seedance-video-script/
├── SKILL.md              # Heart: routing + 5-step flow + input contract
├── references/
│   ├── prompt-formula.md       # 8-element formula + SPACE + quality/style
│   ├── shot-timing.md          # Timestamped segments + scene arcs
│   ├── reference-syntax.md     # @reference 14 uses + 4 roles + white-model
│   ├── audio-design.md         # Audio symbols + audio-driven + multilingual
│   ├── tasks-editing.md        # Three tasks + new editing powers
│   ├── camera-language.md      # Camera movement + shot size terms
│   └── pitfalls.md             # Capability edges + anti-patterns
└── assets/
    └── scenarios.md            # 8 business scenario templates
```

## 📜 License

[MIT](LICENSE) · Copyright (c) 2026 Buluu@新西楼.AI

<div align="center">

**If this tool helped you, a ⭐ Star is appreciated. For more AI × cross-border e-commerce practices, follow the WeChat Official Account 「新西楼.AI」.**

</div>
