# 智书企飞 AI Skill

这是一个 AI Skill。安装后，AI 助手可以基于智书企飞的公司资料和产品资料，回答智书企飞、智书AI合同、烽火、智审平台相关问题，并辅助售前、客户成功和内部同学快速形成统一口径。

它更像一个“智书企飞产品顾问 + 客户成功陪伴助手”。

## 关于智书企飞

智书企飞是飞书官方认证服务伙伴，围绕数字化、云计算和 AI，为企业提供“技术 + 咨询 + 服务”一体化的智能运营解决方案。

| 项目 | 内容 |
|---|---|
| 公司定位 | 数字时代的企业智慧引擎 |
| 核心方向 | 飞书生态运营、业务系统建设、AI 合同管理 |
| 核心产品 | 智书AI合同、烽火、智审平台 |
| 服务方式 | 技术 + 咨询 + 服务 |

## 这个 Skill 能做什么

| 能力 | 你可以问 | 来源 |
|---|---|---|
| 公司介绍 | “智书企飞是什么？”“怎么向客户介绍智书企飞？” | references/company.md |
| 产品介绍 | “智书企飞有哪些产品？”“智书合同是做什么的？” | references/products.md |
| 场景判断 | “合同审查适合哪个产品？”“这个客户适合烽火吗？” | references/products.md |
| FAQ | “能不能私有化？”“有试用吗？”“智书合同和智审平台有什么区别？” | references/faq.md |
| 售前话术 | “这个场景怎么讲更容易让客户懂？” | references/sales-playbook.md |
| 竞品口径 | “和 e签宝 / 法大大 / 契约锁怎么比？” | references/competitors.md |

## 核心产品

### 智书AI合同

长在飞书上的 AI 合同应用 / 法律 Agent，面向企业合同全生命周期管理，覆盖起草、协商、审查、审批、比对、归档、履约和数据分析。

### 烽火

基于飞书生态的业务系统解决方案，主打“协同 + 业务 ALL-IN-ONE”，适合把项目、销售、订单、运营、费用等业务流程结构化管理起来。

### 智审平台

智能 AI 合同审查助手，帮助业务、法务和合规团队快速识别合同风险并生成修改建议。

## 目录结构

```text
zhishu-qifei-skill/
├── SKILL.md                 # 核心文件：元数据 + Agent 指令
├── skill.json               # 机器可读配置
├── agents/
│   └── openai.yaml          # UI 展示元信息
├── references/              # 公司、产品、FAQ、售前、竞品资料
│   ├── company.md
│   ├── products.md
│   ├── faq.md
│   ├── sales-playbook.md
│   └── competitors.md
├── README.md
└── LICENSE
```

## 安装

### 最简单的方式：告诉你的 AI 助手

直接把下面这句话发给你的 AI 助手：

> 帮我安装智书企飞 Skill，仓库地址：https://github.com/l17826834185-arch/ZS-QF-AI-Skill

Agent 会自动克隆仓库并安装到对应的 Skill 目录。

### 手动安装

克隆到本地 Skill 目录：

```bash
git clone https://github.com/l17826834185-arch/ZS-QF-AI-Skill.git \
  ~/.codex/skills/zhishu-qifei-skill
```

只要目录下有 `SKILL.md`，Agent 下次启动就会自动加载这个 Skill。

## 推荐提问

- 智书企飞有哪些产品？
- 合同审查场景适合哪个产品？
- 智书合同和智审平台有什么区别？
- 烽火适合什么客户？
- 和 e签宝 / 法大大 / 契约锁有什么区别？
- 这个客户场景怎么介绍比较合适？

## 信息边界

本 Skill 会优先基于 `references/` 内资料回答。涉及最新价格、部署方式、上线状态、客户案例、外部竞品信息时，应以最新官方资料或商务确认为准。

## 发布状态

| 项目 | 说明 |
|---|---|
| 协议 | Codex Skill |
| 当前版本 | 0.1.0 |
| 仓库地址 | https://github.com/l17826834185-arch/ZS-QF-AI-Skill |
| 可见性 | Private |

## License

MIT
