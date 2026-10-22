# Codex Skills

个人可复用的 Codex 技能集合，持续收录写作、研究与工作流中的实用方法。

每个技能独立存放，包含使用场景、执行方法，以及需要的范例或辅助资源。

## 技能目录

| 技能 | 用途 | 入口 |
| --- | --- | --- |
| `write-tech-satire` · 科技讽刺寓言 | 默认写一个简短冷幽默段子；用“火鸡逻辑”讽刺把过去幸存当成未来保证，让结尾重新解释前面的安全感。 | [技能说明](skills/write-tech-satire/SKILL.md) · [写作范例](skills/write-tech-satire/references/examples.md) · [火鸡逻辑](skills/write-tech-satire/references/turkey-logic.md) |

## 安装与使用

可以直接在 Codex 中提出：

> 从 https://github.com/0xAPTX/codex-skills 安装 skills/write-tech-satire 技能。

也可以下载仓库，将所需技能的整个目录放入个人技能目录 `$CODEX_HOME/skills/`；未设置 `CODEX_HOME` 时，默认是 `~/.codex/skills/`。保留 `SKILL.md` 和所有子目录，若同名技能已存在，先比较内容再更新。

安装并加载后，可以明确调用：

```text
用 $write-tech-satire 调侃一下公司推行 AI 降本增效，辛辣一点。
```

```text
用 $write-tech-satire 把这个新闻写成一段“火鸡农场”那种冷幽默寓言。
```

涉及近期新闻时，技能会要求核实背景，并区分事实与虚构情节。

## 仓库结构

```text
skills/
└── write-tech-satire/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    └── references/
        ├── examples.md
        └── turkey-logic.md
```

## 添加新技能

1. 在 `skills/<skill-name>/` 下创建独立目录，目录名使用小写字母、数字和连字符。
2. 在 `SKILL.md` 的 YAML 头部填写 `name` 和 `description`，正文说明适用场景与方法。
3. 按实际需要添加 `references/`、`scripts/`、`assets/` 或 `agents/openai.yaml`。
4. 更新本页技能目录，检查相对链接，并在发布前确认文件不含密钥、个人路径或未授权的私人资料。

当前提供的内容以中文为主。每个技能的适用范围以其 `SKILL.md` 为准。
