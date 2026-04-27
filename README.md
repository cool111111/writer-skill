<div align="center">

# ✍️ Writer Skill

**让 AI Agent 写出有人味的公众号长文**

一套从选题到成稿的全流程写作方法论 Skill — 自带 HKR 选题质检、反 AI 味词库、三级质检流水线。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Skill: Claude Code](https://img.shields.io/badge/Skill-Claude%20Code-8A2BE2)](https://github.com/anthropics/claude-code)
[![Style: 中文](https://img.shields.io/badge/Style-中文长文-red)]()
[![Stars](https://img.shields.io/github/stars/cool111111/writer-skill?style=social)](https://github.com/cool111111/writer-skill/stargazers)

</div>

> 不是又一个"帮我写一篇关于 X 的公众号文章"的 prompt。
> 是一整套生产规范，让 AI 输出的稿子能直接发，不用人来"去 AI 味"。

<!-- TODO 在此处插入一张 demo 图（同一选题：裸 AI vs Writer Skill 输出对比，最有冲击力）-->
<!-- 拖图教程见 README 底部 -->

## 为什么需要这个 Skill

普通 AI 写公众号长文的三大病：

| 症状 | 表现 | Writer Skill 的解法 |
|------|------|-----|
| AI 味重 | 满屏"说白了""本质上""不仅...更..." | 内置 **禁用词库**，写完自动扫描重构 |
| 没观点 | 罗列信息、复读维基百科 | **HKR 选题质检** 强制要求观点密度 |
| 没人样 | 翻译腔、书面套话、假装客观 | **口语化重构规则**，像聊天一样把事讲透 |

## 核心特性

- 🎯 **HKR 选题质检** — Happy（情绪价值）+ Knowledge（信息密度）+ Resonance（共鸣度）三维度评分，不及格的选题直接拦下
- 🚫 **反 AI 味词库** — 60+ 高频 AI 套话黑名单，写完自动扫描替换
- 🔍 **强制事实核查** — 所有可验证事实必须挂来源，人物引用必须可追溯
- 📐 **三级质检流水线** — L1 硬规则 / L2 风格审查 / L3 深度打磨
- 📚 **方法论可读** — `references/` 目录下完整的内容方法论 + 风格示例库

## Quick Start

把整个目录扔到你 Agent 的 skills 目录下，就完事了：

```bash
git clone https://github.com/cool111111/writer-skill.git \
  ~/.your-agent/skills/writer
```

然后在对话里说："**帮我写一篇关于 XXX 的公众号文章**"，Agent 会自动加载这个 Skill 走完整流程。

## 文件结构

```
writer-skill/
├── SKILL.md                          # 主 Skill 入口（Agent 自动加载）
└── references/
    ├── content_methodology.md        # 内容方法论：选题 / 结构 / 节奏
    └── style_examples.md             # 风格示例库：标题 / 开头 / 收尾的好坏对比
```

## 适配的 Agent

理论上任何支持 [Claude Skills](https://github.com/anthropics/claude-code) 规范的 Agent 都能用，已验证：

- ✅ Claude Code
- ✅ Mavis（多 Agent 编排框架）
- ⚠️ 其他 Agent 需自行验证 SKILL.md 加载机制

## 配套 Skill

写长文用 Writer，写短图文用 [XHS Content Skill](https://github.com/cool111111/xhs-content-skill)，二者共享风格底座。

## License

MIT — 用就完事了。如果对你有帮助，**给个 star** ⭐ 是最大的鼓励。

