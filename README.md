# 从知识点到串线物故事

给一组课本知识点，得到三个适合短视频的中文故事雏形。每个故事围绕一个串线物展开，知识规律参与情节，高潮落在感动、悲伤或燃上。

## 安装

可以直接把这句话发给能访问 GitHub、支持安装技能的 agent。

> 请从 https://github.com/1d-a/knowledge-to-story 安装 `skills/knowledge-to-story` 整个目录，并确认能读到 `references` 里的《串线物研究》和《样例》。

如果界面提供「上传技能」入口，直接上传这个 ZIP。包内顶层是 `knowledge-to-story/`，中文文件名使用 UTF-8。[下载技能安装包](https://github.com/1d-a/knowledge-to-story/raw/refs/heads/main/dist/knowledge-to-story.zip)

| 使用环境 | 手动安装方法 |
| --- | --- |
| 本地 Codex | 将整个 `knowledge-to-story` 文件夹放入项目的 `.agents/skills/`，或个人目录 `~/.agents/skills/`。 |
| 本地 Claude Code | 将整个文件夹放入项目的 `.claude/skills/`，或个人目录 `~/.claude/skills/`。安装后可用 `/knowledge-to-story` 调用。 |
| 其他支持 Agent Skills 的工具 | 将整个文件夹放入该工具的技能目录，让 `SKILL.md` 直接位于 `knowledge-to-story/` 下。 |
| 只能上传文件的对话助手 | 同时附上下面三份 Markdown，告诉它先读三份，再按 `SKILL.md` 创作。这种用法在当前对话生效。 |

目录约定见 [Codex 文档](https://developers.openai.com/codex/skills/) 和 [Claude Code 文档](https://code.claude.com/docs/en/skills)。

## 技能内容

| 文件 | 用途 |
| --- | --- |
| [SKILL.md](skills/knowledge-to-story/SKILL.md) | 创作规则、工作流程、自检清单和交付格式。 |
| [串线物研究.md](skills/knowledge-to-story/references/串线物研究.md) | 用两把尺子判断串线物在情节里管多少事、身上有几层意思，并参考七种形态、八种走法和十个案例。 |
| [样例.md](skills/knowledge-to-story/references/样例.md) | 三个认可的故事和三个反例，供动笔前对照情绪高潮与科学规律。 |

两份参考资料都随包提供，文件路径相对于 `SKILL.md`。文字创作只需能读 Markdown。输入截图时需要识图能力，也可以改贴文字。离线时可从已确认的知识点构思虚构故事。涉及真实人物、真实事件或拿不准的科学事实时，需查证来源。

## 试用

> 用 knowledge-to-story，把初中物理「平面镜成像」写成适合短视频的故事雏形。

默认每组知识点生成三个故事。每个故事都写出落点、串线物、涉及的知识点，以及开头、蓄力、【高潮】、收尾和点睛。也可以在请求里指定数量、题材或情绪落点。
