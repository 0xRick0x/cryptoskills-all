# cryptoskills-all

> 一个为 **AI Coding Agents** 打包的 Web3 / Crypto 协议 **元技能**（Meta Skill）

[![Upstream Check](https://github.com/0xRick0x/cryptoskills-all/actions/workflows/check-upstream-updates.yml/badge.svg)](https://github.com/0xRick0x/cryptoskills-all/actions/workflows/check-upstream-updates.yml)

将 [cryptoskills.dev](https://cryptoskills.dev) 上的 97 个专业技能打包整合成一个技能，让 **Claude Code**、**Cursor**、**Codex**、**Cline** 等 AI coding agent 能够快速、准确地掌握主流区块链协议知识。

---

## ✨ 主要特性

- 将14个类别、15条链、97个主流协议打包为单个元技能
- 完整中文说明 + 具体实用场景
- 自动监控上游更新（每周自动创建 PR）
- 兼容 Claude Code、Cursor、Codex、Cline 等主流 AI 工具

---

## 📌 来源与修改

- **原始来源**： [cryptoskills.dev](https://cryptoskills.dev)（kukapay/crypto-skills）
- **本仓库优化**：
  - 打包为元技能（Meta Skill）
  - 大量中文说明和实用场景
  - 增加代码示例
  - 添加自动上游监控和 PR 创建

---

## 🚀 快速开始

```bash
# 1. Clone 本仓库
git clone https://github.com/0xRick0x/cryptoskills-all.git

# 2. 将 cryptoskills 文件夹复制到你的 AI 工具 skills 目录
cp -r cryptoskills ~/.claude/skills/          # Claude Code
# 或者复制到 Cursor / Codex 相应位置

# 3. 重启 AI 工具即可生效
```

---

## 🛠 具体能帮你做什么

| 场景           | 可以帮你完成的事情                              |
|-------------------|--------------------------------------------------|
| DeFi 集成       | Aave、Jupiter、Morpho、Drift 等集成代码         |
| 跨链操作       | LayerZero / Wormhole 桥接与消息传递             |
| 合约安全       | Slither、Mythril 审计流程和漏洞修复       |
| AI Agent 构建   | 让 AI 自主执行链上交易和跨链操作       |
| 前端 UX        | Privy + viem 钱包连接与交易体验优化       |
| 多链部署       | Arbitrum、Base、Solana 等多链部署方案       |

---

## 📝 实用代码示例

详细示例请查看 [`cryptoskills/SKILL.md`](cryptoskills/SKILL.md)。

包含：
- Aave v3 supply 示例（viem）
- Jupiter Swap 示例（Solana Agent Kit）
- Slither 快速审计命令

---

## ✅ 兼容工具

Claude Code • Cursor • Codex • Cline • 其他 agentskills.io 规范工具

---

## 🔄 自动同步机制

每周一自动检查原项目更新，若有新更新创建 Draft PR 提醒你同步内容。

---

## 🤝 贡献

欢迎提交 Issue 或 PR 改进内容或添加更多实用示例。

---

## 🔗 相关链接

- 原始项目：https://cryptoskills.dev
- 原始 GitHub：https://github.com/kukapay/crypto-skills
- 创建/贡献 Skill：https://cryptoskills.dev/contribute

---

**Let AI truly understand Web3.**