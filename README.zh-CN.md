[English](./README.md) | [中文](./README.zh-CN.md) | [日本語](./README.ja.md) | [Español](./README.es.md) | [Deutsch](./README.de.md)

# Awesome OpenClaw Agent Packs

**开箱即用的 OpenClaw AI Agent 模板包。选一个角色，部署到 Telegram，立刻开始工作。**

[![部署到 ClawPod](https://img.shields.io/badge/部署到-ClawPod-FF6B35?style=for-the-badge)](https://clawpod.app/templates)
![模板包](https://img.shields.io/badge/模板包-11-blue?style=for-the-badge)
![技能](https://img.shields.io/badge/技能-92-purple?style=for-the-badge)
![许可证](https://img.shields.io/badge/许可证-MIT-green?style=for-the-badge)

---

## 这是什么？

每个模板包都能把一个通用的 OpenClaw Agent 变成专业团队成员。**销售助手**帮你准备客户电话、调研潜在客户、撰写跟进邮件。**工程助手**帮你做站会、代码审查、事故响应。**法务分析师**帮你审查合同、检查合规。

每个模板包包含 6 个定义文件 + 完整的 `skills/` 技能目录：

```
packs/sales/
├── SOUL.md          # Agent 的人格（性格、价值观、沟通风格）
├── AGENTS.md        # 启动行为、可用技能、工作流程
├── HEARTBEAT.md     # 定时任务（每日简报、每周复盘）
├── TOOLS.md         # 连接的工具和 MCP 配置
├── MEMORY.md        # 跨会话的记忆结构
├── README.md        # 安装指南
└── skills/          # 9 个技能工作流
    ├── account-research/    → 调研任意公司或客户
    ├── call-prep/           → 带上下文准备销售电话
    ├── draft-outreach/      → 个性化邮件和 LinkedIn 消息
    ├── pipeline-review/     → 分析成交健康度、标记风险
    ├── forecast/            → 加权收入预测
    └── ...                  → + 更多 4 个技能
```

---

## 可用模板包

| 模板包 | 技能数 | 领域 | 部署 |
|--------|--------|------|------|
| [销售助手](./packs/sales/) | 9 | 销售与营收 | [![部署](https://img.shields.io/badge/部署-ClawPod-FF6B35)](https://clawpod.app/templates/sales) |
| [工程助手](./packs/engineering/) | 10 | 软件工程 | [![部署](https://img.shields.io/badge/部署-ClawPod-FF6B35)](https://clawpod.app/templates/engineering) |
| [数据分析师](./packs/data/) | 10 | 数据分析 | [![部署](https://img.shields.io/badge/部署-ClawPod-FF6B35)](https://clawpod.app/templates/data) |
| [营销策略师](./packs/marketing/) | 8 | 营销与内容 | [![部署](https://img.shields.io/badge/部署-ClawPod-FF6B35)](https://clawpod.app/templates/marketing) |
| [法务分析师](./packs/legal/) | 9 | 法律与合规 | [![部署](https://img.shields.io/badge/部署-ClawPod-FF6B35)](https://clawpod.app/templates/legal) |
| [财务分析师](./packs/finance/) | 8 | 财务与会计 | [![部署](https://img.shields.io/badge/部署-ClawPod-FF6B35)](https://clawpod.app/templates/finance) |
| [产品经理](./packs/product-management/) | 8 | 产品管理 | [![部署](https://img.shields.io/badge/部署-ClawPod-FF6B35)](https://clawpod.app/templates/product-management) |
| [人力资源](./packs/human-resources/) | 9 | HR 与人事 | [![部署](https://img.shields.io/badge/部署-ClawPod-FF6B35)](https://clawpod.app/templates/human-resources) |
| [客服支持](./packs/customer-support/) | 5 | 客户服务 | [![部署](https://img.shields.io/badge/部署-ClawPod-FF6B35)](https://clawpod.app/templates/customer-support) |
| [设计助手](./packs/design/) | 7 | UX 与设计 | [![部署](https://img.shields.io/badge/部署-ClawPod-FF6B35)](https://clawpod.app/templates/design) |
| [运营经理](./packs/operations/) | 9 | 业务运营 | [![部署](https://img.shields.io/badge/部署-ClawPod-FF6B35)](https://clawpod.app/templates/operations) |

---

## 快速开始

### 方式 A：一键部署（推荐）

1. 在上表中选一个模板包，点击 **部署到 ClawPod**
2. 输入你的 Telegram Bot Token
3. 30 秒后你的 Agent 就上线了：[clawpod.app](https://clawpod.app)

无需 Docker，无需 VPS，无需配置文件。

### 方式 B：自托管（OpenClaw）

```bash
git clone https://github.com/clawpod-app/awesome-openclaw-agent-packs.git
cp -r awesome-openclaw-agent-packs/packs/sales/* ~/.openclaw/workspace/
openclaw gateway restart
```

Agent 启动时自动读取 `SOUL.md`，加载 `skills/` 中的技能，立即开始工作。

### 方式 C：手动安装

1. 将任意模板包复制到你的 OpenClaw workspace 目录
2. 按 `TOOLS.md` 配置 API 密钥和 MCP 工具
3. 重启你的 Agent

---

## 技能如何工作

技能是文本化的工作流程指南，不是可执行脚本。当用户问"帮我调研 Acme 公司"时，Agent 会：

1. 读取 `skills/account-research/SKILL.md`
2. 按照里面定义的工作流程逐步执行
3. 使用可用的工具（网页搜索、MCP 连接器）完成任务
4. 返回结构化结果

技能默认通过网页搜索即可工作。连接 MCP 工具（CRM、邮件、日历）后效果更好，但不连接也完全可用。

---

## 贡献

欢迎提交新的模板包！要求：

1. 包含全部 6 个核心文件：`SOUL.md`、`AGENTS.md`、`HEARTBEAT.md`、`TOOLS.md`、`MEMORY.md`、`README.md`
2. 至少一个带完整 `SKILL.md` 工作流的技能
3. 在真实的 OpenClaw 或 ClawPod 实例上测试通过
4. README 包含安装步骤和示例对话

参考任意现有模板包了解格式要求。

---

## 来源

改编自 [Anthropic 的 Knowledge Work Plugins](https://github.com/anthropics/knowledge-work-plugins)（Apache-2.0 许可）。详见 [NOTICE](./NOTICE)。

## 许可证

MIT 许可。Knowledge Work 技能衍生自 Anthropic 的 Apache-2.0 许可作品。详见 [LICENSE](./LICENSE)。

---

*由 [ClawPod](https://clawpod.app) 维护 — 30 秒部署你的 AI Telegram Bot。*
