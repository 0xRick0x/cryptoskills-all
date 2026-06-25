---
name: cryptoskills
description: Use for Web3 crypto blockchain DeFi cross-chain security auditing and AI agent development tasks — activate on queries about Aave Compound Jupiter Raydium LayerZero Wormhole Slither Foundry Viem Chainlink Binance Wallet Skills OKX Agent Gate AI Agent Bybit AI Trading Skill Bitget Agent Hub bitget-skill or any of the 97+ protocols and major CEX agent skills. Compatible with Claude Code, Cursor, Codex, Cline.
compatibility: ["claude-code", "cursor", "codex", "cline", "other-agentskills"]
license: MIT
tags: ["crypto", "web3", "defi", "cross-chain", "security", "ai-agent", "binance", "okx", "gate", "bybit", "bitget"]
category: meta
---

# cryptoskills (元技能版)

> **来源**：cryptoskills.dev + Binance + OKX + Gate + Bybit + **Bitget**  
> **修改者**：Grok (xAI) 为用户 0xRick 定制

## 作用

集成了 cryptoskills.dev、Binance、OKX、Gate、Bybit 和 **Bitget Agent Hub** 的核心知识，让 AI Agent 能同时掌握链上 DeFi 和多家 CEX 交易能力。

## Bitget Agent Hub 集成

Bitget 推出了 **Bitget Agent Hub** （https://github.com/Bitget-AI/agent_hub），包含 `bitget-skill` 和 `bitget-client` (bgc CLI)。

**主要特点**：
- 通过 `bgc` CLI 作为桥接，让 AI 直接操用 Bitget API
- 支持 Spot、Futures 交易、仓位管理、杀仓、设置杠杆
- 提供 bitget-skill （适配 Claude Code 等）
- 安全机制：写操作需确认、read-only 模式
- 还包含多个市场分析 Skill（macro-analyst、technical-analysis 等）

## 具体能帮你做什么

**1-3.** DeFi 集成、跨链、安全审计
**4.** Binance Wallet 操作
**5.** OKX CEX 交易 + 机器人
**6.** Gate AI Agent (CEX + DEX + 跨平台)
**7.** Bybit (Spot / Perpetual / Options)
**8. Bitget Agent Hub** — Spot/Futures 交易、仓位管理、市场数据查询

## 实用代码示例

### 示例 1-5: Aave / Jupiter / Binance / OKX / Gate (略)

### 示例 6: Bybit 永续交易
```ts
const order = await bybitTrade.placeOrder({ symbol: 'BTCUSDT', ... });
```

### 示例 7: Bitget 永续合约下单 (bitget-skill)
```ts
// 使用 bitget-skill + bgc CLI 下单
const result = await bgc.futures.placeOrder({
  symbol: 'BTCUSDT_UMCBL',
  marginCoin: 'USDT',
  size: '0.001',
  side: 'open_long',
  orderType: 'market'
});
```

### 示例 8: Bitget 查询余额和仓位
```ts
const balance = await bgc.account.getAccountList();
const positions = await bgc.futures.getPositions();
```

## 响应与使用原则
- 集成了 cryptoskills.dev + Binance + OKX + Gate + Bybit + **Bitget**
- 优先使用安全审计和市场数据
- 原版安装：`npx bitget-hub install --target claude` 或 `npm install -g bitget-skill bitget-client`

## 相关资源

- cryptoskills.dev
- Binance Wallet Skills
- OKX Agent
- Gate AI Agent
- Bybit AI Trading Skill
- **Bitget Agent Hub**: https://github.com/Bitget-AI/agent_hub
- bitget-skill: https://github.com/Bitget-AI/agent_hub/blob/main/docs/packages/bitget-skill.md

此技能已集成六大主流 AI Agent 技能生态。