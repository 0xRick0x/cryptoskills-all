# cryptoskills-all

> 一个集成 **cryptoskills.dev** + **Binance Wallet Skills** 的 Web3 **元技能**（Meta Skill）

[![Upstream Check](https://github.com/0xRick0x/cryptoskills-all/actions/workflows/check-upstream-updates.yml/badge.svg)](https://github.com/0xRick0x/cryptoskills-all/actions/workflows/check-upstream-updates.yml)

将 [cryptoskills.dev](https://cryptoskills.dev) 的 97 个协议与 **Binance Wallet Skills** 打包整合为一个技能，让 AI Agent 能快速掌握 DeFi、跨链、钱包操作、市场信号和安全审计能力。

---

## ✨ 主要特性

- cryptoskills.dev 97 个协议 + Binance 8+ Wallet Skills 集成
- 完整中文说明 + 实用代码示例
- 每周自动检查上游并创建 PR
- 兼容 Claude Code、Cursor、Codex、Cline 等 AI 工具
- 支持 Binance Web3 Wallet 操作和市场能力

---

## 📌 来源与集成

- **cryptoskills.dev** 原始项目
- **Binance Wallet Skills** 官方集成
- 本仓库将两者打包为统一元技能，方便 AI 一站式调用

---

## 🚀 快速开始

```bash
# Clone
git clone https://github.com/0xRick0x/cryptoskills-all.git

# 复制到 AI 工具 skills 目录
cp -r cryptoskills ~/.claude/skills/

# 或者使用 Binance 官方安装
npx skills add binance-web3
```

---

## 🛠 具体能帮你做什么

| 场景               | 能力描述                                      |
|-----------------------|--------------------------------------------------|
| DeFi 集成           | Aave, Jupiter, Morpho, Drift 等集成             |
| Binance 钱包操作   | 转账、DEX 交换、限价单、预测市场     |
| 市场信号与 Meme | crypto-market-rank, meme-rush, trading-signal     |
| 安全审计           | query-token-audit + Slither 双重保障             |
| 钱包持仓查询     | query-address-info 快速查看持仓               |
| AI Agent 构建       | 自主执行链上操作（支持 Binance + 其他） |

---

## 📝 实用代码示例

详见 [`cryptoskills/SKILL.md`](cryptoskills/SKILL.md)，包含：

- Aave v3 Supply
- Jupiter Swap
- **Binance Agentic Wallet Swap**
- **query-address-info 查询持仓**
- Slither 审计

---

## ✅ 兼容工具

Claude Code • Cursor • Codex • Cline • Binance Skills Hub

---

## 🔄 自动同步

每周自动检查 cryptoskills.dev 和 Binance Skills Hub 更新，并创建 PR 提醒同步。

---

## 🤝 贡献

欢迎提交 PR 或 Issue 改进内容。

---

## 🔗 相关链接

- cryptoskills.dev: https://cryptoskills.dev
- Binance Wallet Skills: https://web3.binance.com/zh-CN/dev-docs/products/wallet-skills/supported-skills
- Binance Skills Hub: https://github.com/binance/binance-skills-hub

---

**AI 真正懂 Web3 — cryptoskills + Binance Skills**