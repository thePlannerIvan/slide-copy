# Slide Copy

[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-blue.svg)](LICENSE)

**专治 AI 写 PPT 像写长文章、满屏大词却看不出结论——用咨询顾问 + 资深广告策略师的双重文案纪律，让每页 3 秒抓重点、标题连成逻辑链。**

> 作者：阿祖不看 TVC（小红书同名）· [demyth.info](https://demyth.info) · [Lawyif@163.com](mailto:Lawyif@163.com)

---

## 一句话看懂：它帮你治好什么通病

让普通对话直接写 PPT 文案，十次有九次会出现：标题全是“现状分析 / 优化建议”这种无效标签、页面塞满提词器一样的完整段落、图片跟标题同义反复、以及满屏“赋能 / 闭环 / 抓手”的空洞大词。

**Slide Copy** 是一套轻量但极苛刻的**商业幻灯片原生文案规范**：

1. **影子甲板测试（3 秒扫读）**：把全套每页主标题抽出来连着读，必须就是一条完整的论证多米诺骨牌；
2. **屏幕字与演讲稿解耦**：屏幕上只放定性断言、数字证据和物理对照，把展开讲述留给 Speaker Notes；
3. **两种场合分开写法**：
   - **观念范式（比稿 / 品牌策略 / 创意战役）**：允许画面与标题对撞制造“第三层策略顿悟”，用朗诵意群断句写高潮页，禁用图文同义复述（画一辆车、写“这是一辆车”）；
   - **决策范式（咨询汇报 / 经营复盘）**：主标题直接做支配全页的 Action Title，严格过 `Fact → Insight → Implication` 闭环，拒绝数据裸奔。

---

## 改写前后一眼看懂（动词直接承担因果 + 拒绝生活流水账）

`Slide Copy` 对句子硬度有明确标尺——要求用真实行动主体做主语，让**动词本身推动因果**，不靠“由此 / 从而 / 具备……能力”硬凑逻辑，也不掉进粗糙的生活口语：

| 常见病句写法 | 经 Slide Copy 校准后的策略师成句 | 改在哪里 |
| --- | --- | --- |
| “因为盲目跨到了不熟悉的领域，由此导致了研发能力跟不上，进而影响了现金流” | **“脱离原生场景的盲目跨品类扩张导致专业研发断层，高库存与资金链承压拖垮了主业。”** | 删掉连接装置，由实词和动词直接咬合因果 |
| “店里自己备货、能当场响应需求，产品也都是滑手自己动手改出来的” | **“交付前置到零售终端，核心鞋型全部诞生于滑手的真实自发改装。”** | 从车间生活语域升级到策略师专业语域 |

---

## 什么时候选我 vs 选别的 Skill

| 你的当下任务 | 用哪个 Skill | 分工说明 |
| --- | --- | --- |
| 要打磨整套 PPT 标题链、精炼单页卡片文字、清理废话与空洞大词 | **本 Skill (`slide-copy`)** | 只负责幻灯片原生架构与句子标准 |
| 想把一段枯燥平铺的背景介绍或案例故事改得有悬念、有推进拉扯感 | [`storytelling`](https://github.com/thePlannerIvan/storytelling) | `storytelling` 管宏观认知张力；单页怎么下标题、怎么删废话以我为准 |
| 需要连带读懂整 folder 资料、配图、核查数字、直接产出可交接的内容包 | [`planners-bypage`](https://github.com/thePlannerIvan/planners-bypage) | `bypage` 会自动调用我来写文案并跑完后续流水线 |
| 要画精美视觉排版、套品牌模板、导出 `.pptx` | [`planners-ppt-hell`](https://github.com/thePlannerIvan/planners-ppt-hell) | 我不动视觉框线与导出，只管文字和页面角色分工 |

---

## 快速开始与安装

### 1. 安装

**DSH 用户**：无需单独勾选——通过 [Planners Form](https://github.com/thePlannerIvan/planners-form) 安装 `planners-proposal`、`planners-bypage` 或 `planners-ppt-hell` 时会一并安装，安装后也可单独呼叫 `slide-copy`。

**Codex / Claude Code 用户：**

```bash
npx skills add https://github.com/thePlannerIvan/slide-copy --skill slide-copy
```

或克隆到本地 Skill 目录：

```bash
git clone https://github.com/thePlannerIvan/slide-copy.git ~/.codex/skills/slide-copy
# 或
git clone https://github.com/thePlannerIvan/slide-copy.git ~/.claude/skills/slide-copy
```

*(纯规范型 Skill：**零运行脚本与第三方依赖**，任何对话环境装上即用。)*

### 2. 直接这样调用

```text
用 $slide-copy 帮我重构这份 15 页比稿 Deck 的文案：
先抽取所有页面主标题过一遍影子甲板链条，再把正文里的“从而/因此/赋能”和提词器长句重写成 3 秒扫读版。
```

---

## 目录、协议与商业合作

- **目录构成**：`SKILL.md`（媒介物理、影子甲板、双范式与句子引擎完整规范）、`agents/openai.yaml`（界面元数据）。
- **许可与归属**：以 [AGPL-3.0-only](LICENSE) 发布；作者来源保留于 [NOTICE](NOTICE)，默认不写入客户最终 PPT；商标与 fork 规范见 [TRADEMARK.md](TRADEMARK.md)。
- **商业合作**：企业提案文案规范内训、团队写稿标准定制或闭源授权，请联系 `Lawyif@163.com` 或访问 [demyth.info](https://demyth.info)，详见 [COMMERCIAL.md](COMMERCIAL.md)。
