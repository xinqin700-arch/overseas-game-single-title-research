# 海外游戏单品深度调研（overseas-game-single-title-research）

一个 WorkBuddy Skill：对单一海外游戏/App 做深度买量与用户调研，自动产出**单一完整、可嵌入网页的 HTML 报告**。由一份实测定稿的提示词固化而成，含 10 个板块、5 类真实数据图表、12 维动机 / 8 类人格画像，以及四段式投放建议。

## 能力

- 产品基本情况、榜单排名、投放趋势与媒体结构
- 用户评论（分层抽样 + 双语引用）、用户画像 / 动机 / 人格
- 深度报道（微信搜一搜）、竞品分析、投放大盘对标、投放建议
- 全程强调真实取数：估算值标注、禁止编造评论/阅读量/排名/素材数、取不到就降级说明

## 安装

方式一：下载 `overseas-game-single-title-research.zip`，在 WorkBuddy 的技能管理中选择"导入/安装 zip"。

方式二：把本目录整体放到技能目录后重启 WorkBuddy：

- 用户级：`~/.workbuddy/skills/overseas-game-single-title-research/`
- 项目级：`<项目>/.workbuddy/skills/overseas-game-single-title-research/`

也可直接安装到 SkillHub：在 WorkBuddy 技能市场搜索"海外游戏单品深度调研"。

## 使用（自行替换产品名称）

直接对 WorkBuddy 说：

> 用「海外游戏单品深度调研」skill，帮我调研 `<产品名>`，包名是 `<com.xxx.xxx>`，生成 HTML 报告。

需要替换的 4 个参数：

| 参数 | 说明 | 缺省 |
| --- | --- | --- |
| 产品名 | 中文名/英文名 | 必填 |
| 包名 | Google Play 包名，用于锁定身份 | 尝试自动锁定，否则按名检索并注明 |
| 观察窗口 | 起止日期 | 最近 60 个完整自然日 |
| 公众号名单 | 深度报道优先公众号 | 用内置默认名单 |

参数会由 Skill 自动替换进 `references/full-prompt.md` 的对应占位符，无需手动改文件。

## 依赖

- **橙果数航 / DataVoyage MCP**（买量、榜单、竞品、大盘数据）——需在 WorkBuddy 中启用该连接器。
- Google Play / App Store 公开页面与微信搜一搜（走 WorkBuddy 联网能力）。

## 目录结构

```
overseas-game-single-title-research/
├── SKILL.md                                   # 触发条件、参数收集、工作流、红线
└── references/
    ├── full-prompt.md                         # 提示词正文（一至十五节，执行准则）
    ├── appendix-a-personality-weights.md      # 8 类人格 × 12 维动机权重
    ├── appendix-b-motivation-anchors.md       # 12 项动机判定锚点
    └── params-quickref.md                     # 可调参数速查
```

## License

MIT
