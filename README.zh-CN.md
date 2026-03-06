# Product Manager Skills 中文说明

**这不是模板包，而是一个给 AI 编码工具安装的 PM 大脑。**

它会把 Claude Code、Codex、Cursor、Windsurf 这类工具，变成一个能写 PRD、诊断 SaaS 指标、做路线图取舍、做用户研究框架化思考、以及辅导 PM 晋升的产品经理搭档。

## 它为什么更容易被反复使用

多数 AI 工具能把话说顺，但很难把 PM 判断做对。这个项目更适合这些高频场景：

- 把模糊需求推进成有问题定义、有指标、有边界的 PRD
- 根据 MRR、churn、CAC、LTV 直接做业务健康诊断
- 在路线图和优先级讨论中指出 tradeoff，而不是只会“建议平衡”
- 帮高级 PM 准备 Director / VP 级别的面试和能力迁移

## 60 秒安装

### Claude Code / OpenClaw

```bash
clawhub install product-manager-skills
```

### Codex / Cursor / Windsurf

```bash
npx skills add Digidai/product-manager-skills
```

安装后可以直接粘贴这些 prompt：

```text
帮我写一个通知偏好功能的 PRD。缺失信息请合理假设，并明确标注。

分析这些指标：MRR 5 万美元，500 个客户，毛利率 80%，月流失 8%，CAC 500 美元。

帮我评审这个 roadmap，指出哪些地方是利益相关方在推，而不是证据在推。
```

更多可直接复用的提示词见：[STARTER-PROMPTS.md](STARTER-PROMPTS.md)

## 三个最值得先试的场景

| 场景 | 你会得到什么 | 示例 |
|---|---|---|
| **SaaS 业务诊断** | 它会算公式、给 benchmark、指出根因，不是泛泛建议 | [examples/saas-health-diagnostic.md](examples/saas-health-diagnostic.md) |
| **PRD 评审与挑错** | 它会指出 Solution Smuggling、指标缺失、范围过大、交付风险 | [examples/prd-review.md](examples/prd-review.md) |
| **晋升 / 面试辅导** | 它会判断你的“海拔”是否到 Director 级别，并给补齐方案 | [examples/director-coaching.md](examples/director-coaching.md) |

## 这个项目包含什么

- 6 个知识域：发现研究、战略定位、交付执行、财务指标、职业发展、AI 产品
- 12 个模板：PRD、User Story、Problem Statement、Roadmap、Competitive Analysis 等
- 30+ 个框架：JTBD、Geoffrey Moore、PRFAQ、OST、RICE、Kano 等
- 32 个 SaaS 指标：带公式、阶段基准值、红旗等级
- 一套统一质量门槛：要求标注假设、量化结果、说明取舍、识别反模式

## 它和通用 AI 的区别

| 通用 AI | Product Manager Skills |
|---|---|
| 会把需求写得像样 | 会先判断问题定义是不是错了 |
| 会说“优化用户体验降低流失” | 会算出 8% 月流失约等于 63% 年流失，并判断是否应该先停投放 |
| 会接受模糊目标 | 会要求 baseline、target、timeframe |
| 容易顺着你说 | 会主动推回来，指出坏 framing 和错误取舍 |

## 适合谁

- 已经在 AI 编码工具里工作的技术型 PM、Founder、产品负责人
- 想把 PM 认知嵌到本地工作流里，而不是再买一个 SaaS 工具的人
- 需要“会挑战你”的 AI，而不是只会把格式写完整的人

## 不适合谁

- 更想要带审批、协作、评论、共享的网页产品的团队
- 只想套模板，不希望 AI 指出 framing 问题的人
- 不愿意使用本地安装或 repo 型知识包的人

## 信任与安全

这是一个纯 Markdown 项目：

- 没有脚本
- 没有网络调用
- 不需要密钥
- 没有提权
- 所有内容都可审查

## 相关文件

- 英文主 README：[README.md](README.md)
- 快速提示词：[STARTER-PROMPTS.md](STARTER-PROMPTS.md)
- 技能入口：[SKILL.md](SKILL.md)

[CC BY-NC-SA 4.0](LICENSE)
