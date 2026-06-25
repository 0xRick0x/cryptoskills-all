---
name: cryptoskills
description: Use for Web3 crypto blockchain DeFi cross-chain security auditing and AI agent development tasks — activate on queries about Aave, Jupiter, Binance, OKX, Gate, Bybit, Bitget, Uniswap, PancakeSwap, GMGN, Polymarket or any major on-chain protocol and CEX/DEX agent skills. Compatible with Claude Code, Cursor, Codex, Cline.
compatibility: ["claude-code", "cursor", "codex", "cline", "other-agentskills"]
license: MIT
tags: ["crypto", "web3", "defi", "cross-chain", "security", "ai-agent", "binance", "okx", "gate", "bybit", "bitget", "uniswap", "pancakeswap", "gmgn", "polymarket"]
category: meta
---

# cryptoskills (元技能版)

> **来源**：cryptoskills.dev + Binance + OKX + Gate + Bybit + Bitget + Uniswap + PancakeSwap + GMGN + Polymarket
> **修改者**：Grok (xAI) 为用户 0xRick 定制

## 作用

集成了主流链上协议、CEX Agent、DEX AI Skills 和预测市场的核心知识，让 AI Agent 能同时掌握 DeFi 协议集成、CEX 交易、DEX 操作、Meme/Smart Money 分析和预测市场交易能力。

## 集成生态概览

| 类别           | 主要生态                          | 核心能力                     |
|-------------------|---------------------------------------------|-----------------------------------------|
| 链上协议   | cryptoskills.dev + Uniswap + PancakeSwap   | DeFi 集成、Swap、Liquidity、Hooks     |
| CEX Agent        | Binance + OKX + Gate + Bybit + Bitget      | Spot/Futures/Options + 机器人        |
| Meme / Smart Money | GMGN                                       | Trending、Smart Money、Token Analysis   |
| 预测市场     | Polymarket                                 | 市场查询、持仓分析、交易   |

## 具体能帮你做什么

**1. 链上 DeFi 协议集成**
- Uniswap / PancakeSwap Swap、Liquidity、Farming
- Aave、Jupiter、Morpho 等借贷和交换

**2. CEX 交易与机器人**
- Binance / OKX / Gate / Bybit / Bitget 现货、永续、期权交易
- 网格、DCA 策略、限价单

**3. Meme 币与 Smart Money 分析**
- GMGN Trending Tokens、Smart Money 跟踪、KOL 信号

**4. 预测市场交易**
- Polymarket 市场查询、持仓分析、事件交易

**5. 开发与安全**
- v4 Hooks 安全审查、Slither 快速审计
- viem / wagmi 集成

## 实用代码示例

### 1. Uniswap / PancakeSwap Swap
```ts
const tx = await uniswap.swap(quote);
// 或 PancakeSwap
```

### 2. Binance / OKX / Gate / Bybit / Bitget 交易
```ts
const res = await baw.swap({ fromToken: 'BNB', toToken: 'USDT', amount: '0.5' });
// 或 okxTrade.placeOrder(...)
// 或 gateFutures.placeOrder(...)
```

### 3. GMGN Trending + Smart Money
```ts
const trending = await gmgn.getTrendingTokens({ chain: 'sol', timeWindow: '1h' });
```

### 4. Polymarket 查询市场
```ts
const markets = await polymarket.gamma.getMarkets({ limit: 20, order: 'volume24hr' });
```

### 5. Polymarket 下单
```ts
const order = await polymarket.clob.placeOrder({
  market: 'marketId',
  outcome: 'Yes',
  side: 'BUY',
  price: 0.65,
  size: 100
});
```

## 响应与使用原则
- 优先使用安全审计和市场数据
- CEX 交易前建议使用安全审计 Skills
- 原版安装方式参见各自官方文档

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
- Polymarket API: https://docs.polymarket.com/cn/api-reference/introduction

此技能已集成主流链上协议、CEX Agent、DEX Skills 和预测市场生态。