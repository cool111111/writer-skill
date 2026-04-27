# Writer Skill

一套为 AI Agent 设计的公众号长文写作方法论，从选题到成稿的全流程规范。

基于 Claude Code 的 Skill 机制构建，可直接加载到支持 Skill 的 AI Agent 中使用。

## 核心特点

- **HKR 选题质检**：Happy + Knowledge + Resonance 三维度评估选题质量
- **口语化写作**：像聊天一样写文章，拒绝"说白了""本质上"等 AI 味表达
- **严格事实核查**：所有可验证事实必须有来源，人物引用必须可追溯
- **禁用词体系**：自动规避书面套话和营销号用语
- **结构化质检**：L1 硬性规则 + L2 风格审查 + L3 深度打磨三级质检

## 文件结构

```
writer-skill/
├── SKILL.md                          # 主 Skill 文件（Agent 加载入口）
└── references/
    ├── content_methodology.md        # 内容方法论参考
    └── style_examples.md             # 风格示例库
```

## 使用方式

放到 AI Agent 的 skills 目录下即可自动加载。

```
your-agent/skills/writer/
├── SKILL.md
└── references/
    ├── content_methodology.md
    └── style_examples.md
```

## License

MIT
