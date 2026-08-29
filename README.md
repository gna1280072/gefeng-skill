# 割风 · ge-feng

> 一个把"情感越大，句子越平"写到极致的 AI 写作技能。
> A cold, restrained narrative writing skill for AI agents — born from the viral Chinese story 《我的女友景甜》.

**割风**是一套冷峻克制叙事文风：用记账式的精确、物流式的冷静，去写最昂贵的情感和最昂贵的失败。核心张力来自"巨额的财富"与"什么都没发生"之间的落差。

SKILL.md 遵循开放标准 [Agent Skills Specification](https://agentskills.io/specification)，主流 AI 工具可直接加载使用。

## 风格铁律（五条）

1. **句号统治**：段落 1-3 句，绝不写长句和排比。
2. **数字代替形容词**：不说"很贵""很久"，只说"一百五十块（犹豫了三天）"。数字即情绪。
3. **情绪零度**：再大的事也用报物流的口吻写。禁止直接抒情。
4. **以"无"为引擎**：戏都在"没发生的事"上——空着的楼层、买光的座位。结尾常落在"什么都没有发生"。
5. **物件即关系**：靠 2-3 个反复出现的具体物件承载感情，首尾呼应。

## 十大技法

精确记账 · 大小对照 · 情绪留白 · 极简对话 · 单发比喻 · 省略胜于言说 · 物件复现 · 时间折叠 · 事实锚点 · 以"无"收束

每条技法的定义、规则与原文例证见 `SKILL.md` 与 `references/style-analysis.md`。

## 安装

SKILL.md 是开放标准格式（YAML frontmatter + Markdown 指令），以下工具支持直接安装：

| 工具 | 存放位置 |
|---|---|
| WorkBuddy | `~/.workbuddy/skills/` |
| Claude Code | `~/.claude/skills/` |
| OpenAI Codex CLI | `~/.codex/skills/` |
| Gemini CLI | `~/.gemini/skills/` |
| OpenCode | `~/.config/opencode/skills/` |

安装方式：把本仓库（或仅 `SKILL.md` + `references/`）复制到上表对应目录。

> Cursor / Windsurf / GitHub Copilot 使用各自规则格式（`.mdc` / `.windsurfrules` / `copilot-instructions.md`），可将 SKILL.md 正文转换为对应格式，或用社区工具（如 `agent-skill-creator`）自动转换。

## 使用

对 AI 说：

- "用割风文风写一篇……"
- "用冷叙事 / 克制白描的风格写……"
- "以不煽情的方式写深情"

技能会按 8 步工作流执行：定内核 → 找物件 → 建对照 → 列数字 → 排时间 → 写初稿 → 删 → 验，最后按输出检查清单自检。

## 示例文章

| 文件 | 形态 |
|---|---|
| `examples/保护区.md` | 科幻短篇 · 极简形态（末日 AI 病毒 × 保护区爱情，约 1200 字） |
| `examples/绿萝.md` | 都市爱情 · 长篇形态（合租 × 日久生情 × 隐情，约 5000 字，展示对话与细节） |

## 目录结构

```
gefeng-skill/
├── SKILL.md                    # 技能本体（必需）
├── references/
│   └── style-analysis.md       # 《我的女友景甜》逐技法拆解（含原文引用）
└── examples/
    ├── 保护区.md               # 示例：科幻短篇
    └── 绿萝.md                 # 示例：都市爱情 5000 字
```

## 适用边界

- 强依赖"求而不得"的情感内核，写圆满结局会不成立。
- 数字必须前后自洽，读者会当纪实核对。
- 涉及真实公众人物/机构时，虚构与影射的边界由使用者自行把关；本技能只提炼文体技法，不鼓励针对真实人物的恶意影射。

## License

MIT
