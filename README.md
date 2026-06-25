# cryptoskills-all

> **集成主流链上协议 + CEX Agent + DEX Skills + 预测市场的 Web3 元技能**

[![Upstream Check](https://github.com/0xRick0x/cryptoskills-all/actions/workflows/check-upstream-updates.yml/badge.svg)](https://github.com/0xRick0x/cryptoskills-all/actions/workflows/check-upstream-updates.yml)

将 **cryptoskills.dev**、**Binance**、**OKX**、**Gate**、**Bybit**、**Bitget**、**Uniswap**、**PancakeSwap**、**GMGN** 和 **Polymarket** 的核心能力打包为一个统一元技能，让 AI Agent 真正具备全栈 Web3 操作能力。

---

## ✨ 核心亮点

| 亮点               | 说明                                      |
|--------------------|-------------------------------------------|
| **多生态覆盖**     | 链上 DeFi + 5 大 CEX + DEX + Meme + 预测市场 |
| **高级组合用法**   | 提供多个跨平台协同实战示例                 |
| **实用性强**       | 包含真实交易流程和风险管理思路             |
| **持续维护**       | 自动监控上游更新并创建 PR                  |
| **即插即用**       | 兼容 Claude Code、Cursor、Codex 等主流工具 |

---

## 📦 集成生态

| 类别               | 主要来源                                      | 核心能力                              |
|--------------------|-----------------------------------------------|---------------------------------------|
| **链上 DeFi**      | cryptoskills.dev + Uniswap + PancakeSwap     | Swap、Liquidity、Farming、Hooks       |
| **CEX Agent**      | Binance + OKX + Gate + Bybit + Bitget        | Spot/Futures/Options + 机器人         |
| **Meme & Smart Money** | GMGN                                     | Trending、Smart Money 跟踪            |
| **预测市场**       | Polymarket                                    | 市场查询、持仓分析、事件交易          |

---

## 🚀 快速开始

```bash
git clone https://github.com/0xRick0x/cryptoskills-all.git
cp -r cryptoskills ~/.claude/skills/

# 安装 CEX Agents
npx skills add binance-web3
npx skills add okx/agent-skills
npx skills add gate/gate-skills
npx skills add bybit-exchange/skills
npx bitget-hub install --target claude

# 安装 DEX Skills
npx skills add Uniswap/uniswap-ai
npx skills add PancakeSwap/pancakeswap-ai

# 安装 GMGN
npx skills add GMGNAI/gmgn-skills

# Polymarket 使用官方 API
```

> **提示**：推荐根据实际需求按需安装，不必一次性安装所有 Skills。

---

## 📖 详细使用指南

想深入了解如何高效组合不同平台的 Skills？

请阅读 **[USAGE.md](./USAGE.md)**，其中包含：

- 推荐的跨平台组合实战流程
- 安全最佳实践
- 常见问题解答
- 进阶使用建议

---

## 🛠 具体能帮你做什么

### 🔹 链上 DeFi 协议集成
- Uniswap / PancakeSwap 的 Swap、添加流动性、Farming
- Aave、Jupiter、Morpho 等借贷与收益策略

### 🔹 CEX 交易与自动化
- Binance / OKX / Gate / Bybit / Bitget 现货、永续、期权交易
- 支持网格、DCA、限价单、批量操作

### 🔹 Meme 币与 Smart Money 分析
- GMGN 实时 Trending Tokens
- Smart Money / KOL 买入信号跟踪
- Token 基础面 + 链上数据分析

### 🔹 预测市场交易
- Polymarket 市场发现、持仓查询、下单交易

### 🔹 开发与安全
- Uniswap v4 Hooks 安全审查
- Slither 快速审计 + viem/wagmi 集成

### 🔹 高级组合策略（推荐）
- **GMGN 信号 → CEX/DEX 执行**
- **Polymarket 分析 → CEX 对冲**
- **Meme 币分析 → DEX 流动性 + CEX 风险对冲**
- **多 CEX 价差套利 + On-chain 对冲**

---

## ✅ 兼容平台

`Claude Code` • `Cursor` • `Codex` • `Binance` • `OKX` • `Gate` • `Bybit` • `Bitget` • `Uniswap` • `PancakeSwap` • `GMGN` • `Polymarket`

---

## 🔄 自动同步更新

GitHub Action 会定期检查上游项目更新，并自动创建 Pull Request，保持内容最新。

---

## 🤝 贡献

欢迎通过 Issue 或 Pull Request 贡献新的示例、优化文档或提出建议。

---

## 🔗 相关链接

- [cryptoskills.dev](https://cryptoskills.dev)
- [Binance Wallet Skills](https://web3.binance.com)
- [OKX Agent](https://www.okx.com/docs-v5/agent_zh/)
- [Gate AI Agent](https://www.gate.com/docs/developers/agent/zh_CN/)
- [Bybit AI Trading Skill](https://github.com/bybit-exchange/skills)
- [Bitget Agent Hub](https://github.com/Bitget-AI/agent_hub)
- [Uniswap AI Skills](https://developers.uniswap.org/docs/uniswap-ai/skills)
- [PancakeSwap AI Skills](https://pancakeswap.ai/skills/)
- [GMGN AI Skills](https://github.com/GMGNAI/gmgn-skills)
- [Polymarket API](https://docs.polymarket.com/cn/api-reference/introduction)
- [详细使用指南 (USAGE.md)](./USAGE.md)

---

**让 AI 真正理解并操作整个 Web3 世界** 🚀