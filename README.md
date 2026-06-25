# cryptoskills-all

> 集成 **cryptoskills.dev** + **Binance** + **OKX** + **Gate** + **Bybit** 的 Web3 **元技能**

[![Upstream Check](https://github.com/0xRick0x/cryptoskills-all/actions/workflows/check-upstream-updates.yml/badge.svg)](https://github.com/0xRick0x/cryptoskills-all/actions/workflows/check-upstream-updates.yml)

将五大主流 AI Agent 技能生态打包为一个统一元技能，让 AI 能同时掌握链上 DeFi 和多家主流 CEX 交易能力。

---

## ✨ 主要特性

- cryptoskills.dev 97 个协议
- Binance + OKX + Gate + **Bybit** 集成
- Bybit 官方 AI Trading Skill + MCP Server
- 多个实用代码示例
- 自动监控上游 + PR
- 兼容 Claude Code、Cursor、Codex 等

---

## 📌 集成来源

- cryptoskills.dev
- Binance Wallet Skills
- OKX Agent
- Gate AI Agent
- **Bybit AI Trading Skill & MCP Server**

---

## 🚀 快速开始

```bash
git clone https://github.com/0xRick0x/cryptoskills-all.git
cp -r cryptoskills ~/.claude/skills/

# Binance
npx skills add binance-web3

# OKX
npx skills add okx/agent-skills

# Gate
npx skills add gate/gate-skills

# Bybit
npx skills add bybit-exchange/skills
# 或者使用 MCP Server
npx bybit-official-trading-server@latest
```

---

## 🛠 具体能帮你做什么

| 场景               | 能力                                           |
|-----------------------|----------------------------------------------------|
| DeFi 集成           | Aave, Jupiter 等                                   |
| Binance 钱包       | 转账、DEX 交换、限价单               |
| OKX CEX               | 现货/永续/期权 + 网格/DCA 机器人     |
| Gate AI Agent         | CEX + DEX + 跨平台 + 市场研究             |
| **Bybit**             | **Spot / Perpetual / Options 交易 + MCP**         |

---

## 📝 实用代码示例

详见 SKILL.md，包含 Bybit 永续合约下单等示例。

---

## ✅ 兼容

Claude Code • Cursor • Codex • Binance • OKX • Gate • Bybit

---

## 🔄 自动同步

自动监控五大上游并创建 PR。

---

## 🤝 贡献

欢迎 PR 和 Issue。

---

## 🔗 链接

- cryptoskills.dev
- Binance Wallet Skills
- OKX Agent
- Gate AI Agent
- **Bybit**: https://github.com/bybit-exchange/skills
- Bybit MCP: https://www.npmjs.com/package/bybit-official-trading-server

---

**AI 真正懂 Web3 — 链上 + Binance + OKX + Gate + Bybit**