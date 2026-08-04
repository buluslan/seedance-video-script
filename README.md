<div align="center">

<!-- <img src="assets/banner.png" alt="Seedance Video Script" width="100%"> -->

# 🎬 Seedance Video Script

**把商业意图 + 素材,转成 Seedance 2.5 可直接使用的视频分镜提示词**

**想了解更多最新AI行业动态,AI+电商/广告的行业实践方法,人与AI如何协作共生的思考,请关注公众号:【新西楼】**

![qrcode_for_gh_e3b954bd3859_258](https://github.com/user-attachments/assets/d8f068d9-c4f8-46c7-914c-fbcab5d52f2a)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-SKILL-blueviolet.svg)](https://docs.anthropic.com/en/docs/claude-code)
[![Version](https://img.shields.io/badge/version-0.2.0-black.svg)]()

**时间戳分镜 · @引用语法 · 白模参考 · 绿幕/区域/运镜编辑 · 原生音频 · SPACE 框架 · 零依赖**

**Created By Buluu@新西楼**

</div>

## 项目简介

一个 **Claude Code / Agent 原生**的 Skill:输入商业意图 + 素材,输出可直接粘到**即梦 Dreamina / 火山方舟 Ark**的 Seedance 2.5 完整分镜 prompt + 素材上传顺序。

- **Agent 原生**:装到 Claude Code 即用,Agent 按 5 步流程帮你生成 prompt
- **平台兼容**:产出适配即梦(C 端)和火山方舟(B 端 API)两个平台
- **零依赖**:不调 API、不生成视频本身,纯知识底座 + prompt 生成

## ✨ 它做什么

把"我想做个 XX 视频"转成 Seedance 2.5 能精准执行的 prompt:

| 能力 | 说明 |
|---|---|
| 时间戳分镜 | `0-5秒:...;6-10秒:...`,2.5 核心语法 |
| @引用分配 | 为每个素材标用途(人物/场景/运镜/音色/产品) |
| 白模参考 | `@白模N` 锁空间结构/运镜/轨迹 |
| 编辑能力 | 绿幕 / 区域 / 运镜 / 时间戳编辑 |
| 原生音频 | 台词`{}`音效`<>`音乐`()`字幕`【】`+ 纯音频驱动 + 多语言 |
| SPACE 框架 | 快速版分镜公式 |
| 避坑自检 | ID 漂移/字幕乱入/风格漂移等 + 解法 |

**5 步生成流程**:摸意图 → 盘素材分配@引用 → 时间戳分镜 → 音频+约束 → 避坑自检

## 🚫 它不做什么

- ❌ 不调 Seedance API(纯产出 prompt,你自行上传到即梦/方舟生成)
- ❌ 不生成视频本身(输出是文字 prompt,不是视频文件)
- ❌ 不处理素材文件(素材由你上传到平台,skill 只给 @编号 + 顺序)

## 🚀 快速开始

**安装**(放进 Claude Code skills 路径):
```bash
# 个人级(所有项目可用)
git clone https://github.com/buluslan/seedance-video-script.git ~/.claude/skills/seedance-video-script
```

**最小输入示例**:
```
给 TikTok 做个自动猫砂盆的带货视频,30 秒,我有产品图和猫咪图。
```
Agent 会反问补全(场景/平台/比例/素材),或你照 SKILL.md 的「输入契约」一次给全跳过反问。

## 🧠 知识底座

覆盖 Seedance 2.5 全部能力(详见 `references/`):30 秒时长 / 50 参考 / 时间戳分段 / 白模参考 / 绿幕·区域·运镜编辑 / 原生音频与纯音频驱动 / SPACE 框架。

## 📁 结构

```
seedance-video-script/
├── SKILL.md              # 心脏:路由 + 5 步生成流程 + 输入契约
├── references/
│   ├── prompt-formula.md       # 8 要素公式 + SPACE + 画质风格
│   ├── shot-timing.md          # 时间戳分段 + 场景弧线
│   ├── reference-syntax.md     # @引用 14 用途 + 4 功能角色 + 白模
│   ├── audio-design.md         # 音频符号 + 纯音频驱动 + 多语言
│   ├── tasks-editing.md        # 三大任务 + 编辑新能力
│   ├── camera-language.md      # 运镜 + 景别术语
│   └── pitfalls.md             # 能力边界避坑 + 反模式
└── assets/
    └── scenarios.md            # 8 商业场景模版库
```

## 📜 License

[MIT](LICENSE) · Copyright (c) 2026 Buluu@新西楼

<div align="center">

**如果这个工具帮到了你,欢迎 ⭐ Star 支持。更多 AI × 跨境电商实操内容,关注公众号「新西楼」。**

</div>
