# Slide Copy

商业幻灯片的结构、标题链与页面文案规范。

[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-blue.svg)](LICENSE)

作者：阿祖不看 TVC · 小红书同名账号 · [demyth.info](https://demyth.info) · Lawyif@163.com

## 使用方式

调用名：`slide-copy`。提案、战略方案、咨询报告、路演和高层汇报的内容编写或校订。不负责 PPT 排版渲染、图像生成或事实取证。

先明确整案的叙事链和页面角色，再组织每页主张、证据与正文，区分屏幕内容与口播备注，并检查影子甲板的连贯性。

```text
用 slide-copy 检查这份逐页稿：先看标题链，再改每页的主张和证据表达。
```

## 安装

```bash
npx skills add https://github.com/thePlannerIvan/slide-copy --skill slide-copy
```

也可以克隆到支持 Skill 的 Agent 目录（以下为 Claude Code）：

```bash
git clone https://github.com/thePlannerIvan/slide-copy.git ~/.claude/skills/slide-copy
```

在 DSH 中，Planners Form 会随调用本组件的配套 Skill 安装它；安装后仍可通过 `slide-copy` 独立调用。它没有独立审阅页，不在 Planners Form 设置中单列。

没有额外脚本运行时或审阅页依赖。

## 目录

`SKILL.md`：甲板治理与页面文案规范；`agents/openai.yaml`：界面元数据。

## 开源与归属

许可文本见 [LICENSE](LICENSE)（AGPL-3.0）。作者和来源见 [NOTICE](NOTICE)，名称使用边界见 [TRADEMARK.md](TRADEMARK.md)，合作入口见 [COMMERCIAL.md](COMMERCIAL.md)。署名用于仓库和工作过程，默认不加入最终客户交付物。
