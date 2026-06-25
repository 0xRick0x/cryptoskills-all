# cryptoskills-all

> 集成 **cryptoskills.dev** + **Binance Wallet Skills** + **OKX Agent** 的 Web3 **元技能**

[![Upstream Check](https://github.com/0xRick0x/cryptoskills-all/actions/workflows/check-upstream-updates.yml/badge.svg)](https://github.com/0xRick0x/cryptoskills-all/actions/workflows/check-upstream-updates.yml)

将三大主流 AI Agent 技能生态打包为一个统一元技能，让 AI 能快速掌握链上 DeFi + CEX 交易、安全审计和自动化策略。

---

## ✨ 主要特性

- cryptoskills.dev 97 个协议
- Binance Wallet Skills 集成
- **OKX Agent** 集成（现货/永续/期权 + 网格/DCA 机器人）
- 多个实用代码示例
- 自动上游监控 + PR 创建
- 兼容 Claude Code、Cursor、Codex 等

---

## 📌 集成来源

- cryptoskills.dev
- Binance Wallet Skills
- **OKX Agent Trade Kit**（官方支持现货/永续/期权/机器人）

---

## 🚀 快速开始

```bash
git clone https://github.com/0xRick0x/cryptoskills-all.git
cp -r cryptoskills ~/.claude/skills/

# Binance
npx skills add binance-web3

# OKX
npx skills add okx/agent-skills
```

---

## 🛠 具体能帮你做什么

| 场景             | 能力                                           |
|---------------------|----------------------------------------------------|
| DeFi 集成         | Aave, Jupiter, Morpho 等                           |
| Binance 钱包       | 转账、DEX 交换、限价单、安全审计       |
| **OKX CEX 交易**   | 现货/永续/期权下单、网格/DCA 机器人   |
| 安全审计       | Slither + query-token-audit                          |
| AI Agent 构建     | Binance + OKX + 链上自动化交易                 |

---

## 📝 实用代码示例

详见 SKILL.md，包含：

- Aave / Jupiter
- Binance Swap + Limit Order
- **OKX 下单** (okx-cex-trade)
- **OKX 创建网格机器人** (okx-cex-bot)
- **OKX 市场数据查询**

---

## ✅ 兼容

Claude Code • Cursor • Codex • Binance Skills • OKX Agent Skills

---

## 🔄 自动同步

自动监控 cryptoskills.dev + Binance + OKX 上游并创建 PR。

---

## 🤝 贡献

欢迎 PR 和 Issue。

---

## 🔗 链接

- cryptoskills.dev
- Binance Wallet Skills
- **OKX Agent**: https://www.okx.com/docs-v5/agent_zh/
- OKX GitHub: https://github.com/okx/agent-skills

---

**AI 真正懂 Web3 — 链上 + Binance + OKX**