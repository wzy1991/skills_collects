# skills_collects

一个用于收集、整理和复用 AI Skills 的仓库。

这个仓库适合存放各种可复用的 AI 工作流，例如：学习规划、写作辅助、代码审查、行业研究、产品需求分析、数据分析等。

## 目录结构

```text
skills_collects/
├── README.md
├── LICENSE
├── skills/
│   └── learning-navigator/
│       ├── SKILL.md
│       ├── README.md
│       ├── examples/
│       └── prompts/
└── templates/
    └── SKILL_TEMPLATE.md
```

## 已收录 Skills

| Skill | 中文名 | 作用 | 状态 |
|---|---|---|---|
| [`learning-navigator`](./skills/learning-navigator/) | 学习导航员 | 为任何行业、课程或技能生成结构化学习路线 | v1.0 |

## 如何使用

### 方式一：复制到 ChatGPT / 自定义 GPT

打开对应 Skill 的 `SKILL.md`，复制其中的说明内容，粘贴到自定义 GPT 的 Instructions 中。

### 方式二：复制到 Agent Skills 目录

将某个 Skill 文件夹复制到你的 Agent Skills 目录中，例如：

```bash
cp -r skills/learning-navigator ~/.your-agent/skills/
```

### 方式三：作为提示词模板使用

也可以直接复制 `README.md`、`SKILL.md` 或 `prompts/` 中的内容，在 ChatGPT、Claude、Gemini、Kimi、通义千问等模型中使用。

## 新增 Skill 规范

建议每个 Skill 使用如下结构：

```text
skills/your-skill-name/
├── SKILL.md
├── README.md
├── examples/
└── prompts/
```

命名建议：

- 使用英文小写
- 单词之间用短横线 `-`
- 名称尽量短，例如 `writing-coach`、`code-reviewer`、`industry-researcher`

## 质量要求

一个好的 Skill 应该满足：

1. 触发场景明确：什么时候应该使用它。
2. 输出格式稳定：每次生成结构一致。
3. 任务边界清楚：知道该做什么，也知道不该做什么。
4. 可操作性强：避免空话，给出具体步骤、模板和示例。
5. 可复用：换一个主题、行业或项目也能稳定工作。

## License

MIT License
