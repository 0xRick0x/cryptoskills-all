---
name: cryptoskills
description: Use for Web3 crypto blockchain DeFi cross-chain security auditing and AI agent development tasks — activate on queries about Aave Compound Jupiter Raydium LayerZero Wormhole Slither Foundry Viem Chainlink Binance Wallet Skills OKX Agent Gate AI Agent Bybit AI Trading Skill Bitget Agent Hub Uniswap AI Skills PancakeSwap AI Skills GMGN AI Skills Polymarket API prediction-markets gamma-api clob-api or any of the 97+ protocols and major DEX/CEX/prediction market skills. Compatible with Claude Code, Cursor, Codex, Cline.
compatibility: ["claude-code", "cursor", "codex", "cline", "other-agentskills"]
license: MIT
tags: ["crypto", "web3", "defi", "cross-chain", "security", "ai-agent", "binance", "okx", "gate", "bybit", "bitget", "uniswap", "pancakeswap", "gmgn", "polymarket"]
category: meta
---

# cryptoskills (元技能版)

> **来源**：cryptoskills.dev + Binance + OKX + Gate + Bybit + Bitget + Uniswap + PancakeSwap + GMGN + **Polymarket**  
> **修改者**：Grok (xAI) 为用户 0xRick 定制

## 作用

集成了 cryptoskills.dev、多家 CEX Agent、多个 DEX AI Skills 和 **Polymarket API** 的核心知识，让 AI Agent 能同时掌握链上 DeFi、CEX 交易、DEX 集成、Meme/Smart Money 和预测市场交易能力。

## Polymarket API Skills 集成

Polymarket 推出了官方 **Polymarket API** （https://docs.polymarket.com/cn/api-reference/introduction），是全球最大的预测市场平台之一（基于 Polygon）。

**主要 API 分类**：

- **Gamma API** — 市场、事件、标签、搜索等公共数据（无需认证）
- **Data API** — 用户持仓、交易记录、排行榜、开放利息等分析数据
- **CLOB API** — 订单簿、价格、交易操作（部分端点需认证）

**优势**：
- 完整的预测市场交易能力
- 支持事件类型的交易（选举、体育、新闻等）
- 适合 AI Agent 进行信息收集和策略交易

## 具体能帮你做什么

**1.** DeFi 协议集成和 Uniswap/PancakeSwap Swap/Liquidity/Farming
**2.** 跨链和安全审计
**3-8.** Binance / OKX / Gate / Bybit / Bitget CEX 交易
**9.** GMGN — Solana Meme 币、Smart Money 跟踪
**10. Polymarket** — 预测市场查询、持仓分析、事件交易

## 实用代码示例

### 示例 1-8: Aave / Jupiter / Binance / OKX / Gate / Bybit / Uniswap / PancakeSwap (略)

### 示例 9: GMGN Trending Tokens
```ts
const trending = await gmgn.getTrendingTokens({ chain: 'sol', ... });
```

### 示例 10: Polymarket 查询市场 (Gamma API)
```ts
// 查询热门预测市场
const markets = await polymarket.gamma.getMarkets({
  limit: 20,
  order: 'volume24hr'
});
```

### 示例 11: Polymarket 下单 (CLOB API)
```ts
// 使用 CLOB API 下单（需要认证）
const order = await polymarket.clob.placeOrder({
  market: 'marketId',
  outcome: 'Yes',
  side: 'BUY',
  price: 0.65,
  size: 100
});
```

## 响应与使用原则
- 集成了 cryptoskills.dev + 多家 CEX + DEX Skills + GMGN + **Polymarket**
- 优先使用安全审计和市场数据
- 原版文档：https://docs.polymarket.com/cn/api-reference/introduction

## 相关资源

- cryptoskills.dev
- Binance Wallet Skills
- OKX Agent
- Gate AI Agent
- Bybit
- Bitget Agent Hub
- Uniswap AI Skills
- PancakeSwap AI Skills
- GMGN AI Skills
- **Polymarket API**: https://docs.polymarket.com/cn/api-reference/introduction

此技能已集成主流链上协议、CEX Agent、DEX Skills 和预测市场生态。